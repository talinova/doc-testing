---
title: "Canvas Encoder Compatibility"
tags: documentation, datasheet, stream.one, canvas, encoder
date:
  created: "01/03/2023"
  modified: "01/03/2023"
description: A quick guide to encoding compatibility with the SAVI Stream.One and SAVI Canvas.
---

<div style="text-align: center">

<a href="../Assets/Documentation/stream-one.png">
  <img src="../Assets/Documentation/stream-one.png" width="700" height="">
</a>
</div>

# Canvas Encoder Compatibility
When using third-party devices in conjunction with SAVI, it is important to know what is or isn’t compatible with Canvas. This is a short informational guide to make that process easier.

To start off, the SAVI Stream.One is the only certified video encoder for the SAVI Canvas system. However, SAVI compatible LG Signage displays support video streaming using a broad array of open standards protocols. This means that many popular encoders will work out of the box with SAVI Canvas.

Here are some of the most common encoder standards used by SAVI dealers:

## Common Standards

<table>
<tr><th>   UDP           </th></tr>
<tr><th> Media Container </th><td> Transport Stream (TS) </td></tr>
<tr><th> Video Codec     </th><td> H.264                 </td></tr>
</table>

<table>
<tr><th>   RTP           </th></tr>
<tr><th> Media Container </th><td> Transport Stream (TS) </td></tr>
<tr><th> Video Codec     </th><td> H.264                 </td></tr>
</table>

For environments where keeping video playback in sync is paramount, we recommend using RTSP.

## Sync Focused Standards

<table>
<tr><th>   RTSP           </th></tr>
<tr><th> Media Container </th><td> Transport Stream (TS) </td></tr>
<tr><th> Video Codec     </th><td> H.264                 </td></tr>
</table>

For environments where playing multiple streams on a single display is needed, please keep in mind the following:

* If any of the streams are interlaced (ex: 1080i) only a single stream can be played on one display
* The combined bandwidth of the streams must fall below 50 mbps for Ultra HD and 40 mbps for Full HD

Please remember this is not a comprehensive list of compatible video encoder codecs. Further information can be found in the LG WebOS media formats document. If you have any questions regarding an encoder or codec you would like to use with SAVI Canvas, please reach out to your SAVI contact or our support team.

SAVI Support can be reached at +1 (214) 785-6510 option #2 between 8:00 a.m. - 5:00 p.m. CST.

>***All encoders must be tested with SAVI Canvas BEFORE being implemented in a live project***