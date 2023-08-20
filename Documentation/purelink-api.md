---
title: "Stream.One API"
tags: creator, driver, equipment, stream.one, savi, api
date:
  created: "08/25/2022"
  modified: "08/26/2022"
description: Resource for the SAVI Stream.One API.
---

<div style="text-align: center">

<a href="../Assets/Knowledge-Base/Creator/Drivers/Logos/savi-04-blue.svg">
  <img src="../Assets/Knowledge-Base/Creator/Drivers/Logos/savi-04-blue.svg" alt="SAVI Logo" width="700" height="">
</a>
</div>

# Stream.One API



## Stream.One 2K Version 1.00.25
|    | Get Commands                | Description           |
| :-: | ----------------------------|-----------------------|
| 1  | `*GETIPADDRESS!`                      | Get device ip address |
| 2  | `*GETSUBNET!`                         | Get device subnet |
| 3  | `*GETGATEWAY!`                        | Get device gateway |
| 4  | `*GETIPMETHOD!`                       | Get device ip method |
| 5  | `*GETMACADDRESS!`                     | Get device mac address |
| 6  | `*GETACTIVESIGNAL!`                   | Get input signal active status |
| 7  | `*GETINPUTDATA!`                      | Get input signal information |
| 8  | `*GETSPLASHSCREEN!`                   | Get splashscreen on/off status |
| 9  | `*GETOSDON!`                          | Get osd text string |
| 10 | `*GETOSDONSTATE!`                     | Get osd on/off status |
| 11 | `*GETDEVICES!`                        | Get online devices |
| 12 | `*GETSTREAMLOCKSTATE!`                | Get front panel stream button lock on/off status |
| 13 | `*GETMENULOCKSTATE!`                  | Get front panel menu button lock on/off status |
| 14 | `*GETFIRMWARE!`                       | Get device firmware version |
| 15 | `*GETMAINSTREAMSTATE!`                | Get main stream status |
| 16 | `*GETAUDIOSTREAMSTATE!`               | Get audio stream status |
| 17 | `*GETCHANNEL!`                        | Get channel number |
| 18 | `*GETUSERLABEL!`                      | Get userlabel |
| 19 | `*GETEDID!`                           | Get current edid data |
| 20 | `*GETTEMP!`                           | Get device internal temperature |
| 21 | `*GETRUNHOURS!`                       | Get device run time |
| 22 | `*GETFAULTS!`                         | Get report error information |
| 23 | `*GETSERIALNUMBER!`                   | Get serial number |
| 24 | `*GETSDP!`                            | Get session description protocol file |
| 25 | `*GETANALOGAUDIODELAY!`               | Get analog audio delay time (ms) |
| 26 | `*GETENCODERBITRATE!`                 | Get encoder bitrate |
| 27 | `*GETENCODERBITRATECONTROL!`          | Get encoder bitrate control |
| 28 | `*GETENCODERFRAMERATE!`               | Get encoder frame rate |
| 29 | `*GETENCODERRESOLUTION!`              | Get encoder resolution |
| 30 | `*GETENCODERH264LEVEL!`               | Get encoder h264 level |
| 31 | `*GETENCODERGOP!`                     | Get encoder gop |
| 32 | `*GETMAINMULTICAST!`                  | Get main multicastip and port number |
| 33 | `*GETSECONDMULTICAST!`                | Get second multicastip and port number |

