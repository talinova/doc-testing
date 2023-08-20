---
title: "Release notes - SAVI - Version 3.1.2-hf4"
tags: release, notes, 3.1.2, hf4, internal
date:
  created: "06/21/2022"
  modified: "01/25/2023"
description: June 2022
---

# Release notes - SAVI - Version 3.1.2-hf4


# Internal
## DevOps 
* Port CI squashfs image building to 3.1.2-hf4 line

## Creator
* Devices without a location no longer cause Connections to crash
* Fixed issue where autodiscovery failure caused driver process to restart

## Drivers
* RGB Galileo Layout now includes a "Surface" argument on the setLayout and setLayoutManual commands
* Canvas line input regions now properly scale for UH5L
* Fixed Back, Cancel and Set Input buttons for Sony Simple IP
