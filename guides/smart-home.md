---
layout: default
title: Smart Home Integration
---

<div class="back-nav">
  <a href="/">← Back to Guide</a>
</div>

# Smart Home Integrations

> **Recommendation:** Before setting up smart home integrations, we recommend configuring a static IP address for your GLORB. This ensures reliable access and better performance with automation systems. See the [Network Settings Guide](/info/network-settings#static-ip-address-configuration) for detailed instructions.

<details markdown="1" class="expandable-section">
<summary><h2>Home Assistant</h2></summary>

Coming soon...
</details>

<details markdown="1" class="expandable-section">
<summary><h2>HomeKit</h2></summary>

### Prerequisites

- **Firmware Version:** Ensure your GLORB is running firmware release 0.14.4-GLORB.1.2 or later. If you need to update, see the [firmware update guide](/firmware).

### GLORB Setup

1. Open the SNRGY app on your mobile device
2. Navigate to **Settings** → **WLED Controls** → **Config** → **Usermods**
3. Scroll down to the **HomeKit** section
4. Check the **Enable** box
5. Press **Save**
6. Wait for your GLORB to reboot

### HomeKit Setup

1. Open the **Home** app on your iOS device
2. Tap **Add Accessory**
3. Scan the QR code displayed below or enter the setup code manually
4. Follow the on-screen instructions to complete the setup process

> **Note:** This is not a certified HomeKit implementation. During setup, you will receive a warning about this, but you can safely press **"Add Anyway"** to proceed with the setup.

<div class="homekit-image-container">
    <img src="/assets/images/homekit/homekit.jpeg" alt="HomeKit Integration">
</div>

</details>

<details markdown="1" class="expandable-section">
<summary><h2>Amazon Alexa</h2></summary>

The GLORB can be controlled via Amazon Alexa through its built-in Alexa emulation feature. You will need an Echo device for the setup process. 

Here's how to set it up:

### GLORB Setup

1. Navigate to WLED Controls → Config → Sync Interfaces
2. Find the "Alexa Voice Assistant" section
3. Enable "Emulate Alexa device"
4. Enter your desired device name in the "Alexa invocation name" field
5. Set the number of presets to 0 for best performance (see below)
6. Save the configuration
7. Restart your GLORB for changes to take effect

<div class="img-center">
    <img src="/assets/images/wled-alexa.png" alt="WLED Alexa Integration">
</div>

### Preset Control

To control GLORB presets with Alexa, you can enable preset emulation in the Alexa settings. This will create virtual devices for the first X presets in your preset list (X between 1-9), but we recommend keeping this disabled as it can be unreliable.

If you do want to use presets, you can manage their IDs and names in WLED Controls → Presets tab. Make sure to use simple, clear names that Alexa can understand. 

<div class="img-center img-narrow">
    <img src="/assets/images/wled-presets.png" alt="WLED Presets">
</div>

### Alexa Setup

Once the GLORB is configured, you'll need to add it to your Alexa app:

1. Open the Alexa app on your mobile device
2. Set up your Echo device (if not already paired)
3. Tap on "Devices" at the bottom of the screen
4. Tap the "+" (plus) icon in the top right corner
5. Select "Add Device"
6. Scroll down and select "Other" at the bottom of the list
7. Choose "WiFi"
8. Press "Discover Devices" and wait while Alexa searches
9. Your GLORB device should be discovered with the name you configured
10. Follow the on-screen instructions to complete the setup

<br>

<div class="image-grid">
    <img src="/assets/images/alexa/alexa2.png" alt="Alexa Setup Step 2">
    <img src="/assets/images/alexa/alexa3.png" alt="Alexa Setup Step 3">
</div>

### External Links

For a video walkthrough of setting up WLED devices with Alexa, check out this helpful guide by Chris Maher:

<div class="video-embed">
    <iframe src="https://www.youtube.com/embed/3WrfmZXny7c" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

</details>

<details markdown="1" class="expandable-section">
<summary><h2>Philips Hue</h2></summary>

This feature allows you to set the color of your GLORB to that of one of your Hue lights. It does NOT enable individual control of your GLORB from the Hue app.

For more information about this integration for WLED devices, visit the [WLED Knowledge Base](https://kno.wled.ge/interfaces/philips-hue/).

### GLORB Setup

1. Navigate to WLED Controls → Config → Sync Interfaces
2. Scroll down to the "Philips Hue" section
3. Enter the IP address of your Hue bridge
4. Enter the Light ID of your Hue light
   > Note: Newer versions of the Hue app do not display light IDs in the "About" section of the app anymore, to find it, the app **Hue Config Viewer** is highly recommended. It is available on the [Play Store](https://play.google.com/store/apps/details?id=com.life4hue.hueconfigviewer) and [App Store](https://apps.apple.com/app/id1145977453).
5. Press save and reboot the GLORB

<div class="img-center">
    <img src="/assets/images/wled-philips-hue.png" alt="WLED Philips Hue Integration">
</div>

</details>

<details markdown="1" class="expandable-section">
<summary><h2>Homey</h2></summary>

Coming soon...
</details>

<details markdown="1" class="expandable-section">
<summary><h2>Other Platforms</h2></summary>

Coming soon...
</details>