|    | Set Commands                       | Description    |
| :-: | ---------------------------------- |----------------|
| 34 | `*SETANALOGAUDIODELAY_[nnnn]!`     | Set analog audio delay time (ms)  nnnn= 0 ~ 1500 |
| 35 | `*SETENCODERBITRATE_[nnnn]!`       | Set encoder bitrate nnnn= 32 ~ 32000 |
| 36 | `*SETENCODERBITRATECONTROL_[xxx]!` | Set encoder bitrate control  xxx=VBR  xxx=CBR |
| 37 | `*SETENCODERFRAMERATE_[nn]!`       | Set encoder frame rate  nn= 5 ~ 60 |
| 38 | `*SETENCODERRESOLUTION_[xxx]!`     | Set encoder resolution xxx=SAME xxx=1080 xxx = 720 xxx=480 |
| 39 | `*SETENCODERH264LEVEL_[xxx]!`      | Set encoder h264 level xxx=BASELINE xxx=MAIN xxx=HIGH |
| 40 | `*SETENCODERGOP_[nnn]!`            | Set encoder gop nnn= 5 ~ 300 |
| 41 | `*SETCHANNEL_[xxx]!`               | Set channel number  xxx= 0 ~ 999 |
| 42 | `*SETIPADDRESS_[nnn.nnn.nnn.nnn]!` | Set static network ip |
| 43 | `*SETSUBNET_[nnn.nnn.nnn.nnn]!`    | Set static network netmask |
| 44 | `*SETGATEWAY_[nnn.nnn.nnn.nnn]!`   | Set static network gateway |
| 45 | `*SETIPMETHOD_[xxx]!`              | Set ip method       xxx=STATIC   xxx=DHCP |
| 46 | `*SETEDID_[xxx]!`                  | Set edid mode       xxx=DEFAULT  xxx=1080   xxx=720   xxx=CUSTOM |
| 47 | `*SETOSDON_[sss]!`                 | Set osd on and osd text on |
| 48 | `*SETOSDOFF!`                      | Set osd off |
| 49 | `*SETUSERLABEL_[xxx]!`             | Set user label |
| 50 | `*SETALLSTREAMSTATE_[xxx]!`        | Set stream status   xxx=START    xxx=PAUSE  xxx=STOP |
| 51 | `*SETMAINSTREAMSTATE_[xxx]!`       | Set main stream status   xxx=START    xxx=PAUSE  xxx=STOP |
| 52 | `*SETAUDIOSTREAMSTATE_[xxx]!`      | Set audio stream status   xxx=START    xxx=PAUSE  xxx=STOP |
| 53 | `*SETSPLASHSCREEN_[xxx]!`          | Set splashscreen on/off          xxx=ON     xxx=OFF |
| 54 | `*SETSTREAMLOCKSTATE_[xxx]!`       | Set front pane stream button lock on/off       xxx=ON     xxx=OFF |
| 55 | `*SETMENULOCKSTATE_[xxx]!`         | Set front pane menu button lock on/off       xxx=ON     xxx=OFF |
| 56 | `*SETSIGNALMUTE_[xxx]!`            | Set input mute  xxx = ON  xxx = OFF |
| 57 | `*REBOOT!`                         | Set reboot the device |
| 58 | `*SETFACTORYDEFAULT!`              | Set reset the device |
| 59 | `*HELP!`                           | Show all Get/Set Commands |



## Stream.One 2K Version 1.00.38

|    | Get Commands                         | Description      |
| :-: | ------------------------------------ |------------------|
| 1  | `*GETIPADDRESS!`              | Get device ip address               |
| 2  | `*GETSUBNET!`                 | Get device subnet                   |
| 3  | `*GETGATEWAY!`                | Get device gateway                  |
| 4  | `*GETPREFERREDDNS!`           | Get device preferred dns server     |
| 5  | `*GETALTERNATEDNS!`           | Get device alternate dns server     |
| 6  | `*GETIPMETHOD!`               | Get device ip method                |
| 7  | `*GETMACADDRESS!`             | Get device mac address              |
| 8  | `*GETACTIVESIGNAL!`           | Get input signal active status      |
| 9  | `*GETINPUTDATA!`              | Get input signal information        |
| 10 | `*GETSPLASHSCREEN!`           | Get splashscreen on/off status      |
| 11 | `*GETOSDON!`                  | Get osd text string                 |
| 12 | `*GETOSDONSTATE!`             | Get osd on/off status               |
| 13 | `*GETDEVICES!`                | Get online devices                  |
| 14 | `*GETSTREAMLOCKSTATE!`        | Get front panel stream button lock on/off status     |
| 15 | `*GETMENULOCKSTATE!`          | Get front panel menu button lock on/off status       |
| 16 | `*GETFIRMWARE!`               | Get device firmware version         |
| 17 | `*GETMAINSTREAMSTATE!`        | Get main stream status              |
| 18 | `*GETAUDIOSTREAMSTATE!`       | Get audio stream status             |
| 19 | `*GETCHANNEL!`                | Get channel number                  |
| 20 | `*GETUSERLABEL!`              | Get userlabel                       |
| 21 | `*GETEDID!`                   | Get current edid data               |
| 22 | `*GETTEMP!`                   | Get device internal temperature     |
| 23 | `*GETRUNHOURS!`               | Get device run time                 |
| 24 | `*GETFAULTS!`                 | Get report error information        |
| 25 | `*GETSERIALNUMBER!`           | Get serial number                   |
| 26 | `*GETSDP!`                    | Get session description protocol file    |
| 27 | `*GETANALOGAUDIODELAY!`       | Get analog audio delay time (ms)    |
| 28 | `*GETENCODERBITRATE!`         | Get encoder bitrate                 |
| 29 | `*GETENCODERBITRATECONTROL!`  | Get encoder bitrate control         |
| 30 | `*GETENCODERFRAMERATE!`       | Get encoder frame rate              |
| 31 | `*GETENCODERRESOLUTION!`      | Get encoder resolution              |
| 32 | `*GETENCODERH264LEVEL!`       | Get encoder h264 level              |
| 33 | `*GETENCODERGOP!`             | Get encoder gop                     |
| 34 | `*GETNTPSERVER!`              | Get NTP Server                      |
| 35 | `*GETNTPPORT!`                | Get NTP port                        |
| 36 | `*GETTSMULTICAST!`            | Get TS Multicast Address            |
| 37 | `*GETRTSPMULTICAST!`          | Get RTSP Multicast Address          |
| 38 | `*GETAUDIOMULTICAST!`         | Get Audio Multicast Address         |
| 39 | `*GETCPU\_USAGE!`             | Reports CPU load                    |
| 40 | `*GETMEMORY\_USAGE!`          | Reports memory load                 |
| 41 | `*GETDRTSPCONNECT!`           | Get rtsp connect status             |

