---
title: "Merging Branches"
tags: documentation, devops, internal
date:
  created: "10/06/2022"
  modified: "10/06/2022"
description: Resource for developer operations. For internal use only.
---

# Merging Branches


Merging SN-XX branches
1. Make sure story fix version matches up with target branch of MR
2. Hit the rebase button on the MR if it exists
3. If rebase fails or it says rebase has to be done manually, yell at the assignee
4. On the MR page in Gitlab, view the Changes tab
5. If you don’t see the tree towards the left below where it says “Compare XXX and XXX”, click the tree button next to “Compare XXX and XXX”
6. If there’s a file listed in the tree that’s inside the “lerna/packages/sled-core/migrations/migrations” folder, holler at the developer or paul to verify whether it needs to be renamed to be ordered correctly within that folder.
7. Merge the MR
8. If the target branch is ‘develop’ gitlab will update the Jira story to ‘Done’ automatically. Otherwise, manually update the story yourself once the merge completes

* make sure the branch it's targeting is not already released or on a code freeze
* rebase with the test - always
* check that the reviewer in the issue marked approval of the MR
* perhaps do a control+f for console - since it isn’t always caught by lint or the reviewer
    * definitely would appreciate step 7 (edited) 
