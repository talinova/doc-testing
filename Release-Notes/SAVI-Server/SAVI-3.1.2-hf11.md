---
title: "Release notes - SAVI - Version 3.1.2-hf11"
tags: release, notes, 3.1.2, hf11, internal
date:
  created: "12/20/2022"
  modified: "01/25/2023"
description: Oct 2022
---

# Release notes - SAVI - Version 3.1.2-hf11

# Internal
## DevOps
* Build out AES70 service
* aes70 daemon no longer requires ports
* Add script to report canvas displays temperature

## Canvas
* Network instability now causes fewer problems with initial handshake
* Restoring project with screenshots no longer breaks dashboard

## Creator
* Fixed issue with syncing Primary SAVI Server to Secondary SAVI Server

## Drivers
* Added support for BSS London BLU-800
* Added source selection and volume control to Bosch Dynacord MXE5
* Zektor driver now sends audio config on every reconnect
* Rename Zektor to Pulse-Eight and added setEQ command
* Generic Telnet Device now supports hex codes in the sendCommand argument
* COM51 Tuner no longer sends config at process startup

## Facility View
* Fixed issue with SAVI login and the Chrome Extension Lastpass
