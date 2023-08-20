---
title: "Creating Releases"
tags: documentation, devops, internal
date:
  created: "10/06/2022"
  modified: "10/06/2022"
description: Resource for developer operations. For internal use only.
---

# Creating Releases

This is still a work in progress. There are multiple steps even in the lower numbers that need to be expanded. Please feel free to add comments and I’ll update this main mess to reflect them.

1. Verify that all “Ready to Merge” MR that target the release branch have been merged
2. If this is a beta release, merge any earlier point release branches into this mergeback any branches from prior point releases
3. Verify that the final pipeline for the build completed successfully and make a note of the pipeline id
4. Let the System Test team know that they should start smoke testing
5. Wait for smoke testing to complete before proceeding
6. Checkout the branch we’re releasing
7. Create a new branch named `release/v<next-version-number>`
8. Change RELEASE_VER in gitlab-ci.yml to match `next-version-number`
9. Commit change using message `[skip-ci] Updated sled release version to <next-version-number>`
10. Push branch upstream
11. Tag release/v<version-being-released> as `v<version-being-released>`
12. Push tag upstream
13. Look at all non-“Ready to Merge” MR that target the release branch
14. All of the branches from the prior step should be changed to target `release/v<next-version-number>`
15. Create a new release in Jira for the `next-version-number` release
16. Open the release we’re releasing in Jira
17. If there are “Issues in Progress”
    1. Click the `Issues in Progress` link in the header to see only those issues
    2. Click the `View in Issue Navigator` link on the right side of the header
    3. Click the ellipsis button in the top right just under your avatar/profile icon
    4. Select the `Bulk change all xxx issues` option from the drop down
    5. Highlight all of the issues and click the `Next` button
    6. Select the `Edit Issues` radio button and then click the `Next` button
    7. Use the `Change fix versions` option to add `next-version-number` to each of the issues
    8. When finished, go back to the `Change fix version` page and remove the fix version we’re releasing
18. Navigate back to the release we’re releasing in Jira and click the `Release` button
19. Let the documentation team know that they can now create the release notes
20. Let DevOps (Currently Paul Ward) know about the release and provide the final pipeline id
    1. Update the golden disk image if appropriate
    2. Release the update (Process TBD)
21. Mergeback this release into develop
    1. Create a `mergeback-<release-version>` branch based on the release branch
    2. Merge develop into the `mergeback-<release-version>` branch and resolve any conflicts
    3. Push the `mergeback-<release-version>` branch to origin
    4. Create an MR for the `mergeback-<release-version>` branch targeting develop



