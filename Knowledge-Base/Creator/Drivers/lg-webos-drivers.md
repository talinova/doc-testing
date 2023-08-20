---
title: "LG WebOS Display Drivers"
tags: creator, driver, equipment, lg, webos
date:
  created: "03/25/2022"
  modified: "12/12/2022"
description: Resource for the LG WebOS Display Drivers.
---
<div style="text-align: center">

<a href="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/lg-logo.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/lg-logo.png" alt="LG Logo" width="700" height="">
</a>
</div>

# LG WebOS Display Drivers

The named LG Display drivers ([SM5KC](https://www.lg.com/global/business/digital-signage/lg-55SM5KC), [SM5KD](https://www.lg.com/global/business/digital-signage/lg-55SM5KD), [SM5KE](https://www.lg.com/global/business/digital-signage/lg-55sm5ke-b), and [UL3G](https://www.lg.com/global/business/digital-signage/lg-43ul3g-b)) allow control of those specific displays. However the LG webOS Display driver serves as a generic driver for all SAVI Canvas compatible LG webOS displays. As these drivers all share configurations, only the LG webOS Display driver is detailed below. Connections may vary based on device.

>***Note: Layouts with multiple regions on these devices only support one line input (hardwired connection). Additional line inputs will display as blank sections.***

#### General Properties
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/lg-webos-display-general-01.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/lg-webos-display-general-01.png" alt="LG WebOS Display configuration general 01" width="300" height="">
</a>
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/lg-webos-display-general-02.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/lg-webos-display-general-02.png" alt="LG WebOS Display configuration general 02" width="300" height="">
</a>

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **Hidden Sources:** Sources that are not shown when viewing the source select in Facility View for this display.

* **Default Layout:** Canvas layout that is auto selected when playing a source.

* **Available Layouts:** Canvas layouts available to be viewed on the display and selectable from the layout selector in Facility View. This can be edited here or in the Layout Editor.

* **Power Off After 15 Min of 'No Signal':** If True, this display will automatically power down after 15 mins of not getting a signal. This is unchecked by default as enabling it is not recommended with SAVI.

* **Power On Status:** When this display (re)connects to SAVI, its power on status is changed to this value.

* **Rotation:** The orientation of the display. 0 is default, with the display mounted horizontal. 90 and 270 are used when the display is mounted vertically (rotated either right or left). 180 is used when mounting the display horizontally upside-down (not recommended as most mounts are not designed for this).

* **Startup Audio Mode:** When this display (re)connects to SAVI, its audio mode is changed to this value.

* **Startup Volume:** When this display (re)connects to SAVI, its volume level is changed to this value.

* **Startup Picture Mode:** When this display (re)connects to SAVI, its picture mode is changed to this value

* **Startup Power Management Mode:** When this display (re)connects to SAVI, its power management mode is changed to this value.

* **USB Lock:** Enabling this will disable file reading from the USB port on the display but will still allow input from peripheral devices, like keyboards and mice.

* **IR Mode:** Setting this to Normal allows IR input as usual, Use Power Only will only allow IR input to power the display on/off, and Block All prevents all IR input at the display (however this will still allow IR control if IR Remote Map is enabled).

* **Button Mode:** Like IR Mode, setting this to Normal allows button presses on the display as per usual, Use Power Only will only allow button input to power the display on/off, and Block All disables all buttons on the display.

* **Streaming Latency:** The delay (in ms) injected into the streaming pipeline to keep playback smooth. Range of 400 to 10000. Use -1 to keep the manufacturer's default. Default value is 700.

>***Note: Streaming Latency values below 400 are not recommended.***


#### Advanced Properties
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/lg-webos-display-advanced-01.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/lg-webos-display-advanced-01.png" alt="LG WebOS Display configuration advanced 01" width="300" height="">
</a>
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/lg-webos-display-advanced-02.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/lg-webos-display-advanced-02.png" alt="LG WebOS Display configuration advanced 02" width="300" height="">
</a>
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/lg-webos-display-advanced-03.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/lg-webos-display-advanced-03.png" alt="LG WebOS Display configuration advanced 03" width="300" height="">
</a>

* **Tile Mode (SM5KE, UL3G, \& webOS Only):** Determines how tile mode is treated by SAVI.
    * **Do Not Change:** This setting will leave Tile Mode settings alone and allow switching between modes.
    * **Yes:** This setting will enable Tile Mode.
    * **No:** This setting will disable Tile Mode completely.

* **Tile Mode Row:** Sets the number of rows in the tile configuration. Set to 1 by default. Range is 1-15.

* **Tile Mode Column:** Sets the number of columns in the tile configuration. Set to 1 by default. Range is 1-15.

* **Tile Mode Tile Id:** Sets which display this is in the grid (starts at 1 in the top left, increasing by 1 from left to right and continuing on the left of the next row underneath). Set to 1 by default. Range is 1-255.

<a href="../../../Assets/Knowledge-Base/Creator/Drivers/lg-tile-mode.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/lg-tile-mode.png" alt="LG WebOS Display tile mode example" width="300" height="">
</a>

* **Tile Mode Natural Mode:** Enabling this will partly omit the edges of the image displayed to compensate for distance between displays.

<br>

* **IR Remote Map: Video:** The way in which IR remotes control video in SAVI. Disabled prevents remote control, Gestures allows control of layouts and sources with a standard LG remote (Left and Right arrows toggle through sources, Up and Down arrows toggle through layouts), Control Source allows control of the connected source (if that source is controllable).

* **IR Remote Map: Audio:** The way in which IR remotes control audio in SAVI. Disabled prevents remote control. Allows the LG remote's volume buttons to control the display's volume (if "Control Display" is selected) or a connected SAVI Audio Zone (if "Control Audio Zone" is selected)

* **Audio Zone for IR Remote Map:** The audio zone to control when IR Remote Map: Audio is set to 'Control Audio Zone.'

* **Display Specific Region (1-4) Type:** Set the type of input so Creator knows whether to look at the URL field or Line In Input field.

* **Display Specific Region (1-4) URL:** For any type of URL (Video, Image, VNC). Ignored when Region Type is Line In.

* **Display Specific Region (1-4) Line In Input:** Which physical input to use for each region. Ignored when Region Type is not Line In.

* **Startup TruMotion:** Used to convert lower framerates up to 60 fps.
    * **Do Not Change:** Will use SAVI defaults (recommended).
    * **Disable:** Will disable framerate adjustments and match source framerate.

* **Startup Real Cinema:** Used to convert lower refresh rates up to 120 Hz.
    * **Do Not Change:** Will use SAVI defaults (recommended).
    * **Enable:** Will convert lower refresh rates up to 120 Hz.
    * **Disable:** Will disable refresh rate adjustments and match source refresh rate.

### Connections
Each of the LG WebOS Display drivers has both HDMI and DVI connections. Some of the device specific drivers have additional input connections which are labeled as such below.

##### Input
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/lg-webos-display-connections-input.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/lg-webos-display-connections-input.png" alt="LG webOS input connections" width="300" height="">
</a>
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/lg-sm5kc-display-connections-input.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/lg-sm5kc-display-connections-input.png" alt="LG SM5KC input connections" width="300" height="">
</a>
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/lg-sm5kd-display-connections-input.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/lg-sm5kd-display-connections-input.png" alt="LG SM5KD input connections" width="300" height="">
</a>
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/lg-sm5ke-display-connections-input.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/lg-sm5ke-display-connections-input.png" alt="LG SM5KE input connections" width="300" height="">
</a>
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/lg-ul3g-display-connections-input.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/lg-ul3g-display-connections-input.png" alt="LG webOS input connections" width="300" height="">
</a>


* **HDMI:** Connects to any available HDMI output.

* **DVI:** Connects to any available DVI output.

* **Display Port (SM5KE, SM5KD, \& SM5KC Only):** Connects to any available DP output.

* **RGB (SM5KC \& SM5KD Only):** Connects to any available RGB/VGA output.
