---
layout: default
title: Audio Reactivity Guide
---

<div class="back-nav">
  <a href="/">← Back to Guide</a>
</div>

# Audio Reactivity Guide

## Overview
Your GLORB has a built-in microphone that allows it to react to sound in real-time. This feature works with specific animations that are designed to be audio-reactive.

Currently, these GLORB animations support audio reactivity:
- Colorwaves
- Swirl

We're actively developing more audio-reactive animations that will be available in future updates!

> **Note:** We're aware of an issue where the Swirl effect occasionally stops responding to audio. As a temporary solution, we've added a "regular" non-reactive Swirl mode in the [latest firmware version](/firmware). A full fix is coming soon.

## Additional Audio-Reactive Effects

The WLED interface (see [WLED Controls Guide](/info/wled-controls)) offers many more audio-reactive effects beyond the GLORB-optimized ones. You can find these by:
1. Looking for the musical note (♪) icon next to effect names
2. Using the audio-reactive filter in the effects list

While these effects work, they haven't been specifically optimized for GLORB's spherical shape yet.

## Adjusting Audio Settings

If the audio reactivity isn't working as expected, you can go to **Settings → WLED Controls → Config → Usermods → AudioReactive** and adjust the following settings as needed. 

> **Note:** These settings affect all audio-reactive animations globally, but individual animations may interpret and use these settings differently. 

### Config

**Squelch** – Filters out background noise (recommended: 4–6).
- Lower numbers make the mic more sensitive.
- Higher numbers ignore quiet sounds.

**Gain** – Boosts the incoming audio signal (recommended: 40–60).
- Increase if effects look too weak.
- Decrease if the lights “max out” too easily.

**AGC (Automatic Gain Control)** – Keeps volume levels balanced.
- Leave on Normal for most situations.

### Dynamics

**Limiter** – Prevents loud sounds from overwhelming the effects.
- Keep this switched ON.

**Rise** – How fast the lights respond to new sounds (recommended: 50–100 ms).
- Lower = snappier
- Higher = smoother.

**Fall** – How long the lights take to fade after a sound (recommended: 800–1500 ms).
- Lower = quick fade
- Higher = lingering trails.

### Frequency

**Scale** – Controls how frequencies are balanced.
- Square Root (Energy) is best for natural, balanced visuals.

### Quick Fix Tips

- If nothing reacts, lower Squelch or raise Gain.
- If the lights stay maxed out, lower Gain or raise Squelch.
- If effects look too jittery, increase Rise and Fall.
- If they lag too much, decrease Fall.

## Audio Sync Feature

You can synchronize multiple GLORBs to react to the same audio source! Only one GLORB needs to have its microphone active - it will send the audio data to other GLORBs on your network.

### Setting Up Audio Sync

1. On the GLORB that will capture audio (the sender):
   - Go to WLED Controls → Config → Usermods
   - Find the AudioReactive section and set Sync mode to "Send"
   - Save settings and reboot the GLORB

2. On other GLORBs (the receivers):
   - Go to WLED Controls → Config → Usermods
   - Find the AudioReactive section and set Sync mode to "Receive"
   - Save settings and reboot the GLORB(s)

> **Note:** Audio sync requires your network to support multicast. If sync isn't working, check your router settings or try placing GLORBs closer to your WiFi router.
