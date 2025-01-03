---
layout: default
title: Troubleshooting
---

<div class="back-nav">
  <a href="{{ site.baseurl }}/">← Back to Guide</a>
</div>

# Troubleshooting Guide

## Connection Issues

### Device Not Found in App
- Power cycle the GLORB (unplug and plug back in) and restart the app
- iOS: Make sure Bluetooth is enabled
- Android: Verify GLORB is [connected to WiFi]({{ site.baseurl }}/setup#verifying-connection))
- Ensure you're within range of device

### No Access Point (AP) in WiFi List
- Power cycle the GLORB and wait for a full boot
- Toggle device WiFi to refresh networks
- Check if not already connected (see [Verifying Connection](setup#verifying-connection))

## Performance Issues

### GLORB Flickers/Freezes/Crashes
- Power cycle the GLORB and verify the power supply specs
- [Update firmware]({{ site.baseurl }}/firmware) and check [Release Notes]({{ site.baseurl }}/releases) for known issues
- Check for smart home integration interference

## Factory Reset Instructions

### Using WLED Controls
1. Go to Config → Security & Updates
2. Check the "Factory Reset" box
3. Click "Save" and wait for device restart

### Using GLORB Web Installer
- Visit [GLORB Web Installer](https://snrgy-studios.github.io/GLORB-WebInstaller/) and follow the instructions

**Note:** Factory reset deletes all presets and settings. You'll need to [backup and restore presets](#backup-and-restore-presets) and [reconnect to WiFi]({{ site.baseurl }}/setup).

## Backup and Restore Presets

### Using WLED Controls

#### Backup Presets
- Go to Config → Security & Updates
- Click "Backup presets" to download presets.json

#### Restoring Presets
- Go to Config → Security & Updates
- Choose File → select presets.json
- Upload and wait for completion

## Still Need Help?
- Visit our [Community Forum](https://discord.com/invite/hnQ5V2GNjh)
- Contact support@glorb.me