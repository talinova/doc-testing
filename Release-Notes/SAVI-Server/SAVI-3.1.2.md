---
title: "Release notes - SAVI - Version 3.1.2"
tags: release, notes, 3.1.2, internal
date:
  created: "04/28/2022"
  modified: "01/24/2023"
description: April 2022
---

# Release notes - SAVI - Version 3.1.2


<!---
project = 00000 AND fixVersion = 00000 AND labels != TitleReviewed ORDER BY priority DESC, key ASC
--->

# Internal 
## Canvas
* Layouts now support YouTube regions
* Added additional templates for L-Shaped Wide
* UH5F now properly rotates line input regions

## Creator
* Added a Source Change event to Macros in Audio Zones
* Canvas Network device is no longer visible
* Device names no longer overflow in Macros tab
* Fixed issue where selecting all connections can overwrite connections
* SAVI Macro COM51 Reset - Does not work with Slot 2 board

## Driver
* Triad AMS now supports TMS-8
* Changed Connect.One IR Module default Delay After Success/Failure
* COM51 Tuner Advanced Preview function
* Control4 drivers have been removed
* Added support for Binary 660 Series 4K HDR HDMI Matrix Switcher - 4x4 \(IP\)
* Added support for Binary 120 Series 4K HDR HDMI Matrix Switcher - 8x8 \(rs232\)
* Added support for Planar UltraRes X Series driver \(IP\)
* COM51 Tuner now has an optimized control UI
* COM51 Tuner can now control "closed" channels
* Changed default Min/Max Gains in QSC QSYS Level Driver
* Added support for Sony BRAVIA TV display \(IP\)
* Fixed issue with Qsys Core Router driver crashing

## Facility View
* Thermostat now shows proper data
* Backport SN-2133 Source Save/Restore
* Added user profile modal
* Fixed issue with "play" command timing out when playing on multiple devices
* Program data now includes \`new\`, \`repeat\` and \`live\` fields
* Team Logos no longer appear on replay games

## Map View
* Televisions can now be added

## Scheduler
* New "Game View" interface
* Added support for caching guidedata for team logos
* Fixed issue where only 24 hours of data is visible
* Fixed overflow issue with first time slot
* Optimized for larger screens

## Scene Selector
* Can now delete and edit scenes
  * If an installer clicks `Close_Channel` on a tuner from the COM3000 management webui, it would previously prevent SAVI from controlling that tuner. This is now fixed.

## Uncategorized  
* Removed sled-app-2 from monorepo
* Add "Game View" button to DTV Modal
