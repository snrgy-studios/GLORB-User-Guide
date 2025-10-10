---
layout: default
title: Network Settings Guide
---

<div class="back-nav">
  <a href="/">← Back to Guide</a>
</div>

# Network Settings Guide

## Overview

Your GLORB connects to your network via WiFi, allowing you to control it remotely and sync with other devices. This guide covers all the network-related settings and configurations available for your GLORB.

## WiFi Configuration

### Initial WiFi Setup

When you first set up your GLORB, you'll need to connect it to your WiFi network. Follow our [detailed setup guide](/setup) for step-by-step instructions, or use this quick overview:

1. Power on your GLORB
2. Use the SNRGY app to scan for your device bia Bluetooth
3. Select your device and go to the Modes tab to scan for WiFi networks
4. Select your network, input your password and wait for connection

### Accessing WiFi Settings

To modify your GLORB's network connection:

1. Open the SNRGY app and select your device
2. Go to Settings → WLED Controls
3. Select "Config" tab
4. Navigate to "WiFi Setup"

Here you can:
- Change WiFi network name and password
- Configure a static IP address
- Configure remote control via ESP-NOW

> **Important:** Leave the WiFi sleep settings unchanged, as they are required for Bluetooth functionality.

## Network Troubleshooting

If your GLORB won't connect to WiFi:

1. **Check Network Credentials:** Ensure the WiFi name and password are correct
2. **Signal Strength:** Move your GLORB closer to your router
3. **Network Compatibility:** Verify your network uses 2.4GHz (GLORB doesn't support 5GHz)
4. **Router Settings:** Check if your router blocks new devices or mutlicast traffic
5. **Configure Static IP:** Configure a static IP address (see below)

## Static IP Address Configuration

A static IP address is a fixed network address that doesn't change, unlike dynamic IP addresses which may change each time your GLORB connects to the network. Setting up a static IP can be beneficial for several reasons:

- **Reliable Remote Access:** If you control your GLORB through home automation systems or custom scripts, a static IP ensures the device can always be found at the same address
- **Faster Connection:** Your network doesn't need to look up the device's address each time
- **Better Sync Performance:** Other GLORBs and apps can reliably find and communicate with your device
- **Port Forwarding:** If you need to access your GLORB from outside your network, a static IP makes router port forwarding rules more reliable

We recommend using a static IP if you:
- Use Home Assistant or other smart home integrations
- Have multiple GLORBs that sync together
- Frequently access your GLORB's web interface
- Experience connection delays or dropouts

### Instructions

You can configure a static IP address for your GLORB using one of these two methods:

1. GLORB WiFi Settings:
- Open Settings → WLED Controls → Config → WiFi Setup
- Find "Static IP (leave at 0.0.0.0 for DHCP)"
- Enter your device's current IP address (found at the top of the page or in device settings)
- Example: If your device shows "192.168.1.182", enter that exact address
- Click "Save & Connect" to apply

2. Your Router Settings:
- Access your router's admin interface (check your router's manual for instructions)
- Look for "DHCP Reservation" or "Static DHCP" settings
- Add a new reservation using:
  - IP Address: Your GLORB's current IP address
  - MAC Address: Found in GLORB's Settings → About section

> **Note:** Format MAC address with colons between each pair of characters. Example: MAC "1051db2dd290" becomes "10:51:DB:2D:D2:90"

## Getting Help

If you're still experiencing network issues:
- Check our [Troubleshooting Guide](/troubleshooting)
- Visit our [Community Forum](https://discord.com/invite/hnQ5V2GNjh)
- Review [Known Issues](/known-issues) for reported problems
