---
title: "Release notes - SAVI - Version 3.2.3"
tags: release, notes, 3.2.3, internal
date:
  created: "12/21/2022"
  modified: "01/25/2023"
description: Dec 2022
---

# Release notes - SAVI - Version 3.2.3


# Internal
## DevOps
* Fixed project export API when the topgolfAPI feature flag is enabled
* aes70 daemon no longer requires ports
* Add script to report canvas displays temperature

## Canvas
* Restoring project with screenshots no longer breaks dashboard

## Driver
* Added support for BSS London BLU-800
* Added support for Alfatron - ALF-DSP88-U
* Rename Zektor to Pulse-Eight and added setEQ command
* Generic Telnet Device now supports hex codes in the sendCommand argument
* COM51 Tuner no longer sends config at process startup