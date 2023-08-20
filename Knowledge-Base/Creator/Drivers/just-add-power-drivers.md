---
title: "Just Add Power Drivers"
tags: creator, driver, equipment, just-add-power, tiler
date:
  created: "03/25/2022"
  modified: "12/12/2022"
description: Resource for the Just Add Power drivers.
---
<div style="text-align: center">

<a href="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/just-add-power-logo.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/Logos/just-add-power-logo.png" alt="Just Add Power Logo" width="" height="">
</a>
</div>

# Just Add Power Drivers
These drivers work together or independently to control [transmitters and receivers](http://justaddpower.com/product-range.html).

## Receiver Driver
Each display should have one of these Receiver drivers to control the device.

#### Properties
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/just-add-power-receiver.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/just-add-power-receiver.png" alt="SAVI Creator Just Add Power Receiver" width="300" height="">
</a>

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **Hidden Sources:** Sources that should not be shown when selecting sources for this device.
* **IP Address:** The destination IP address that SAVI will use when communicating with the device.
* **Rotation:** The orientation of the display. 0 is default, with the display mounted horizontal. 90 and 270 are used when the display is mounted vertically (rotated either right or left). 180 is used when mounting the display horizontally upside-down (not recommended as most mounts are not designed for this).

#### Connections

##### Input
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/just-add-power-receiver-connections-input.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/just-add-power-receiver-connections-input.png" alt="SAVI Creator Just Add Power Receiver - connections - input" width="300" height="">
</a>

* **RJ 45:** Ethernet source.

-----
Will need to use either a cisco or luxul switch.

## Switch Cisco Driver
Needed to control receivers.

#### Properties
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/just-add-power-switch-cisco.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/just-add-power-switch-cisco.png" alt="SAVI Creator Just Add Power Switch Cisco" width="300" height="">
</a>

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **IP Address:** The destination IP address that SAVI will use when communicating with the device.

* **Username:** Login username of the device.

* **Password:** Login password of the device.

#### Connections

##### Input
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/just-add-power-switch-cisco-connections-input.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/just-add-power-switch-cisco-connections-input.png" alt="SAVI Creator Just Add Power Switch Cisco - connections - input" width="300" height="">
</a>

* **Input Port (001-072):** Up to seventy-two sources.

##### Output
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/just-add-power-switch-cisco-connections-output.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/just-add-power-switch-cisco-connections-output.png" alt="SAVI Creator Just Add Power Switch Cisco - connections - output" width="300" height="">
</a>

* **Output Port (001-072):** Up to seventy-two outputs.



## Switch Luxul Driver
#### Properties
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/just-add-power-switch-luxul.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/just-add-power-switch-luxul.png" alt="SAVI Creator Just Add Power Switch Luxul" width="300" height="">
</a>

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **IP Address:** The destination IP address that SAVI will use when communicating with the device.

* **Username:** Login username of the device.

* **Password:** Login password of the device.

* **Number of transmitters:** Set to 1 by default.

* **Number of receivers:** Set to 1 by default.

#### Connections

##### Input
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/just-add-power-switch-luxul-connections-input.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/just-add-power-switch-luxul-connections-input.png" alt="SAVI Creator Just Add Power Switch Luxul - connections - input" width="300" height="">
</a>

* **Input Port (001-048):** Up to forty-eight sources.

##### Output
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/just-add-power-switch-luxul-connections-output.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/just-add-power-switch-luxul-connections-output.png" alt="SAVI Creator Just Add Power Switch Luxul - connections - output" width="300" height="">
</a>

* **Output Port (001-048):** Up to forty-eight outputs.

----
Requires all 3 wall drivers 

## Wall Driver
Adding this will enable a wall scene in Facility View.

#### Properties
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/just-add-power-wall.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/just-add-power-wall.png" alt="SAVI Creator Just Add Power Wall" width="300" height="">
</a>


* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **Columns:** How many displays the videowall is across.

* **Rows:** How many displays the videowall is from top to bottom.

* **Layouts:** Select the "Just Add Power Wall Layout."

* **Hide Zone Names:** If true, the zone names are hidden in the video wall scene.

* **Receiver (01-32):** Up to thirty-two receiver connections.

#### Connections

##### Output
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/just-add-power-wall-connections-output.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/just-add-power-wall-connections-output.png" alt="SAVI Creator Just Add Power Wall - connections - output" width="300" height="">
</a>

* **Virtual Output (01-32):** Up to thirty-two outputs via network connection.




## Wall Layout Driver
Configures the videowall layout.

#### Properties
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/just-add-power-wall-layout.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/just-add-power-wall-layout.png" alt="Just Add Power Wall Layout" width="300" height="">
</a>


* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **Zone (01-32) Enabled:** If true, this zone is included in the layout.

* **Zone (01-32) X:** Starting column for this zone.

* **Zone (01-32) Y:** Starting row for this zone.

* **Zone (01-32) Width:** Width (in columns) for this zone.

* **Zone (01-32) Height:** Height (in columns) for this zone.

* **Zone (01-32) Rotation:** The orientation of the display. 0 is default, with the display mounted horizontal. 180 is used when mounting the display horizontally upside-down (not recommended as most mounts are not designed for this).



## Wall Zone Driver
Each zone is a region in the wall layout.

#### Properties
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/just-add-power-wall-zone.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/just-add-power-wall-zone.png" alt="Just Add Power Wall Zone" width="300" height="">
</a>

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **Hidden Sources:** Sources that should not be shown when selecting sources for this device.

#### Connections

##### Input
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/just-add-power-wall-zone-connections-input.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/just-add-power-wall-zone-connections-input.png" alt="SAVI Creator Just Add Power Wall - connections - input" width="300" height="">
</a>

* **Input:** Source input.


<!---

------------



## Tiler Driver
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/just-add-power-tiler.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/just-add-power-tiler.png" alt="SAVI Creator Just Add Power Tiler configuration" width="300" height="">
</a>

Previously a Source driver, this device adds video tiling to Ultra HDMI over IP matrix switches. multiple sources on one display.

#### Properties

* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="../../../Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **IP Address:** The destination IP address that SAVI will use when communicating with the device.

* **Image Preview Refresh Interval:** This will set how often Creator should refresh (reload) the Preview Image. By default this is set to 67ms.

### Connections

##### Input
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/just-add-power-tiler-connections-input.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/just-add-power-tiler-connections-input.png" alt="SAVI Creator Just Add Power Tiler input connections" width="300" height="">
</a>

* **RX 1 RJ45:** Ethernet receiver for first stream.

* **RX 2 RJ45:** Ethernet receiver for second stream.

* **RX 3 RJ45:** Ethernet receiver for third stream.

* **RX 4 RJ45:** Ethernet receiver for fourth stream.

##### Output
<a href="../../../Assets/Knowledge-Base/Creator/Drivers/just-add-power-tiler-connections-output.png">
  <img src="../../../Assets/Knowledge-Base/Creator/Drivers/just-add-power-tiler-connections-output.png" alt="SAVI Creator Just Add Power Tiler output connections" width="300" height="">
</a>

* **HDMI Out:** Audio/video output with combined inputs.

* **TX RJ 45:** Ethernet transmitter for combined stream.

--->