|    | Set Commands                         | Description      |
| :-: | ------------------------------------ |------------------|
| 42 | `*SETANALOGAUDIODELAY_[nnnn]!`        | Set analog audio delay time (ms)  nnnn= 0 ~ 1500  |
| 43 | `*SETENCODERBITRATE_[nnnn]!`          | Set encoder bitrate nnnn= 32 ~ 32000    |
| 44 | `*SETENCODERBITRATECONTROL_[xxx]!`    | Set encoder bitrate control  xxx=VBR  xxx=CBR  |
| 45 | `*SETENCODERFRAMERATE_[nn]!`          | Set encoder frame rate  nn= 5 ~ 30      |
| 46 | `*SETENCODERRESOLUTION_[xxx]!`        | Set encoder resolution xxx=SAME xxx=1080 xxx = 720 xxx=480  |
| 47 | `*SETENCODERH264LEVEL_[xxx]!`         | Set encoder h264 level xxx=BASELINE xxx=MAIN xxx=HIGH  |
| 48 | `*SETENCODERGOP_[nnn]!`               | Set encoder gop nnn= 5 ~ 300    |
| 49 | `*SETCHANNEL_[xxx]!`                  | Set channel number  xxx= 0 ~ 999         |
| 50 | `*SETIPADDRESS_[nnn.nnn.nnn.nnn]!`    | Set static network ip         |
| 51 | `*SETSUBNET_[nnn.nnn.nnn.nnn]!`       | Set static network netmask        |
| 52 | `*SETGATEWAY_[nnn.nnn.nnn.nnn]!`      | Set static network gateway          |
| 53 | `*SETPREFERREDDNS_[nnn.nnn.nnn.nnn]!` | Set static preferred dns server        |
| 54 | `*SETALTERNATEDNS_[nnn.nnn.nnn.nnn]!` | Set static alternate dns server        |
| 55 | `*SETIPMETHOD_[xxx]!`                 | Set ip method       xxx=STATIC   xxx=DHCP       |
| 56 | `*SETEDID_[xxx]!`                     | Set edid mode       xxx=DEFAULT  xxx=1080   xxx=720   xxx=CUSTOM  |
| 57 | `*SETOSDON_[x,y]_[sss]!`              | Set osd on and osd text on[x,y]         |
| 58 | `*SETOSDOFF!`                         | Set osd off             |
| 59 | `*SETUSERLABEL_[xxx]!`                | Set user label               |
| 60 | `*SETALLSTREAMSTATE_[xxx]!`           | Set stream status   xxx=START    xxx=PAUSE  xxx=STOP    |
| 61 | `*SETMAINSTREAMSTATE_[xxx]!`          | Set main stream status   xxx=START    xxx=PAUSE  xxx=STOP |
| 62 | `*SETAUDIOSTREAMSTATE_[xxx]!`         | Set audio stream status   xxx=START    xxx=PAUSE  xxx=STOP |
| 63 | `*SETNTPSERVER_[xxx]!`                | Set NTP Server         |
| 64 | `*SETNTPPORT_[xxx]!`                  | Set NTP port nnn= 1 ~ 65535          |
| 65 | `*SETTSMULTICAST_[xxx]!`              | Set TS Multicast Enable on/off       xxx=ON     xxx=OFF   |
| 66 | `*SETRTSPMULTICAST_[xxx]!`            | Set RTSP Multicast Enable on/off       xxx=ON     xxx=OFF |
| 67 | `*SETRTSPUNICAST_[xxx]!`              | Set RTSP Unicast Enable on/off       xxx=ON     xxx=OFF  |
| 68 | `*SETAUDIOMULTICAST_[xxx]!`           | Set Audio only Multicast Enable on/off       xxx=ON     xxx=OFF |
| 69 | `*SETTSMULTICASTPORT_[xxx]!`          | Set TS Multicast Port nnn= 1 ~ 65535  |
| 70 | `*SETRTSPMULTICASTPORT_[xxx]!`        | Set RTSP Multicast Port nnn= even number(2 ~ 65532)  |
| 71 | `*SETAUDIOMULTICASTPORT_[xxx]!`       | Set Audio only Multicast Port nnn= even number(2 ~ 65532) |
| 72 | `*SETSPLASHSCREEN_[xxx]!`             | Set splashscreen on/off          xxx=ON     xxx=OFF   |
| 73 | `*SETSTREAMLOCKSTATE_[xxx]!`          | Set front pane stream button lock on/off       xxx=ON     xxx=OFF |
| 74 | `*SETMENULOCKSTATE_[xxx]!`            | Set front pane menu button lock on/off       xxx=ON     xxx=OFF  |
| 75 | `*SETSIGNALMUTE_[xxx]!`               | Set input mute  xxx = ON  xxx = OFF    |
| 76 | `*REBOOT!`                            | Set reboot the device         |
| 77 | `*SETFACTORYDEFAULT!`                 | Set reset the device        |
| 78 | `*HELP!`                              | Show all Get/Set Commands        |

