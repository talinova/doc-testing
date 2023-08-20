---
title: "Release notes - SAVI - Version 3.3.0"
tags: release, notes, 3.3.0
date:
  created: "01/24/2023"
  modified: "01/30/2023"
description: Jan 2023
---

# Release notes - SAVI - Version 3.3.0


# Internal 
## Backend
* Dealers can now install canvas firmware
* Resolvers for ducking
* System startup now clears "pulling screenshot" flag

## Canvas
* Added support for region.width and region.height in IFrame URL values
* Fixed webOS LineIn Issue

## Creator 
* DNS settings are no longer required
* Fixed project export API when the topgolfAPI feature flag is enabled
* Macros now only show "edit arguments" modal when argument present
* Removed Rs232 EMITCONFIG Command
* Disabling RTSP on Stream.One now works properly
* Wide L-shaped layouts now correctly arranged
* Update SAVI Server firmware now displays upload/install information

## DevOps
* Added id values to the DOM for test automation
* Now linting files that are deeply nested in the monorepo
* Add script to report canvas displays temperature
* Port license.supportExpiresAt from SN-2608 to develop
* Moved daemon --config into a plugin
* Artifacts for savi builds are now saved on in the CI pipeline
* Fixed issue with artifact file names in package build step
* Software install now allows overriding root directory by including ROOT\_DIR env variable
* Switched from nodejs 12.16.1 to 12.20.2
* Revert removed token validation code for the creator websocket server
* aes70 daemon no longer requires ports

## Drivers
* Meta Functionality Improvements
* Removed DeviceVariables from collection injected into drivers
* Re-factor cache for DSP I/Os
* Humax Sky esd-160s Satellite now correctly named
* Fixed an issue with tileMode fields and streaming latency
* webOS tuner driver no longer logs errors with \`attachDevce is not a function\`

## Floor Plan
* Added permissions for map views

## SAVI Show
* Aspect '8:1 Slim Wide' has been renamed to '7:1 Slim Wide'


# External
## What’s New

### Map View 

SAVI’s newest, no-code feature delivering a holistic and nested bird’s eye view of your entire AV system. Perfect for a neighborhood bar or a professional sports stadium with thousands of end points, it’s never been easier for integrators to deliver a visually intuitive tool to their customers. 

TL;DR 

*	No coding required to create a full-scale system map 
*	Simply upload a floor plan to Creator, add and edit endpoints 
*	Maps can be nested and organized by location, room, level, or zone
*	With Multi-Select, Multi-Edit, Previewer, and filterable devices and endpoints
*	The new Quick Find “@” feature lets you view exactly where sources are distributed 

### Game View 
Game View is a game changer come game time, aggregating current and future sporting event data into a simple and irresistibly stylish view. Search by team or filter by sport to see upcoming athletic events at-a-glance. Game View provides a visually informative schedule complete with team logos, colors, and program data making it easy and fun to fulfill any fan’s fantasy, any time. 

TL;DR
*	Aggregates current and future sporting event data into a simple and modern view
*	Search by team or filter by sport to see upcoming athletic events at-a-glance and schedule games up to four days in advance
*	Game View’s schedule is complete with team logos, colors, and program data making it quick and easy to fulfill any obscure sports fan’s request 

### SAVI Show 
SAVI Show puts content creation, distribution, and management in the hands of everyday users. Simplified at every step, from basic signage to custom layouts, users can easily upload multiple files at once, create slideshows, and distribute content to any display, anytime– all without the cost of complicated digital signage solutions.

TL;DR
*	You don’t have to integrate an additional digital signage player. Everything else below is just a bonus. 
*	Dedicated storage for content like slideshows, logos, ads, menus, and more
*	BYOD with drag/ drop and bulk upload functionality
*	Create looping slideshows with settings for duration, transitions, and speed
*	SAVI Show auto categorizes content for Canvas Layouts based on aspect ratios
*	Create custom tags, filters, and categories
*	Facility View auto displays matching content based on aspect ratio and displays a Preview of the content 

### Refreshed Facility View
Refreshed and reimagined, Facility View delivers a faster, more intuitive user experience with elevated design treatments and even more built-in features. Give your thumbs a break from endless scrolling with our new mobile design providing superior control capabilities across a wide range of devices. 

TL;DR 
*	Canvas Layouts are now conveniently organized into an illustrative dropdown menu with thumbnails for matching content in the source pane and the selected layout region 
*	Guide and Scheduler’s mobile-friendly functionality allows users to search, schedule, and change content from anywhere. Filter by genre, program name, or channel name and view scheduled content by source or endpoint   
*	Enhanced search functionality within the source pane allows you to find exactly what you're looking for in seconds
*	Updated Multi-Select allows you to choose and change video, audio and lighting settings across all zones
*	Macros now include action descriptions with selectable, two-step prompts so large commands aren’t accidentally executed

### Downloadable SAVI Software and LG webOS firmware updates
Once on SAVI 3.3.0, you can download the newest SAVI software from the dealer portal and update your project in the Creator updates module. Firmware updates for your LG webOS displays are also available directly in Creator. 

TL;DR
*	Download future SAVI updates once you’re on SAVI 3.3.0 
*	LG webOS display firmware updates are also now available

## Enhancements

*	We’ve improved Creator’s UX and workflows by renaming buttons for increased clarity (“Add Driver to Project” to “Create Custom Driver”), refocusing cursors, and organization fields and properties for more intuitive navigation

## Drivers
### New
*	BSS London BLU-800
*	STREAM.One 4K
*	Alfatron ALF-DSP88-U

### Improved 
*	Renamed Zektor to Pulse-Eight and added setEQ command
*	Generic Telnet Device now supports hex codes in the send Command argument
*	DBX now unmutes after playing a source
*	Kramer VS now has input ports
*	Thermostat Cool/Heat points can now be changed on the device itself
*	COM51 Tuner no longer sends config at process startup
*	Ovation Player can now play Spotify playlists
*	Individual buttons now work with Sony Bravia driver

## Bug Fixes
*	We fixed the Canvas Dashboard stability issue when importing projects in Creator
*	Single source audio is now enabled for displays with Canvas Layouts and multiple content sources
*	All valid macros now execute even when invalid commands are present, helping ensure your projects are running seamlessly
*	The video preview in Creator has also been fixed when disconnecting and connecting sources to SAVI STREAM.Ones, no longer displaying previous URLs
*	Endpoint metadata for SAVI Show content has been corrected when displaying in Canvas Layouts in Facility View
*	The drivers module in Creator now offers a more straightforward configuration with the removal of the multiple connection option to line level inputs

## How to Update
*	How to get SAVI 3.3 (link)
*	How to update once on SAVI 3.3 (link)

## Depreciated 
*	SAVI 3.3.0 no longer supports Control4 integration 



# Known Issues
