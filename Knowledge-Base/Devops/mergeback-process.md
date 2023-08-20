---
title: "General Mergeback Process"
tags: documentation, devops, internal
date:
  created: "10/06/2022"
  modified: "10/06/2022"
description: Resource for developer operations. For internal use only.
---

# General Mergeback Process


Merging back is a process that happens when changes made to a specific branch need to be part of other branches we’re working on. The most common use case is when we’re creating a release of the software. Typically, those changes should be made part of the `develop` branch so that the changes automatically become part of all future releases.

When we’re performing a mergeback the `Mergeback Source` is the branch that we’re merging from and the `Mergeback Target` is the branch that we’re merging to. For example, when we’re releasing version 3.2.0, the source branch would be `release/v3.2.0` and the target branch would normally be `develop`.

Process to mergeback branches:

1. Inform the team that they should not perform any merges on the `Mergeback Target` branch
2. Checkout the `Mergeback Source` branch
3. Create a new branch named `mergeback-<source-branch-name>`
4. Merge the `Mergeback Target` branch into `mergeback-<source-branch-name>` and resolve any conflicts
5. Push `mergeback-<source-branch-name>` to your origin fork
6. Create an MR to merge `mergeback-<source-branch-name>` into the target branch
7. Verify that the MR is set to ***not*** squash commits
8. Set the MR to merge on success
9. Wait for the MR to merge
10. Inform the team that merges can now be performed on the `Mergeback Target` branch 