## Stream.One 2K Version 1.10.10

|    | Get Commands                | Description                                      |
| :-: | --------------------------- | ------------------------------------------------ |
| 1  | `*GETIPADDRESS!`             | Get device ip address                            |
| 2  | `*GETSUBNET!`                | Get device subnet                                |
| 3  | `*GETGATEWAY!`               | Get device gateway                               |
| 4  | `*GETPREFERREDDNS!`          | Get device preferred dns server                  |
| 5  | `*GETALTERNATEDNS!`          | Get device alternate dns server                  |
| 6  | `*GETIPMETHOD!`              | Get device ip method                             |
| 7  | `*GETMACADDRESS!`            | Get device mac address                           |
| 8  | `*GETACTIVESIGNAL!`          | Get input signal active status                   |
| 9  | `*GETINPUTDATA!`             | Get input signal information                     |
| 10 | `*GETSPLASHSCREEN!`          | Get splashscreen on/off status                   |
| 11 | `GETOSDON!`                  | Get osd text string                              |
| 12 | `*GETOSDONSTATE!`            | Get osd on/off status                            |
| 13 | `*GETDEVICES!`               | Get online devices                               |
| 14 | `*GETSTREAMLOCKSTATE!`       | Get front panel stream button lock on/off status |
| 15 | `*GETMENULOCKSTATE!`         | Get front panel menu button lock on/off status   |
| 16 | `*GETFIRMWARE!`              | Get device firmware version                      |
| 17 | `*GETMAINSTREAMSTATE!`       | Get main stream status                           |
| 18 | `*GETAUDIOSTREAMSTATE!`      | Get audio stream status                          |
| 19 | `*GETCHANNEL!`               | Get channel number                               |
| 20 | `*GETUSERLABEL!`             | Get userlabel                                    |
| 21 | `*GETEDID!`                  | Get current edid data                            |
| 22 | `*GETTEMP!`                  | Get device internal temperature                  |
| 23 | `*GETRUNHOURS!`              | Get device run time                              |
| 24 | `*GETFAULTS!`                | Get report error information                     |
| 25 | `*GETSERIALNUMBER!`          | Get serial number                                |
| 26 | `*GETSDP!`                   | Get session description protocol file            |
| 27 | `*GETANALOGAUDIODELAY!`      | Get analog audio delay time (ms)                 |
| 28 | `*GETENCODERBITRATE!`        | Get encoder bitrate                              |
| 29 | `*GETENCODERBITRATECONTROL!` | Get encoder bitrate control                      |
| 30 | `*GETENCODERFRAMERATE!`      | Get encoder frame rate                           |
| 31 | `*GETENCODERRESOLUTION!`     | Get encoder resolution                           |
| 32 | `*GETENCODERH264LEVEL!`      | Get encoder h264 level                           |
| 33 | `*GETENCODERGOP!`            | Get encoder gop                                  |
| 34 | `*GETNTPSERVER!`             | Get NTP Server                                   |
| 35 | `*GETNTPPORT!`               | Get NTP port                                     |
| 36 | `*GETTSMULTICAST!`           | Get TS Multicast Address                         |
| 37 | `*GETRTSPMULTICAST!`         | Get RTSP Multicast Address                       |
| 38 | `*GETAUDIOMULTICAST!`        | Get Audio Multicast Address                      |
| 39 | `*GETCPU_USAGE!`             | Reports CPU load                                 |
| 40 | `*GETMEMORY_USAGE!`          | Reports memory load                              |
| 41 | `*GETDRTSPCONNECT!`          | Get rtsp connect status                          |

