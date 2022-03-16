[![LG logo](http://kb.savicontrols.com/wp-content/uploads/2020/10/2560px-LG_logo_2015.svg.png)](http://kb.savicontrols.com/wp-content/uploads/2020/10/2560px-LG_logo_2015.svg.png)

<img src='http://kb.savicontrols.com/wp-content/uploads/2020/10/2560px-LG_logo_2015.svg.png' alt='LG logo' width='1000'/>

![LG_logo_2015](http://kb.savicontrols.com/wp-content/uploads/2020/10/2560px-LG_logo_2015.svg.png)

# LG WebOS Displays

The LG Display drivers (SM5KC, SM5KD, SM5KE, and UL3G) allow control of those specific displays. However the LG webOS Display driver serves as a generic driver for all SAVI Canvas compatible LG webOS displays. As these drivers all share configurations, only the LG webOS Display driver is detailed below. These allow SAVI to tightly leverage Content, Control, and Management.

#### General Properties

[![SAVI Creator equipment. LG WebOS Display configuration general 1](http://kb.savicontrols.com/wp-content/uploads/2020/10/Creator-lg-webos-display-config-01-204x300.png)](http://kb.savicontrols.com/wp-content/uploads/2020/10/Creator-lg-webos-display-config-01.png)[![SAVI Creator equipment. LG WebOS Display configuration general 2](http://kb.savicontrols.com/wp-content/uploads/2020/10/Creator-lg-webos-display-config-02-203x300.png)](http://kb.savicontrols.com/wp-content/uploads/2020/10/Creator-lg-webos-display-config-02.png)

* **Name:** Name of Device. This is what is shown in Facility View.

* **Location:** Location of Display within Project.  Endpoints located within common rooms will automatically be quarriable within Facility View.  New Locations can be created by selecting field, typing in a new name, and then selecting corresponding "Add New Tag" option or pressing Enter on your keyboard.
[![Adding Main Dining Tag to Location](http://kb.savicontrols.com/wp-content/uploads/2020/10/Sources-03-300x91.png)](http://kb.savicontrols.com/wp-content/uploads/2020/10/Sources-03.png)

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

* **Streaming Latency:** The delay (in ms) injected into the streaming pipeline to keep playback smooth. Use -1 to keep the manufacturer's default.

#### Advanced Properties

[![SAVI Creator equipment. LG WebOS Display configuration advanced 1](http://kb.savicontrols.com/wp-content/uploads/2020/10/Creator-lg-webos-display-config-03-203x300.png)](http://kb.savicontrols.com/wp-content/uploads/2020/10/Creator-lg-webos-display-config-03.png)[![SAVI Creator equipment. LG WebOS Display configuration advanced 2](http://kb.savicontrols.com/wp-content/uploads/2020/10/Creator-lg-webos-display-config-04-202x300.png)](http://kb.savicontrols.com/wp-content/uploads/2020/10/Creator-lg-webos-display-config-04.png)
[![SAVI Creator equipment. LG WebOS Display configuration advanced 3](http://kb.savicontrols.com/wp-content/uploads/2020/10/Creator-lg-webos-display-config-05-300x128.png)](http://kb.savicontrols.com/wp-content/uploads/2020/10/Creator-lg-webos-display-config-05.png)

* **IR Remote Map: Video:** The way in which IR remotes control video in SAVI. Disabled prevents remote control, Gestures allows control of layouts and sources with a standard LG remote (Left and Right arrows toggle through sources, Up and Down arrows toggle through layouts), Control Source allows control of the connected source (if that source is controllable).

* **IR Remote Map: Audio:** The way in which IR remotes control audio in SAVI. Disabled prevents remote control. Allows the LG remote's volume buttons to control the display's volume (if "Control Display" is selected) or a SAVI Audio Zone (if "Control Audio Zone" is selected)

* **Audio Zone for IR Remote Map:** The audio zone to control when IR Remote Map: Audio is set to 'Control Audio Zone.'

* **Display Specific Region (1-4) Type:** Set the type of input so Creator knows whether to look at the URL field or Line In Input field.

* **Display Specific Region (1-4) URL:** For any type of URL (Video, Image, VNC). Ignored when Region Type is Line In.

* **Display Specific Region (1-4) Line In Input:** Ignored when Region Type is not Line In.

### Connections
[![SAVI Creator LG webOS input connections](http://kb.savicontrols.com/wp-content/uploads/2020/10/LG-WebOS-display-connections-input-278x300.png)](http://kb.savicontrols.com/wp-content/uploads/2020/10/LG-WebOS-display-connections-input.png)

##### Input

* **SAVI Canvas Network:** This connects to one of the available Canvas Network Sources. Recommend against changing this.

* **HDMI (1-3):** Connects to any available HDMI output.

* **DVI (1&2):** Connects to any available DVI output.
