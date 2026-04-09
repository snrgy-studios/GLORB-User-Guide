---
layout: default
title: Known Issues
---

<div class="back-nav">
  <a href="/">← Back to Guide</a>
</div>

# Known Issues

This page lists currently known issues with GLORB hardware, firmware, and apps. For solutions to common problems, see our [Troubleshooting Guide](/troubleshooting).

## Important Notice

Before reporting any issues, please ensure you are running the latest versions:

### Check Your Versions
1. **GLORB Firmware**: [Update to latest version](/firmware)
2. **Mobile Apps**: See [Quick Links](/#quick-links) for app downloads

See our [Release Notes](/releases) for details on the latest improvements and fixes.

## Hardware Issues

### Loose Panels
- Caused during shipping
- See the [Repair Guide](/guides/repair#how-to-fix-a-loose-panel) for instructions on how to reattach panels
- Inform us on our [support email](mailto:support@glorb.me)

### Dead LEDs
- Can be caused by faulty LEDs or assembly error
- Contact us on our [support email](mailto:support@glorb.me)

## Firmware

### Random Crashes and Reboots
- GLORB may crash and reboot randomly or during heavy load (e.g. frequent app requests)
- This is a known issue caused by heap memory drop and fragmentation. A fix is planned for the next firmware update
- **Workaround**: If the reboots are disturbing, you can set the default boot behavior to start in an off state:
  - **iOS**: Available directly in the **Settings** tab
  - **Android**: Go to **WLED Controls** > **Config** > **LED Preferences** and disable **Turn LEDs on after power up/reboot** (see [WLED Controls](/info/wled-controls#led-preferences))

## Mobile App

### SNRGY App (Android)
- See [Android App Guide](/info/android-app) for current features and limitations

## Reporting Issues
Found a bug not listed here? Help us improve:
- Join our [Discord Community](https://discord.com/invite/hnQ5V2GNjh)
- Email [support@glorb.me](mailto:support@glorb.me)
