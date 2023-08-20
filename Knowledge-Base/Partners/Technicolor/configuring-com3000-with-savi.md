---
title: "Configuring COM3000 With SAVI"
tags: partner, com3000, technicolor, com400, com51
date:
  created: "03/21/2022"
  modified: "09/13/2022"
description: A step-by-step guide on configuring a new COM3000 system to work with SAVI. Covers COM400 setup, COM51 setup, and SAVI Creator driver setup.
---

# Configuring COM3000 With SAVI
<a href="../../../Assets/Knowledge-Base/Partners/Technicolor/com3000-chassis.png">
  <img src="../../../Assets/Knowledge-Base/Partners/Technicolor/com3000-chassis.png" alt="COM3000 Chassis" width="700" height="">
</a>

This details the configuration of the Technicolor COM3000 system to work with SAVI. For more detailed information about the COM3000, visit the [Technicolor website](https://www.technicolor.com/distribute/home-experience/play/com3000-solution "Technicolor website").

## COM400
Your first step is to connect the chassis to your network. You need at least a 1 Gbit network connection via Ethernet to one of the 10 Gbit ports for the multicast streams. It is also recommended you have a separate connection to one of the 1 Gbit ports on the chassis. This allows using two VLANs which lets you keep the default static IP unchanged.

### Initial Login To The COM400
<a href="../../../Assets/Knowledge-Base/Partners/Technicolor/com400-login.png">
  <img src="../../../Assets/Knowledge-Base/Partners/Technicolor/com400-login.png" alt="COM400 login window" width="300" height="">
</a>

Before you setup the individual cards in the COM3000 system, you need to configure the COM400 chassis. The chassis has a dedicated static IP out of the box that can be used for initial setup. Enter the IP into your browser's address bar to reach the log-in screen.
>COM 400 Default Static IP: `192.168.10.2`

The last octet of this IP is determined by the chassis ID + 1. If this is your first and only chassis, it is 2.
On first login, you are greeted with the login window (left).

The default credentials are:
>Username: `admin`
>Leave the Password field blank

This guide assumes that you are not changing the COM400 password. If you change the password, ensure you note it for future use. Forgetting the login information may require a full system reset.

### COM400 IP Configuration
The next thing you need to setup is the IP address for the COM400.
<a href="../../../Assets/Knowledge-Base/Partners/Technicolor/com400-ip-config.png">
  <img src="../../../Assets/Knowledge-Base/Partners/Technicolor/com400-ip-config.png" alt="COM400 IP config" width="700" height="">
</a>

1. Navigate to **Configuration > System > IP**
2. Click **Add Interface**
3. Number the **VLAN** (we recommend 2)
4. Enter the desired IP **Address** for the COM400 chassis
5. Enter the desired **Mask Length**
    >* This determines the amount of IPs available on the Subnet Mask
    >* We recommend 23 or 24 depending on your network size
    >24 = 254 addresses available, Subnet starts at `255.255.255.0`
    >23 = 510 addresses available, Subnet starts at `255.255.254.0`
    >16 = 65,534 addresses available, Subnet starts at `255.255.0.0`

6. Click **Save**

Further information can be found in the COM3000 Integrator's Manual on page 37.

### COM400 Global VLAN Configuration
Now you need to set your new VLAN IP as active on one of the 10 Gbit ports.
<a href="../../../Assets/Knowledge-Base/Partners/Technicolor/com400-global-vlan-config.png">
  <img src="../../../Assets/Knowledge-Base/Partners/Technicolor/com400-global-vlan-config.png" alt="COM400 Global VLAN config" width="700" height="">
</a>

1. Navigate to **Configuration > VLANs > Configuration**
2. Reference the chart to determine what each port Corresponds to
3. Change Port 10 and any COM51 slots you wish to use with SAVI to the following configuration:
    >* **Mode:** Hybrid
    >* **Port VLAN:** 2 (from step 3 in "**COM400 IP Configuration**")
    >* **Port Type:** C-Port
    >* **Egress Tagging:** Untag Port VLAN
    >* **Allowed VLANs:** 1-4095
    >* leave all other fields as default

4. Click **Save**

>***Warning: You will lose connection to the UI if you only have a connection to the network through the COM400 10 Gbit port and not through a 1 Gbit port as well.***

|  **Port #**  |  **COM400 Connection**  |
| :------------ | :------------ |
|  1  |  COM51 slot 6  |
|  2  |  COM51 slot 5  |
|  3  |  COM51 slot 4  |
|  4  |  COM51 slot 3  |
|  5  |  COM51 slot 2  |
|  6  |  COM51 slot 1  |
|  7  |  QAM Port 2 (TOP)  |
|  8  |  QAM Port 1 (BOTTOM)  |
|  9  |  Unmanaged Ethernet switch to both 1 GIG ports  |
|  10  |  Top 10 GIG  |
|  11  |  Bottom 10 GIG  |

Additional information can be found in the COM3000 Integrator's Manual on page 38.

### COM400 IGMP Snooping Configuration
Once you reconnect to the COM400 chassis, configure your IGMP settings. IGMP settings can be found on page 35 of the COM3000 Integrator's Manual.
<a href="../../../Assets/Knowledge-Base/Partners/Technicolor/com400-igmp-snooping-config.png">
  <img src="../../../Assets/Knowledge-Base/Partners/Technicolor/com400-igmp-snooping-config.png" alt="COM400 IGMP Snooping Config" width="" height="">
</a>
<a href="../../../Assets/Knowledge-Base/Partners/Technicolor/com400-igmp-snooping-vlan-config.png">
  <img src="../../../Assets/Knowledge-Base/Partners/Technicolor/com400-igmp-snooping-vlan-config.png" alt="COM400 IGMP Snooping VLAN Config" width="" height="">
</a>

1. Navigate to **Configuration > IPMC > IGMP Snooping > Basic Configuration**
2. Ensure the Global Configuration is as follows:
    >* **Snooping Enabled:** `Checked`
    >* **Unregistered IPMCv4 Flooding Enabled:** `Unchecked`

3. Ensure the Port Related Configuration has only the **10** and **11** **Router Ports** checked
    >* leave all other fields unchecked

4. Click **Save**
5. Navigate to **Configuration > IPMC > IGMP Snooping > VLAN Configuration**
6. Ensure the IGMP Snooping VLAN Configuration is as follows for both VLAN IDs:
    >* **Snooping Enabled:** `Checked`
    >* **Querier Election:** `Unchecked`
    >* **Querier Address:** `2.2.2.2`

7. Click **Save**


### COM400 Save Startup Configuration
Finally, you need to save all of these configurations to the startup-config. This allows the COM400 to reapply these settings after a power cycle, otherwise the default settings override these settings.
<a href="../../../Assets/Knowledge-Base/Partners/Technicolor/com400-maint-menu.png">
  <img src="../../../Assets/Knowledge-Base/Partners/Technicolor/com400-maint-menu.png" alt="COM400 Maintenance menu" width="" height="">
</a>
<a href="../../../Assets/Knowledge-Base/Partners/Technicolor/com400-save-running-config.png">
  <img src="../../../Assets/Knowledge-Base/Partners/Technicolor/com400-save-running-config.png" alt="COM400 Startup config save" width="700" height="">
</a>

1. Navigate to **Maintenance > Configuration > Save startup-config**
2. Click **Save Configuration**

See page 39 of the COM3000 Integrator's Manual for further information.


------------

## COM51

### COM51 Slot Base IP
Now that the COM400 chassis is configured, you need to setup the individual tuner cards. This requires either a direct connection into one of the 10 Gbit Ethernet ports on the COM3000 or a direct connection to a switch connected to one of those ports. You also need to change the computer you are using to a static IP address.

1. Open the network settings on your computer (this varies based on your Operating System)
2. Change configuration to the following:
    >* **IP address:** `192.168.3.100`
    >* **Subnet mask:** `255.255.255.0` (this should match your settings in step 5 of "**COM400 IP Configuration**")

3. Browse to the default COM51 IP address:
    > COM51 Default Static IP: `192.168.3.18`

4. If the user interface requires a password, use the default unless you have changed it previously
    > COM51 Default Password: `com3k`

<a href="../../../Assets/Knowledge-Base/Partners/Technicolor/com51-overview.png">
  <img src="../../../Assets/Knowledge-Base/Partners/Technicolor/com51-overview.png" alt="COM51 Overview" width="700" height="">
</a>

5. Click **Overview** to ensure the page is fully loaded
    >* Before proceeding, you may wish to ensure your installed COM51s have your correct licensing. This process can be found on page 42 of the COM3000 Integrator's Manual.

6. Select the first Tuner number in the last Slot in the Chassis
7. Scroll down to User Config

>***Note: The slot number may be clicked to minimize those tuner fields***

<a href="../../../Assets/Knowledge-Base/Partners/Technicolor/com51-user-config.png">
  <img src="../../../Assets/Knowledge-Base/Partners/Technicolor/com51-user-config.png" alt="COM51 User config" width="700" height="">
</a>

8. Configure as follows:
    >* **IP_Config:** `4 = Fixed`
    >* **Base_IP:** Set to your desired IP address for the tuner, such as `10.7.11.18` (the first three octets should match the chassis VLAN)
    >* **Subnet:** This should match your settings in step 5 of "**COM400 Slot Base IP**"
    >* **Gateway:** The IP of your router or gateway
    >* **DNS_IP:** Your Domain Name Server. You can use `8.8.8.8` or `8.8.4.4` if you do not have a DNS
    >***Ensure each Base_IP is unique***

9. Click **Submit**

You may need to reboot the card, if so scroll down to **Reset** and click **Submit**

<a href="../../../Assets/Knowledge-Base/Partners/Technicolor/com51-reset.png">
  <img src="../../../Assets/Knowledge-Base/Partners/Technicolor/com51-reset.png" alt="COM51 reset" width="" height="">
</a>

From here you should continue to work backwards through the chassis, configuring the User Config under **Tuner 1** for each of the Slots.
>***Ensure each Base_IP is unique.***

### COM51 Tuner IP
The final step to configuring the COM51 cards are establishing the Tuner IPs themselves. These are the multicast streaming IPs available to SAVI.

1. Navigate back to **Overview**
2. Select the first Tuner
<a href="../../../Assets/Knowledge-Base/Partners/Technicolor/com51-channel-tune-config.png">
  <img src="../../../Assets/Knowledge-Base/Partners/Technicolor/com51-channel-tune-config.png" alt="COM51 Channel Tune config" width="" height="">
</a>

3. Configure the Channel Tune section as follows:
    >* **Dest_IP_Address:** `224.2.2.1` (these should increase incrementally, i.e., `224.2.2.2`, `224.2.2.3`, etc.)
    >* **Dest_Port_Number:** `1000`
    >* **Protocol_Type:** `0 = UDP`
    >* **Security_Mode:** `0 = None` (removes stream encryption), `1 = Pro_Idiom` (channels remain encrypted with Pro-Idiom), other options are discussed on page 46 of the COM3000 Integrators Manual
    >* **Persistent:** `1 = TRUE`
    >Leave all other fields alone

4. Click **Submit**



------------

## Creator Drivers
The final configuration process is setting up SAVI Creator drivers so that each tuner displays as a source in SAVI Facility View. You need to be connected to the same network as your SAVI Server Pro (which should be accessible to the COM3000). For further information on SAVI Creator, check out its User Guide under Documents on the dealer portal or its section in the [Knowledge Base](/Knowledge-Base/Creator/creator-getting-started.md "Knowledge Base").
<a href="../../../Assets/Knowledge-Base/Partners/Technicolor/com51-tuner-driver.png">
  <img src="../../../Assets/Knowledge-Base/Partners/Technicolor/com51-tuner-driver.png" alt="COM51 Tuner driver in Creator" width="700" height="">
</a>

1. Navigate to **Creator > Equipment**
2. Search for **Technicolor COM51 Tuner** driver
3. Name the driver to identify it in SAVI (each driver will connect to a single tuner)
4. Configure the properties as follows:
    >* **Management IP:** The IP address of the tuner (from step 3 in "**COM51 Tuner IP**").
    >* **Chassis:** The chassis number. If this is your only chassis, then this will be `1`.
    >* **Slot:** The COM51 card slot. This can be found on the Overview page as well as the Tuner page.
    >* **Tuner:** The tuner number. This can be found on the Overview page as well as the Tuner page.
    >Leave the other fields alone.

5. Click **Add to Project**

Your SAVI project now has a source with the same name as your newly created driver. Repeat this driver addition for each tuner on each COM51 so they are available to SAVI.

Congratulations! Your COM3000 system is now configured.

Check out [how to control your new sources in SAVI](/Knowledge-Base/User-Interface/Facility/facility-performing-tasks.md "how to control your new sources in SAVI") for directions on using sources in Facility View.
