---
title: "Audio Zone Has No Audio"
tags: creator, savi, sources, driver, audio, facility, troubleshooting
date:
  created: "03/21/2022"
  modified: "09/13/2022"
  description: Troubleshooting instructions for inoperable audio zone.
---

# Audio Zone Has No Audio
<a href="../../Assets/Knowledge-Base/Creator/Drivers/audio-zone.png">
  <img src="../../Assets/Knowledge-Base/Creator/Drivers/audio-zone.png" alt="Creator Audio Zone driver" width="300" height="">
</a>

If speaker audio zones in Facility View are not playing, the volume defaults and presets may not be configured. Follow these steps:

1. In Creator, navigate to the Equipment category, to the Equipment in Project list, then find the Audio Zone driver that is not producing audio.

2. Verify the Max Value is either -1 or high enough to be audible.
    >This may need to be set to -1 temporarily to prevent Creator from capping the volume too low.

3. Verify the Default Value field has a value specified (range=0 to 100).
    >This may need to be set to 100 temporarily for troubleshooting.

4. If applicable, verify the Alternate Volume Control is connected to the correct audio control device and port.
    >This configuration option is not always needed, depending on the audio device used.

If the audio zone still does not play audio, try the following steps:

1. In Facility View, select Volume Presets from the menu and select the audio zone

2. Verify at least 1 volume preset is enabled and configured to >0.
