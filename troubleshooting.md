---
layout: default
title: Troubleshooting
---

<div class="back-nav">
  <a href="{{ site.baseurl }}/">← Back to Guide</a>
</div>

# Troubleshooting Guide

## Connection Issues

### GLORB Not Found in App
- Power cycle the GLORB (unplug and plug back in) and restart the app
- iOS: Make sure Bluetooth is enabled
- Android: Verify GLORB is [connected to WiFi]({{ site.baseurl }}/setup#verifying-connection)

### No Access Point (AP) in WiFi List
- Power cycle the GLORB and wait for a full boot
- Toggle device WiFi to refresh network list
- Verify that the GLORB is not already [connected to WiFi]({{ site.baseurl }}/setup)

### Connection Failed
- Check that you're using the correct WiFi network and password
- Check that you're connecting to a 2.4GHz WiFi network (5GHz networks are not supported)
- Disable VPNs or other network interference
- If AP configuration failed, make sure you changed the network settings and not the access point settings (further down on the page). This would rename the AP to the network name (SSID) you entered.

## Performance Issues

### GLORB does not start
- Could be a faulty power supply. See if you can try another one with the same specs (5V/3A)
- Check if the app recognizes the unit or if the access point (AP) appears in your WiFi networks list. This means it's running but not outputting light. 
- Fully reset the firmware using the [Web Installer]({{ site.baseurl }}/firmware#web-installer) (bottom of the page). If the web installer doesn't recognise the unit it is not booting at all. 
- If still not working, contact [support](mailto:support@glorb.me) and we will replace your unit.

### GLORB Flickers/Freezes/Crashes
- Power cycle the GLORB and verify the power supply specs
- [Update firmware]({{ site.baseurl }}/firmware) and check [Release Notes]({{ site.baseurl }}/releases) for known issues
- Check for smart home integration interference

## App Features

### Sync Feature
- Sync only triggers when there's an actual state change on the device
- Make sure all devices are connected to the same WiFi network
- If multiple devices have sync enabled, they will all broadcast their state changes to each other. Consider designating one device as the master
- If still not working, try toggling sync off and on again in the app and reboot all synced devices

### Scheduling Feature
- Scheduling requires WiFi and location services to work properly. Set your location in device settings to update the local time. You might need to restart the app after setting the location. 

## Factory Reset Instructions

### Using GLORB Web Installer
- Visit the [Web Installer]({{ site.baseurl }}/firmware#web-installer) section (bottom of the page) and follow the instructions

### Using WLED Controls
1. Go to Config → Security & Updates
2. Check the "Factory Reset" box
3. Click "Save" and wait for device restart

**Note:** Factory reset deletes all presets and settings. You'll need to [backup and restore presets](#backup-and-restore-presets) and [reconnect to WiFi]({{ site.baseurl }}/setup).

## Backup and Restore Presets

### Using WLED Controls

#### Backup Presets
- Go to Config → Security & Updates
- Click "Backup presets" to download a presets.json file with all your presets

#### Restoring Presets
- Go to Config → Security & Updates
- Choose File → select the presets.json file you downloaded
- Upload and wait for completion

## Still Need Help?
- Visit our [Community Forum](https://discord.com/invite/hnQ5V2GNjh)
- Email: [support@glorb.me](mailto:support@glorb.me)