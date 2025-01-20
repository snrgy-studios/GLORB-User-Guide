---
layout: default
title: WLED Controls Guide
---

<div class="back-nav">
  <a href="{{ site.baseurl }}/">← Back to Guide</a>
</div>

# Understanding WLED Controls

## Overview

The GLORB is powered by [WLED](https://kno.wled.ge/), an open source lighting control system. While WLED includes many built-in effects designed for LED strips and flat panels, we've adapted a selection of these effects specifically for the GLORB's unique spherical shape. This ensures the lighting patterns flow smoothly across the curved surface.

The SNRGY app (iOS) shows you our customized effects, but you can also access WLED's complete collection of effects through its interface if you want to experiment with more options!

## WLED Controls

WLED provides a web interface that gives you access to additional settings and controls beyond what's available in the GLORB app. Here's how to access it:

For iOS users:
1. Open the SNRGY app and select your device
2. Go to Settings → WLED Controls
4. Select "Config" to see all available settings

Below you'll find a list of the most important settings you can adjust. For best results, we recommend leaving any settings not mentioned here at their default values.

### WiFi Setup
Configure your GLORB's network settings:
- Change WiFi network name and password
- Configure a static IP address if needed

> **Important:** Leave the WiFi sleep settings unchanged, as they are required for Bluetooth functionality.

### LED Preferences
Customize how your GLORB behaves:
- Set the default brightness level when powered on
- Choose which animation plays when your GLORB starts up:
    1. Find the preset ID number in your preset list
    2. Enter that ID in "Apply preset ___ at boot"

> **Note:** If you can't save changes, set "Maximum Current" to 5000 first.

### Sync Interfaces
Set up external control options:
- Connect to smart home systems like Home Assistant (see [Smart Home Integrations]({{ site.baseurl }}/guides/smart-home))
- Enable DMX control for professional lighting setups (see [DMX Control]({{ site.baseurl }}/guides/dmx))

### Time & Macros
Automate your GLORB:
- Set your local timezone
- Create schedules to automatically change presets at specific times

### Usermods
Advanced settings:
- Fine-tune sound reactivity sensitivity and response
- Toggle Bluetooth functionality
    - Disabling Bluetooth may help resolve [DMX control issues]({{ site.baseurl }}/guides/dmx)

### Security & Updates
Manage your device:
- Reset to factory settings if needed (see [Factory Reset Instructions]({{ site.baseurl }}/troubleshooting#factory-reset-instructions))
- Update firmware manually (see [Firmware Updates]({{ site.baseurl }}/firmware#android-users))
- Backup and restore your presets (see [Backup and Restore Presets]({{ site.baseurl }}/troubleshooting#backup-and-restore-presets))

