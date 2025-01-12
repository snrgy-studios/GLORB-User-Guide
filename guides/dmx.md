---
layout: default
title: DMX Control Guide
---

<div class="back-nav">
  <a href="{{ site.baseurl }}/">← Back to Guide</a>
</div>

# DMX Control Guide

> **Important:** Before proceeding, make sure your GLORB is running the [latest firmware]({{ site.baseurl }}/firmware). With the latest release, you can optionally disable the Bluetooth Control module for a smoother DMX output, since it interferes with realtime light control due to WiFi sleep requirements.

## Overview
The GLORB is built using [WLED](https://kno.wled.ge/) firmware, which supports variuos protocols for realtime light control from computers and light interfaces. 

This guide will show you how to set up remote DMX control on your GLORB!

## Configuring DMX (E1.31/Art-Net)

1. (iOS) Go to Settings → WLED Controls to access the WLED interface
    - Make sure your GLORB is [connected to WiFi]({{ site.baseurl }}/setup)
2. (Optional) Navigate to Config → Usermods
    - Disable the Bluetooth Control module and press Save
3. Navigate to Config → Sync Interfaces
    - Select your DMX settings and press Save (see below for more details)
4. Reboot the GLORB
5. Enter the IP address of your GLORB in your DMX software
    - iOS: Find your IP in Settings → Info
    - Android: Find your IP on the device screen in WLED Native

## DMX Channel Mapping

WLED supports several DMX modes that can be selected in the Sync Interfaces settings. Below is a summary of the [WLED DMX Documentation](https://kno.wled.ge/interfaces/e1.31-dmx/). 

> **Important:** DO NOT disable WiFi sleep as recommended in the WLED documentation. Instead, follow the instructions above to disable the Bluetooth module.

> **Note:** The GLORB animations have Effect Mode IDs starting from 187

### Single RGB (3 channels)
All LEDs are set to the same color:
- Channel 1: Red
- Channel 2: Green
- Channel 3: Blue

### Single DRGB (4 channels)
All LEDs set to same color with master dimmer:
- Channel 1: Master Dimmer
- Channel 2: Red
- Channel 3: Green
- Channel 4: Blue

### Effect Mode (15 channels)
Control WLED effects via DMX:
- Channel 1: Master Dimmer
- Channel 2: Effect Mode ID
- Channel 3: Effect Speed
- Channel 4: Effect Intensity
- Channel 5: Effect Palette ID
- Channel 6: Effect Options
- Channel 7-9: Primary Color (RGB)
- Channel 10-12: Secondary Color (RGB)
- Channel 13-15: Tertiary Color (RGB)

### Multiple RGB (most common)
3 channels per LED in sequence:
- LED 1: Red, Green, Blue
- LED 2: Red, Green, Blue
- etc...

This is the recommended mode for most DMX software like xLights and LedFx.

### WLED Documentation

For more detailed information and further options, visit the [WLED DMX Documentation](https://kno.wled.ge/interfaces/e1.31-dmx/). 

## GLORB LED Map

The GLORB is configured as a 6x20 matrix with 120 addressable LEDs, running from left to right. However, only 80 of these LEDs are physically present - the rest are "virtual" LEDs used for mapping purposes.

![GLORB LED Map]({{ site.baseurl }}/assets/images/ledmap.png)

When using DMX control with Multiple RGB mode, keep in mind:
- Each LED uses 3 channels (RGB)
- The full matrix is 120 LEDs = 360 channels
- LEDs are addressed sequentially from left to right
- Not all LED positions are active (see map above)

For optimal control, configure your DMX software to match this 6x20 matrix layout. The LED map above shows which positions are active (blue) and inactive (black).