|    | Set Commands                          | Description             |
| :-: | ------------------------------------- | ----------------------- |
| 42 | `*SETANALOGAUDIODELAY_[nnnn]!`        | Set analog audio delay time (ms)  nnnn= 0 ~ 1500                  |
| 43 | `*SETENCODERBITRATE_[nnnn]!`          | Set encoder bitrate nnnn= 32 ~ 32000                              |
| 44 | `*SETENCODERBITRATECONTROL_[xxx]!`    | Set encoder bitrate control  xxx=VBR  xxx=CBR                     |
| 45 | `*SETENCODERFRAMERATE_[nn]!`          | Set encoder frame rate  nn= 5 ~ 30                                |
| 46 | `*SETENCODERRESOLUTION_[xxx]!`        | Set encoder resolution xxx=SAME xxx=1080 xxx = 720 xxx=480        |
| 47 | `*SETENCODERH264LEVEL_[xxx]!`         | Set encoder h264 level xxx=BASELINE xxx=MAIN xxx=HIGH             |
| 48 | `*SETENCODERGOP_[nnn]!`               | Set encoder gop nnn= 5 ~ 300                                      |
| 49 | `*SETCHANNEL_[xxx]!`                  | Set channel number  xxx= 0 ~ 999                                  |
| 50 | `*SETIPADDRESS_[nnn.nnn.nnn.nnn]!`    | Set static network ip                                             |
| 51 | `*SETSUBNET_[nnn.nnn.nnn.nnn]!`       | Set static network netmask                                        |
| 52 | `*SETGATEWAY_[nnn.nnn.nnn.nnn]!`      | Set static network gateway                                        |
| 53 | `*SETPREFERREDDNS_[nnn.nnn.nnn.nnn]!` | Set static preferred dns server                                   |
| 54 | `*SETALTERNATEDNS_[nnn.nnn.nnn.nnn]!` | Set static alternate dns server                                   |
| 55 | `*SETIPMETHOD_[xxx]!`                 | Set ip method       xxx=STATIC   xxx=DHCP                         |
| 56 | `*SETEDID_[xxx]!`                     | Set edid mode       xxx=DEFAULT  xxx=1080   xxx=720   xxx=CUSTOM  |
| 57 | `*SETOSDON_[x,y]_[sss]!`              | Set osd on and osd text on[x,y]                                 |
| 58 | `*SETOSDOFF!`                         | Set osd off                                                       |
| 59 | `*SETUSERLABEL_[xxx]!`                | Set user label                                                    |
| 60 | `*SETALLSTREAMSTATE_[xxx]!`           | Set stream status   xxx=START    xxx=PAUSE  xxx=STOP              |
| 61 | `*SETMAINSTREAMSTATE_[xxx]!`          | Set main stream status   xxx=START    xxx=PAUSE  xxx=STOP         |
| 62 | `*SETAUDIOSTREAMSTATE_[xxx]!`         | Set audio stream status   xxx=START    xxx=PAUSE  xxx=STOP        |
| 63 | `*SETNTPSERVER_[xxx]!`                | Set NTP Server                                                    |
| 64 | `*SETNTPPORT_[xxx]!`                  | Set NTP port nnn= 1 ~ 65535                                       |
| 65 | `*SETTSMULTICAST_[xxx]!`              | Set TS Multicast Enable on/off       xxx=ON     xxx=OFF           |
| 66 | `*SETRTSPMULTICAST_[xxx]!`            | Set RTSP Multicast Enable on/off       xxx=ON     xxx=OFF         |
| 67 | `*SETRTSPUNICAST_[xxx]!`              | Set RTSP Unicast Enable on/off       xxx=ON     xxx=OFF           |
| 68 | `*SETAUDIOMULTICAST_[xxx]!`           | Set Audio only Multicast Enable on/off       xxx=ON     xxx=OFF   |
| 69 | `*SETTSMULTICASTPORT_[xxx]!`          | Set TS Multicast Port nnn= 1 ~ 65535                              |
| 70 | `*SETRTSPMULTICASTPORT_[xxx]!`        | Set RTSP Multicast Port nnn= even number(2 ~ 65532)               |
| 71 | `*SETAUDIOMULTICASTPORT_[xxx]!`       | Set Audio only Multicast Port nnn= even number(2 ~ 65532)         |
| 72 | `*SETSPLASHSCREEN_[xxx]!`             | Set splashscreen on/off          xxx=ON     xxx=OFF               |
| 73 | `*SETSTREAMLOCKSTATE_[xxx]!`          | Set front pane stream button lock on/off       xxx=ON     xxx=OFF |
| 74 | `*SETMENULOCKSTATE_[xxx]!`            | Set front pane menu button lock on/off       xxx=ON     xxx=OFF   |
| 75 | `*SETSIGNALMUTE_[xxx]!`               | Set input mute  xxx = ON  xxx = OFF                               |
| 76 | `*REBOOT!`                            | Set reboot the device                                             |
| 77 | `*SETFACTORYDEFAULT!`                 | Set reset the device                                              |
| 78 | `*HELP!`                              | Show all Get/Set Commands                                         |

