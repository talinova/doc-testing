---
title: "Release notes - SAVI - Version 3.1.2-hf10"
tags: release, notes, 3.1.2, hf10, internal
date:
  created: "08/24/2022"
  modified: "01/25/2023"
description: Aug 2022
---

# Release notes - SAVI - Version 3.1.2-hf10


# Internal
## DevOps
* Backport SN-2597 (static networking fix) to 3.1.2
* Backport (SN-2665 to 3.1.2) Scheduler: driver-scheduler occasionally restarts with out of heap errors

## Drivers
* Increase Q-Sys Router driver inputs and outputs to 64
* Added generic http driver with a `getURL` command to perform http get operations
