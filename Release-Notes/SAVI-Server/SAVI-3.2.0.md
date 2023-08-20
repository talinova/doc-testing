---
title: "Release notes - SAVI - Version 3.2.0"
tags: release, notes, 3.2.0, internal
date:
  created: "12/21/2022"
  modified: "12/21/2022"
description: Oct 2022
---

# Release notes - SAVI - Version 3.2.0


<!---
project = 00000 AND fixVersion = 00000 AND labels != TitleReviewed ORDER BY priority DESC, key ASC
--->

# Internal 
## Backend
* Pin node module versions now reconcile for build stability
* http error log entries now include url
* Backport \(SN-2665 to 3.1.2\) Scheduler: driver-scheduler occasionally restarts with out of heap errors
* HTTP request errors are now logged

## Canvas
* webOS app now allows playing a stream by entering some data directly in the :9998 UI
* Updated UL3J firmware with LG release supporting Pro:Idiom
* Dashboard now requires admin rights
* Canvas displays/tuners no longer use WP400s for their layout control 
* IFrame URL now supports inserting canvas device mac address
* Network instability now causes fewer problems with initial handshake
* Clear cache no longer opens port 9998 on the device
* Can now assign Canvas display to physical display and interact with Display in Canvas Dashboard
* Fixed issue with tile mode not scaling properly
* L-Shaped Wide, Inverted, Mirrored Inverted templates now have correct dimensions

## Creator
* Autodiscovery now supports stream.one
* Macros can now be run as part of another macro
* Cleanup import license code
* Removed the facilityV2 and show Feature Flags
* Removed old creator source
* Endpoints no longer snap to the grid
* Popout menu options have moved to the header
* Now able to upgrade SAVI app to 3.2.x from previous versions without wiping project
* Serial number is now visible
* On project import/clear, the show images and maps folders are now cleared
* Drivers built with the wizard can now be deleted
* 'Source Changed' macros can fire on any source in addition to specific source
* Improved modal text weights
* Included a 'Cancel' button when adding an Endpoint on the Map View
* STREAM.One drivers now have an additional textbox for RTSP Multicast Port
* Fixed issue with Creator crashing when a SAVI Show Slideshow has 0 images
* Devices without a location no longer cause Connections to crash
* Fixed issue with syncing Primary SAVI Server to Secondary SAVI Server
* Corrected IP Address when DHCP is on
* Expired/Invalid logins are now detected quicker and handled better
* Added option to log out
* Audio Zone Alt. Volume Control is now blank by default
* Fixed issue editing multiple COM51 Tuner devices
* List of drivers in Equipment now ignores capitalization when sorting
* Can now edit Location Name
* Floor Plan editor no longer shows the same location twice
* Added a warning when unsaved changes may be lost do to an action
* Spaces before an IP entry are now truncated
* Rebooting now only reboots a single time
* Fixed an issue preventing enabling NTP 
* Delay option in macros now defaults to 500 ms
* Attempting to set server to DHCP no longer fails
* Ubuntu 18.04 servers can now use static networking
* Added space between Layout cards
* Removed SAVI show flag logic from Creator layout editor
* Fixed Equipment & Connection Search Selection bug 
* Fixed an issue where Displays were listed out of order
* Floor Plan: Fixed Button function
* Changes in Creator are now reflected in Facility View without a refresh
* Fixed Macro Container Macro Device Selection
* Map View 'Place Endpoint' grid now automatically resizes
* Map view now only allows saving when required fields are filled
* Favorite Channels now update properly
* Blocked Channels no longer display in Scheduler or Facility
* Auto Discover no longer discovers webOS displays with the Canvas app already installed
* Fixed Auto-Discovery selection behavior
* Improved error checking related to autodiscover
* Fixed an issue causing a redirect loop after clearing a project
* Macro commands that are missing arguments now have a warning
* Device edit now alerts user with a toast when a save fails validation
* Migration failures now prevent the system from starting
* Thermostat no longer incorrectly converts Fahrenheit to Celsius when set to Fahrenheit
* Sensor client now correctly stores state
* Clicking on a command in Macros that takes no arguments no longer opens an empty modal
* Improved stability of Project Backup
* In Layouts filtering and select all only select filtered devices
* Portrait layouts show Landscape above Zone Arrangement


