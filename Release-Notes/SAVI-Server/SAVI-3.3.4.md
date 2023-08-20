---
title: "Release notes - SAVI - Version 3.3.4"
tags: release, notes, 3.3.4
date:
  created: "08/01/2023"
  modified: "08/07/2023"
description: Aug 2023
---

# Release notes - SAVI - Version 3.3.4


# Bug Fixes
## Creator
* Fixed problem when restoring projects with SAVI Show images
* SAVI Link modal now matches the DSP UI View
* "Revert" button now works on more fields
* Log Out button now shows correct mouse pointer
* Main menu is no longer hidden by other windows
* setColor argument now correctly assigns color
* Fixed a bug causing QSYS systems to reboot
* Fixed a bug that caused graphql server to constantly restart
* Now correctly able to control custom serial driver as display

## Drivers
* WP400 serial support now works with hex values above \\x7F
* DSP now works better with larger DSP project files
* Fixed problems with properly decrypting DSP password

## DSP
* Fixed a bug preventing adding SAVI Links after removing them from Creator UI

## Facility
* Users can now assign view-only sources to endpoints they can control
* Buttons in the remote modal now correctly link to Guide & Scheduler and Game View
* Project Name is now included in the Facility View UI
* Program guide airings are now correctly filtered by serviceId
* Removed LED Color settings from Light Driver
* Fixed a bug preventing scrolling through SAVI Show images on mobile
* Selecting a Show region on mobile now correctly allows selecting images
* Mobile View selection count no longer includes hidden endpoints
* Fixed bug where rotating the screen in Mobile View would hide half of the page
* Fixed a bug where Audio Zones would deselect while editing presets
* Presets are no longer visible if the selected filter does not include related displays
* Layouts that are not shared between multi-selected displays are now correctly hidden
* Selecting an Audio Zone endpoint now correctly moves right pane scroll position to Volume options
* Altering the volume of Audio Zones is now faster
* Special Permissions tooltip under User Management no longer incorrectly references Maps
* Selecting SAVI Show image on mobile no longer cuts off Cancel button
* Fixed a bug where "Multiple Show Images" Icon would not always appear in the Layout Preview
* Fixed a bug where changes to endpoints in Facility View were sometimes not updated
* Meta drivers now correctly able to send setInput commands
* SAVI no longer crashes when selecting Map View preview
* Fixed a bug where MEGA Enlighten LEDs sometimes did not update in the UI
* Improved facility view performance

## Game View
* Fixed a bug created when TVMedia logo site was unavailable

## Live Data
* Fixed some issues with automatic data refresh for non-admin users

## Map View
* Endpoints are now correctly selected after changing layouts
* Metadata on display endpoints now correctly display SAVI Show media
* Fixed a bug in Map View where the Preview button sometimes displayed a white screen
* Fixed a bug where the small Lighting Icon would not correctly appear
* Fixed a bug where LED Endpoints would sometimes flicker when changed

## Show
* Search for Displays now correctly shows text in the search bar
* Image upload is now limited to 50 images at a time