## Stream.One 2K Version 1.10.17

|    | Get Commands                      | Description                                         |
| :-: | --------------------------------- | --------------------------------------------------- |
| 1  | `*GETIPADDRESS!`                   | Get device ip address                               |
| 2  | `*GETSUBNET!`                      | Get device subnet                                   |
| 3  | `*GETGATEWAY!`                     | Get device gateway                                  |
| 4  | `*GETPREFERREDDNS!`                | Get device preferred dns server                     |
| 5  | `*GETALTERNATEDNS!`                | Get device alternate dns server                     |
| 6  | `*GETIPMETHOD!`                    | Get device ip method                                |
| 7  | `*GETMACADDRESS!`                  | Get device mac address                              |
| 8  | `*GETACTIVESIGNAL!`                | Get input signal active status                      |
| 9  | `*GETINPUTDATA!`                   | Get input signal information                        |
| 10 | `*GETSPLASHSCREEN!`                | Get splashscreen on/off status                      |
| 11 | `*GETOSDON!`                       | Get osd text string                                 |
| 12 | `*GETOSDONSTATE!`                  | Get osd on/off status                               |
| 13 | `*GETDEVICES!`                     | Get online devices                                  |
| 14 | `*GETSTREAMLOCKSTATE!`             | Get front panel stream button lock on/off status    |
| 15 | `*GETMENULOCKSTATE!`               | Get front panel menu button lock on/off status      |
| 16 | `*GETFIRMWARE!`                    | Get device firmware version                         |
| 17 | `*GETMAINSTREAMSTATE!`             | Get main stream status                              |
| 18 | `*GETAUDIOSTREAMSTATE!`            | Get audio stream status                             |
| 19 | `*GETSECONDSTREAMSTATE!`           | Get second stream status                            |
| 20 | `*GETCHANNEL!`                     | Get channel number                                  |
| 21 | `*GETUSERLABEL!`                   | Get userlabel                                       |
| 22 | `*GETEDID!`                        | Get current edid data                               |
| 23 | `*GETTEMP!`                        | Get device internal temperature                     |
| 24 | `*GETRUNHOURS!`                    | Get device run time                                 |
| 25 | `*GETLIFEHOURS!`                   | Get device life hours                               |
| 26 | `*GETSERIALNUMBER!`                | Get serial number                                   |
| 27 | `*GETSDP!`                         | Get session description protocol file               |
| 28 | `*GETANALOGAUDIODELAY!`            | Get analog audio delay time (ms)                    |
| 29 | `*GETMAINENCODERBITRATE!`          | Get main encoder bitrate                            |
| 30 | `*GETSECONDENCODERBITRATE!`        | Get second encoder bitrate                          |
| 31 | `*GETMAINENCODERBITRATECONTROL!`   | Get main encoder bitrate control                    |
| 32 | `*GETSECONDENCODERBITRATECONTROL!` | Get second encoder bitrate control                  |
| 33 | `*GETMAINENCODERFRAMERATE!`        | Get main encoder frame rate                         |
| 34 | `*GETSECONDENCODERFRAMERATE!`      | Get second encoder frame rate                       |
| 35 | `*GETMAINENCODERRESOLUTION!`       | Get main encoder resolution                         |
| 36 | `*GETSECONDENCODERRESOLUTION!`     | Get second encoder resolution                       |
| 37 | `*GETMAINENCODERH265LEVEL!`        | Get main encoder h265 level                         |
| 38 | `*GETSECONDENCODERH264LEVEL!`      | Get second encoder h264 level                       |
| 39 | `*GETMAINENCODERGOP!`              | Get main encoder gop                                |
| 40 | `*GETSECONDENCODERGOP!`            | Get second encoder gop                              |
| 41 | `*GETNTPSERVER!`                   | Get NTP Server                                      |
| 42 | `*GETNTPPORT!`                     | Get NTP port                                        |
| 43 | `*GETMAINMULTICAST!`               | Get main TS and RTSP multicastip and port number    |
| 44 | `*GETSECONDMULTICAST!`             | Get second TS and RTSP  multicastip and port number |
| 45 | `*GETAUDIOMULTICAST!`              | Get audio only multicastip and port number          |
| 46 | `*GETCPU_USAGE!`                   | Reports CPU load                                    |
| 47 | `*GETMEMORY_USAGE!`                | Reports memory load                                 |
| 48 | `*GETMAINRTSPCONNECT!`             | Get main rtsp connect status                        |
| 49 | `*GETSECONDRTSPCONNECT!`           | Get second rtsp connect status                      |

