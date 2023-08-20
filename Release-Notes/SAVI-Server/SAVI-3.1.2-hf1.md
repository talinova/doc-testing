---
title: "Release notes - SAVI - Version 3.1.2-hf1"
tags: release, notes, 3.1.2, hf1, internal
date:
  created: "04/28/2022"
  modified: "01/25/2023"
description: April 2022
---

# Release notes - SAVI - Version 3.1.2-hf1


# Internal
## Creator
* Command router service no longer hangs when a connection loop exists

## Drivers
* C4 drivers are now hidden behind feature flag
* QSC Level now more accurately converts percent gain to dB
* Improved streaming media playback on webOS displays
  * UL3J now plays Pro:Idiom streams. For now only landscape orientation is supported due to LG firmware issue
  * Improved SAVI’s ability to detect a freeze in the streaming media playback on all webOS displays. SAVI restarts the video playback when a freeze is detected.
* C$ drivers are now hidden behind feature flag