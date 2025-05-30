---
layout: default
title: Smart Home Integration
---

<div class="back-nav">
  <a href="{{ site.baseurl }}/">← Back to Guide</a>
</div>

# Smart Home Integrations

> **Note:** This guide is under development. We'll be adding detailed setup instructions for each platform soon.

<details markdown="1" class="expandable-section">
<summary><h2>Home Assistant</h2></summary>

Coming soon...
</details>

<details markdown="1" class="expandable-section">
<summary><h2>Amazon Alexa</h2></summary>

The GLORB can be controlled via Amazon Alexa through its built-in Alexa emulation feature. Here's how to set it up:

### GLORB Setup

1. Navigate to WLED Controls → Config → Sync Interfaces
2. Find the "Alexa Voice Assistant" section
3. Enable "Emulate Alexa device"
4. Enter your desired device name in the "Alexa invocation name" field
5. (Optional) Adjust the number of presets you want to emulate (see next section)
6. Save the configuration
7. Restart your GLORB for changes to take effect

![WLED Alexa Integration]({{ site.baseurl }}/assets/images/wled-alexa.png){:width="80%" style="display: block; margin: 0 auto;"}

### Preset Control

You can control GLORB presets through Alexa by adjusting the "**Also emulate devices to call the first ___ presets**" setting. When you increase this number, Alexa will create separate virtual devices for each of the first X presets in the list, using the current preset name as invocation name. Make sure to use a name that Alexa can recognise easily. 

You can view and edit your preset names and IDs in WLED Controls → Presets tab. Presets are not editable in the SNRGY app yet. 

![WLED Presets]({{ site.baseurl }}/assets/images/wled-presets.png){:width="50%" style="display: block; margin: 0 auto;"}

### Alexa Setup

Once the GLORB is configured, you'll need to add it to your Alexa app:

1. Open the Alexa app on your mobile device
2. Tap on "Devices" at the bottom of the screen
3. Tap the "+" (plus) icon in the top right corner
4. Select "Add Device"
5. Scroll down and select "Other" at the bottom of the list
6. Choose "WiFi"
7. Press "Discover Devices" and wait while Alexa searches
8. Your GLORB device should be discovered with the name you configured
9. Follow the on-screen instructions to complete the setup

<br>

<div class="image-grid" style="display: flex; flex-direction: column; align-items: center;">
    <div class="grid-row" style="margin-bottom: 10px; display: flex; justify-content: center;">
        <img src="{{ site.baseurl }}/assets/images/alexa/alexa1.png" alt="Alexa Setup Step 1" style="width: 45%; margin-right: 2%; object-fit: contain;">
        <img src="{{ site.baseurl }}/assets/images/alexa/alexa2.png" alt="Alexa Setup Step 2" style="width: 45%; object-fit: contain;">
    </div>
    <div class="grid-row" style="margin-bottom: 10px; display: flex; justify-content: center;">
        <img src="{{ site.baseurl }}/assets/images/alexa/alexa3.png" alt="Alexa Setup Step 3" style="width: 45%; margin-right: 2%; object-fit: contain;">
        <img src="{{ site.baseurl }}/assets/images/alexa/alexa4.png" alt="Alexa Setup Step 4" style="width: 45%; object-fit: contain;">
    </div>
    <div class="grid-row" style="margin-bottom: 10px; display: flex; justify-content: center;">
        <img src="{{ site.baseurl }}/assets/images/alexa/alexa5.png" alt="Alexa Setup Step 5" style="width: 45%; margin-right: 2%; object-fit: contain;">
        <img src="{{ site.baseurl }}/assets/images/alexa/alexa6.png" alt="Alexa Setup Step 6" style="width: 45%; object-fit: contain;">
    </div>
    <div class="grid-row" style="margin-bottom: 10px; display: flex; justify-content: center;">
        <img src="{{ site.baseurl }}/assets/images/alexa/alexa7.png" alt="Alexa Setup Step 7" style="width: 45%; margin-right: 2%; object-fit: contain;">
        <img src="{{ site.baseurl }}/assets/images/alexa/alexa8.png" alt="Alexa Setup Step 8" style="width: 45%; object-fit: contain;">
    </div>
</div>

### External Links

For a video walkthrough of setting up WLED devices with Alexa, check out this helpful guide by Chris Maher:

<div class="video-container" style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; margin-bottom: 20px;">
    <iframe style="position: absolute; top: 0; left: 0; width: 80%; height: 100%; left: 50%; transform: translateX(-50%);" src="https://www.youtube.com/embed/3WrfmZXny7c" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

</details>

<details markdown="1" class="expandable-section">
<summary><h2>Philips Hue</h2></summary>

Coming soon...
</details>

<details markdown="1" class="expandable-section">
<summary><h2>Homey</h2></summary>

Coming soon...
</details>

<details markdown="1" class="expandable-section">
<summary><h2>Other Platforms</h2></summary>

Coming soon...
</details>

<style>
.expandable-section summary {
    cursor: pointer;
    transition: background-color 0.3s ease;
    padding: 10px;
    border-radius: 5px;
}

.expandable-section summary:hover {
    background-color: #1a1a1a;
}

.expandable-section summary h2 {
    margin: 0;
}
</style>