|    | Set Commands                          | Description             |
| :-: | ------------------------------------- | ----------------------- |
| 50 | `*SETANALOGAUDIODELAY_[nnnn]!`           | Set analog audio delay time (ms)  nnnn= 0 ~ 1500                          |
| 51 | `*SETMAINENCODERBITRATE_[nnnn]!`         | Set main encoder bitrate nnnn= 32 ~ 32000                                 |
| 52 | `*SETSECONDENCODERBITRATE_[nnnn]!`       | Set second encoder bitrate nnnn= 32 ~ 32000                               |
| 53 | `*SETMAINENCODERBITRATECONTROL_[xxx]!`   | Set main encoder bitrate control  xxx=VBR  xxx=CBR                        |
| 54 | `*SETSECONDENCODERBITRATECONTROL_[xxx]!` | Set second encoder bitrate control  xxx=VBR  xxx=CBR                      |
| 55 | `*SETMAINENCODERFRAMERATE_[nn]!`         | Set main encoder frame rate  nn= 5 ~ 60                                   |
| 56 | `*SETSECONDENCODERFRAMERATE_[nn]!`       | Set second encoder frame rate  nn= 5 ~ 60                                 |
| 57 | `*SETMAINENCODERRESOLUTION_[xxx]!`       | Set main encoder resolution xxx=SAME xxx=4K xxx=1080 xxx = 720 xxx = 480  |
| 58 | `*SETSECONDENCODERRESOLUTION_[xxx]!`     | Set second encoder resolution xxx=1080 xxx = 720 xxx = 480                |
| 59 | `*SETMAINENCODERH265LEVEL_[xxx]!`        | Set main encoder h265 level xxx=MAIN                                      |
| 60 | `*SETSECONDENCODERH264LEVEL_[xxx]!`      | Set second encoder h264 level xxx=BASELINE xxx=MAIN xxx=HIGH              |
| 61 | `*SETMAINENCODERGOP_[nnn]!`              | Set main encoder gop nnn= 5 ~ 300                                         |
| 62 | `*SETSECONDENCODERGOP_[nnn]!`            | Set second encoder gop nnn= 5 ~ 300                                       |
| 63 | `*SETCHANNEL_[xxx]!`                     | Set channel number  xxx= 0 ~ 999                                          |
| 64 | `*SETIPADDRESS_[nnn.nnn.nnn.nnn]!`       | Set static network ip                                                     |
| 65 | `*SETSUBNET_[nnn.nnn.nnn.nnn]!`          | Set static network netmask                                                |
| 66 | `*SETGATEWAY_[nnn.nnn.nnn.nnn]!`         | Set static network gateway                                                |
| 67 | `*SETIPMETHOD_[xxx]!`                    | Set ip method       xxx=STATIC   xxx=DHCP                                 |
| 68 | `*SETPREFERREDDNS_[nnn.nnn.nnn.nnn]!`    | Set static preferred dns server                                           |
| 69 | `*SETALTERNATEDNS_[nnn.nnn.nnn.nnn]!`    | Set static alternate dns server                                           |
| 70 | `*SETEDID_[xxx]!`                        | Set edid mode       xxx=DEFAULT  xxx=2160 xxx=1080   xxx=720   xxx=CUSTOM |
| 71 | `*SETOSDON_[x,y]_[sss]!`                 | Set osd on and osd text on[x,y]                                           |
| 72 | `*SETOSDOFF!`                            | Set osd off                                                               |
| 73 | `*SETUSERLABEL_[xxx]!`                   | Set user label                                                            |
| 74 | `*SETALLSTREAMSTATE_[xxx]!`              | Set stream status   xxx=START    xxx=PAUSE  xxx=STOP                      |
| 75 | `*SETMAINSTREAMSTATE_[xxx]!`             | Set main stream status   xxx=START    xxx=PAUSE  xxx=STOP                 |
| 76 | `*SETSECONDSTREAMSTATE_[xxx]!`           | Set second stream status   xxx=START    xxx=PAUSE  xxx=STOP xxx=DISABLE   |
| 77 | `*SETAUDIOSTREAMSTATE_[xxx]!`            | Set audio stream status   xxx=START    xxx=PAUSE  xxx=STOP                |
| 78 | `*SETNTPSERVER_[xxx]!`                   | Set NTP Server                                                            |
| 79 | `*SETNTPPORT_[xxx]!`                     | Set NTP port nnn= 1 ~ 65535                                               |
| 80 | `*SETTSMULTICAST_[xxx]!`                 | Set TS Multicast Enable on/off       xxx=ENABLE     xxx=DISABLE           |
| 81 | `*SETRTSPMULTICAST_[xxx]!`               | Set RTSP Multicast Enable on/off       xxx=ENABLE     xxx=DISABLE         |
| 82 | `*SETRTSPUNICAST_[xxx]!`                 | Set RTSP Unicast Enable on/off       xxx=ENABLE     xxx=DISABLE           |
| 83 | `*SETAUDIOMULTICAST_[xxx]!`              | Set Audio only Multicast Enable on/off       xxx=ENABLE     xxx=DISABLE   |
| 84 | `*SETTSMULTICASTPORT_[xxx]!`             | Set TS Multicast Port nnn= 1 ~ 65535                                      |
| 85 | `*SETRTSPMULTICASTPORT_[xxx]!`           | Set RTSP Multicast Port nnn= even number(2 ~ 65532)                       |
| 86 | `*SETAUDIOMULTICASTPORT_[xxx]!`          | Set Audio only Multicast Port nnn= even number(2 ~ 65532)                 |
| 87 | `*SETSPLASHSCREEN_[xxx]!`                | Set splashscreen on/off          xxx=ON     xxx=OFF                       |
| 88 | `*SETSTREAMLOCKSTATE_[xxx]!`             | Set front pane stream button lock on/off       xxx=ON     xxx=OFF         |
| 89 | `*SETMENULOCKSTATE_[xxx]!`               | Set front pane menu button lock on/off       xxx=ON     xxx=OFF           |
| 90 | `*SETSIGNALMUTE_[xxx]!`                  | Set input mute  xxx = ON  xxx = OFF                                       |
| 91 | `*REBOOT!`                               | Set reboot the device                                                     |
| 92 | `*SETFACTORYDEFAULT!`                    | Set reset the device                                                      |
| 93 | `*HELP!`                                 | Show all Get/Set Commands                                                 |
