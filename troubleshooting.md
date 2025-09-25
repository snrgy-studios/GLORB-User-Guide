---
layout: default
title: Troubleshooting
---

<div class="back-nav">
  <a href="/">← Back to Guide</a>
</div>

# Troubleshooting Guide

> The GLORB is a new product in its first production release and we are working hard to fix any issues you may encounter. This guide covers common issues and their solutions. If you need further assistance, please reach out to our support team at [support@glorb.me](mailto:support@glorb.me) - we're committed to ensuring your GLORB works perfectly and we really appreciate your help and patience in this process! 

## Connection Issues

### GLORB Not Found in App
- Make sure Bluetooth is enabled
- Try allowing location services for the app
- Power cycle the GLORB (unplug and plug back in) and restart the app

### No Access Point (AP) in WiFi List
- Power cycle the GLORB and wait for a full boot
- Toggle device WiFi to refresh network list
- Verify that the GLORB is not already [connected to WiFi](/setup) (this will deactivate the AP)

### Connection Failed
- Check that you're using the correct WiFi network and password
- Check that you're connecting to a 2.4GHz WiFi network (5GHz networks are not supported)
  - Most routers support both the 2.4GHz and 5GHz band, but you may need to check your router settings to see which ones are active.  
- Try disabling VPNs or other network interference

## Performance Issues

### GLORB does not start
- Could be due to a faulty power supply. See if you can try another one with the same specs (5V/3A)
- Check if the app recognizes the unit or if the access point (AP) appears in your WiFi networks list. This means the GLORB is running but not outputting light. 
- Fully reset the firmware using the [Web Installer](/firmware#web-installer) (bottom of the page). If the web installer does not recognise the unit it is likely not booting at all. 
- If still not working, contact [support](mailto:support@glorb.me) and we will replace your unit.

### GLORB starts by itself

- Try another power supply with the same specs (5V/3A)
- Reset firmware using the [Web Installer](/firmware#web-installer) to clear potential firmware issues
- If you have active features like sync or smart home integrations, try disabling them to isolate the cause. If this resolves the issue, please let us know at [support](mailto:support@glorb.me)
- **If the issue persists**, you can prevent the GLORB from turning on after a restart:
  1. Go to WLED Controls → Config → LED Preferences
  2. Under "Defaults", uncheck "Turn LEDs on after power up/reset"
  3. Click Save
  - This means if the GLORB restarts, it will remain off until manually switched on
  - If you are unable to save the page, change "Maximum Current" from 0 to 5000

<div style="text-align: center">
  <img src="/assets/images/wled-default-boot.png" alt="WLED Default Boot Setting" width="80%">
</div>

### GLORB Flickers/Freezes/Crashes
- Could be due to a faulty power supply. See if you can try another one with the same specs (5V/3A)
- [Update firmware](/firmware) and check [Release Notes](/releases) for known issues
- Try disabling any smart home integrations or sync features to see if the issue persists

## App Features

### Sync Feature
- Confirm all devices share the same network
- Try toggling sync off and on
- Restart the app and devices
- Increase [UDP retransmissions](/info/wled-sync#sync-settings) if sync is unreliable
- Verify router supports network broadcast traffic

### Scheduling Feature
- Scheduling requires WiFi and location services to work properly. Set your location in device settings to update the local time. 
- You might need to restart the app after setting the location. 
- Go to WLED Controls → Config → Time & Macros to see if your time is set correctly and that your events get scheduled properly under "Time-controlled presets"

## Factory Reset Instructions

> The most secure way to factory reset and update your GLORB is using the [Web Installer](/firmware#web-installer). This will reset both the firmware and filesystem of the device. 

### Using GLORB Web Installer
- You will need a computer with a USB-C port and a Chrome/Edge web browser
- Visit the [Web Installer](/firmware#web-installer) section (bottom of the page) and follow the instructions

### Using WLED Controls
1. Go to Config → Security & Updates
2. Check the "Factory Reset" box
3. Click "Save" and wait for device restart

**Note:** This option deletes all presets, you will need to [backup and restore presets](#backup-and-restore-presets) if you want to keep them.

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