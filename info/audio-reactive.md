---
layout: default
title: Audio Reactivity Guide
---

<div class="back-nav">
  <a href="{{ site.baseurl }}/">← Back to Guide</a>
</div>

# Audio Reactivity Guide

## Overview
Your GLORB has a built-in microphone that allows it to react to sound in real-time. This feature works with specific animations that are designed to be audio-reactive.

Currently, these GLORB animations support audio reactivity:
- Colorwaves
- Swirl

We're actively developing more audio-reactive animations that will be available in future updates!

> **Note:** We're aware of an issue where the Swirl effect occasionally stops responding to audio. As a temporary solution, we've added a "regular" non-reactive Swirl mode in the [latest firmware version]({{ site.baseurl }}/firmware). A full fix is coming soon.

## Additional Audio-Reactive Effects

The WLED interface (see [WLED Controls Guide]({{ site.baseurl }}/info/wled-controls)) offers many more audio-reactive effects beyond the GLORB-optimized ones. You can find these by:
1. Looking for the musical note (♪) icon next to effect names
2. Using the audio-reactive filter in the effects list

While these effects work, they haven't been specifically optimized for GLORB's spherical shape yet.

### Adjusting Audio Sensitivity

If the audio reactivity isn't working as expected, you can adjust these settings:
1. Go to Config → Usermods → AudioReactive
2. Adjust these values:
   - Squelch: Controls the minimum volume needed to trigger effects
   - Gain: Controls how strongly the GLORB responds to sound
