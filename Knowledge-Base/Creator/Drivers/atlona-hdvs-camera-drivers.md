---
title: "Atlona Camera Drivers"
tags: creator, driver, equipment, atlona, camera, hdvs
date:
  created: "03/25/2022"
  modified: "08/09/2022"
description: IP and Serial (RS232) drivers for the Atlona HDVS PTZ Camera.
---
<div style="text-align: center">

<a href="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/atlona-logo.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/atlona-logo.png" alt="Atlona Logo" width="700" height="" class="center">
</a>
</div>

# Atlona Camera Drivers
These drivers interface with the [Atlona HDVS Camera](https://atlona.com/product/hdvs-cam/ "Atlona HDVS Camera") through either IP or Serial connection. Specifications on the camera itself can be found on the Atlona site.

## HDVS Camera (IP)

#### Properties
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/atlona-hdvs-camera-ip.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/atlona-hdvs-camera-ip.png" alt="Atlona HDVS Camera IP" width="300" height="">
</a>

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **Image Preview URL:** A link used to preview a streaming video source. If the driver is connected to a Stream.One, this field will auto-populate. This provides the appropriate URL to SAVI Preview in Facility View. Allowable: single image preview or Motion JPEG.

* **Image Preview Refresh Interval:** Determines how often the preview image should be refreshed. Specifies Refresh Interval in Milliseconds (default is 67 which is equal to 15 frames per second).

* **IP Address:** The destination IP address that SAVI will use when communicating with the device.

* **Port:** The IP address port that the device is open to. Set to 1259 by default.

* **Pan Speed:** Speed the camera will pan (left and right) at 1 (low) - 24 (high). Set to 7 by default.

* **Tilt Speed:** Speed the camera will tilt (up and down) at 1 (low) - 20 (high). Set to 7 by default.

* **Zoom Speed:** Speed the camera will zoom at 0 (low) - 16 (high). Set to 1 by default.
* **Focus Speed:** Speed the camera will focus at 0 (low) - 16 (high). Set to 1 by default.

### Connections

##### Output
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/atlona-hdvs-camera-serial-connections-output.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/atlona-hdvs-camera-serial-connections-output.png" alt="Atlona HDVS Camera IP - output connections" width="300" height="">
</a>

* **HDMI Out:** Corresponds to the HDMI output on the back of the camera.

----

## HDVS Camera (Serial)

#### Properties
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/atlona-hdvs-camera-serial.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/atlona-hdvs-camera-serial.png" alt="Atlona HDVS Camera Serial" width="300" height="">
</a>

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **Image Preview URL:** A link used to preview a streaming video source. If the driver is connected to a Stream.One, this field will auto-populate. This provides the appropriate URL to SAVI Preview in Facility View. Allowable: single image preview or Motion JPEG.

* **Image Preview Refresh Interval:** Determines  how often the preview image should be refreshed. Specifies Refresh Interval in Milliseconds (default is 67 which is equal to 15 frames per second).

* **Baud Rate:** Set to 9600 by default.

* **Flow Control:** Sets the serial port handshake type.
  * **None** - Turned off.
  * **Hardware** - Hardware flow control.
  * **XON/XOFF** - Software flow control.
  * **Unknown** - Flow control is unknown.

* **Parity:** Sets the serial port parity type for error detecting.
  * **None** - Turned off.
  * **Even** - Even parity bit.
  * **Odd** - Odd parity bit.
  * **Unknown** - Parity is unknown.

* **Data Bits:** Set to 8.

* **Stop Bits:** Set to either 1 or 2.

* **Pan Speed:** Speed the camera will pan (left and right) at 1 (low) - 24 (high). Set to 7 by default.

* **Tilt Speed:** Speed the camera will tilt (up and down) at 1 (low) - 20 (high). Set to 7 by default.

* **Zoom Speed:** Speed the camera will zoom at 0 (low) - 16 (high). Set to 1 by default.

* **Focus Speed:** Speed the camera will focus at 0 (low) - 16 (high). Set to 1 by default.

### Connections

##### Input
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/atlona-hdvs-camera-serial-connections-input.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/atlona-hdvs-camera-serial-connections-input.png" alt="Atlona HDVS Camera Serial - input connections" width="300" height="">
</a>

* **RS232 In:** Serial input for control.

##### Output
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/atlona-hdvs-camera-serial-connections-output.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/atlona-hdvs-camera-serial-connections-output.png" alt="Atlona HDVS Camera Serial - output connections" width="300" height="">
</a>

* **HDMI Output:** Corresponds to the HDMI output on the back of the camera.