## Drivers
* Broken drivers removed from Creator
* Meta drivers now only show commands with populated codes
* Update DSP.ONE driver to interface w/ the Creator UI
* Stream.one driver now updates stream url when unit is running old firmware
* Added generic http driver with a \`getURL\` command to perform http get operations
* Fixed issues with "RTSP Port" field
* Verify that FW 4.11.00 is working with SAVI
* webOS 4.x\+ now includes Tile Mode settings in Creator
* Sony VPL-PHZ60 \(IP\)
* Added AppleTV IR driver
* Stream.one DetectedDevice record now has correct driverOptions
* LG canvas devices now defaults Streaming Latency to 700ms
* All televisions now have a default source property
* Added source selection and volume control to Bosch Dynacord MXE5
* Added support for Atlas IED AZM4/8 \(IP\)
* Now supports updating the RTSP multicast port setting on Stream.one devices
* Added Support for the QSC Snapshot Selector
* Increased number of streams in SAVI DSP/DMA driver
* RGB Galileo Layout now includes a "Surface" argument on the setLayout and setLayoutManual commands
* Renamed "Generic Telnet Device" to "Generic TCP Device"
* Added Generic UDP Device
* Galileo Layout Driver supports "surfaces"
* Added Atlona AT-HDR-H2H-88MA HDMI Matrix
* Added "Resync Frequency" property to webOS devices
* QSC Media Receiver now allows RTP and RTSP URLs
* Stream.One settings are now only sent to the device when they need to change
* Increase Q-Sys Router driver inputs and outputs to 64
* Zektor driver now sends audio config on every reconnect
* Added support for AVPro AC-MXNET-CBOX Switch
* Updated Rockbot driver to support UI features
* Fixed Back, Cancel and Set Input buttons for Sony Simple IP
* Connect.One contact closure no longer sends erroneous state event change at startup
* SAVI Triad no longer stops communicating when connectivity is lost
* Fixed issues found when the DSP.One driver has to reconnect to a device
* COM51 2-way feedback no longer errors with "axios.create is not a constructor"
* Canvas line input regions now properly scale for UH5L
* Fixed memory leak related to COM51 Tuner 2-way feedback
* Fixed issues with RGB Galileo Layout's "Surface" property
* AZM4/8 driver now waits longer before reconnecting & uses correct port counts
* Previous Channel Button For DirectTV Driver is now operational
* play command is now available to ir/rs232 tv drivers

## DevOps
* Cherrypick new DSP driver into 3.2.0-beta5
* Now building squashfs release
* Pin all UI dependencies
* root should have same bash aliases as savi
* Start saving squashfs build to nas/aws
* Fixed webOS cli mode issue
* Add non-standard service for aes70-daemon
* Backport SN-2597 \(static networking fix\) to 3.1.2
* Build out AES70 service
* Version generation now support release candidates
* Removed usb-qe and gs-api code
* Removed test-project-gene package
* Port mac address portion of SN-2750 to 3.2.0
* Existing migrations no longer fail when reapplied
* Migrations are more robust when run against an existing database
* Removed the facilityV2 and show feature flag from the database
* User Access Denied page should be removed

## Facility View
* App no longer contains import license code
* Filters Pane now intersects selection across filter groups
* Volume bars on television endpoints are now operational
* Login pages no longer cause a redirect loop
* Fixed an issue with executing macros
* Added ability to edit colors on mobile
* Added ability to edit colors on desktop/tablet
* Volume Bars on Displays are now visible when enabled  
* getVariable function now accepts a default parameter
* Macros buttons now give visual feedback when clicked
* Endpoint buttons that are playing Show media now display Show metadata
* Fixed an issue where mobile would occasionally display a white screen
* SAVI 3 is now the default facility view
* Added support for Apple TV Control UI
* Empty Filters / Filter Groups are no longer displayed
* Horizontal scroll bar is now in the correct position on mobile
* Canvas Layout dropdown now collapses when clicking on the right-side arrow
* Fonts now render properly when browsing device does not have internet access
* Fixed missing toolbar icons
* Improved placement of "Source search" edit field
* Layout names in sidebar and Endpoint card now correctly support word wrapping
* Adding to home page on mobile now displays the correct icon
* Added support to change layouts on televisions connected to webOS tuners
* Switch Scenes modal no longer cuts off some scenes
* Fixed issue with Macro button name length
* Moved Device Control X/Dismiss button to top right of remote modal
* Control UI no longer hangs when Stream.one Preview IP is unavailable
* Source selector region now wraps text properly
* Channel ID text is no longer cut off
* Remote modal now correctly closes when clicking outside of the modal
* Volume Preset Editor now sets volume
* Selecting a Macro and then "All" Audio Zones no longer crashes the app
* Endpoint now correctly updates when changing audio zone sources
* Guest account access now works properly
* Reconnect now retries forever instead of giving up after 1 attempt
* Changes made in Scene Editor are now visible in Facility without a refresh
* Added Margin for Last Volume Preset
* Added Volume Presets
* Show images now correctly update on Canvas displays
* Now honors the Hidden Sources flag
* Audio Zone endpoint no longer has "0" when volume level is zero
* Realtime data updates continue to function after Endpoints are filtered out
* Clicking on the icon of a layout in the layout dropdown no longer causes an error
* Source pane no longer shows audio/video items when only LEDs or macros are selected
* Source pane now correctly raises/lowers on mobile
* Volume Presets no longer show incorrect values
* Removed the All | None selection filters next to Thermostat section 
* Now able to select Macro endpoints
* Fixed an issue with too much header on login page 
* Off/On commands now function properly
* Presets only select from filtered endpoints
* Fixed issue with SAVI login and the Chrome Extension Lastpass
* Improved handling of slow network startup
* Navigating to SAVI URL no longer causes a redirect loop
* Fixed some issues with editing user information

## Floor Plan
* Now properly enforcing maximum resolution/size limitations
* Fixed issue with multi-select Endpoints
* Cleared Unsaved Changes message after deleting location and saving
* Endpoint details now always visible
* Deleting a device that exists in a floor plan no longer breaks the floor plan


## Map View
* Changing layout is now reflected in the UI without a manual refresh* SN-2480 Creator v2: Changes are no longer automatically pushed to 10.7.10.149
* Added new feature for Nano-sized Endpoints
* Repositioned "Select Visible" button
* Filters now contain icons
* Macros can now be de-selected
* Tiny endpoints are now multiselectable

## Room View
* Now locked behind a feature flag

## SAVI Show
* Images now automatically fit to the screen
* Managing show assets is only available to Admin and Manager user roles
* duplicate key error when adding a new Category now displays a notification
* Slideshows now work with SAVI Show
* "Other" filter excludes all appropriate images
* Navigating to SAVI Show no longer locks user out if not logged into Facility
* Slideshow images now play in the correct order
* Editing playlists automatically pushes change to displays

## Scene Editor
* Fixed an issue with ordered Presets moving below intended location
* Remove Presets / Remove Sections buttons on mobile now working correctly 
* Filter Name now populating after selecting
* Now able to launch scene that was just edited

## Scheduler
* Feature flag has been removed
* Search Bar and magnifying glass icon are now aligned
* Added ability to return to Facility 3 from Hamburger Menu
* Reconnecting popup is no longer behind modals
* Program Guide Sources now listed in the same order as source tree
* Fixed an issue where scheduler occasionally restarted with out of heap errors
* SN-2354 - Guide v2: Fixed some issues where text was too big for buttons
* SN-2473 - Guide Data: Service now resets itself on a communication failure
