---
layout: default
title: Release Notes
---

<div class="back-nav">
  <a href="/">← Back to Guide</a>
</div>

# GLORB Firmware Releases

## Release GLORB 0.14.4-1.3

Released: 2025-12-23

Firmware for the [GLORB](https://glorb.me/) smart lamp 

By SNRGY Studios AB, Gothenburg, Sweden

### 🌟 What's New

- Refactored BLE usermod for more stable Bluetooth request handling and reconnects
- Added new animations: Pulse Wave, Gradient Flow and Fold
- Added sound reactive support: Colorloop and Running

### ⚡ Improvements

- Optimized memory usage to lower RAM consumption and reduce slowdowns
- General stability fixes and optimizations; this release lays groundwork for further performance tuning 

### ⚠️ Important Notes

- DO NOT install other custom firmware or standard WLED builds unless you are certain of the correct board configuration. Incorrect configurations during firmware updates can brick your device
- If experiencing issues, try restarting the device (power cycle) and/or the mobile app

### 🙏 Credits

* Thanks to @novacom34 and @vinegod (Novacom Studios) for their work on the BLE module and the iOS app integration

*This firmware is based on the [WLED project](https://kno.wled.ge/), an open-source solution for controlling LEDs with ESP microcontrollers. We extend our gratitude to the WLED community for their outstanding work.*

---

## Release GLORB 0.14.4-1.2

Released: 2025-11-01

Firmware for the [GLORB](https://glorb.me/) smart lamp 

By SNRGY Studios AB, Gothenburg, Sweden

### 🌟 What's New

- Added HomeKit support via the HomeSpan library (see our [User Guide](https://user-guide.glorb.me/guides/smart-home) for setup instructions)

### ⚡ Improvements

- Fixed issues with color calibration (gamma correction)
- Updated settings after firmware updates 
- Improved default configurations
- Corrected version numbers, server name and repository links 
- General bug fixes

### ⚠️ Important Notes

- DO NOT install other custom firmware or standard WLED builds unless you are certain of the correct board configuration. Incorrect configurations during firmware updates can brick your device
- If experiencing issues, try restarting the device (power cycle) and/or the mobile app

### 🙏 Credits

* Thanks to @novacom34 and @vinegod (Novacom Studios) for their work on the HomeKit module and the iOS app integration

*This firmware is based on the [WLED project](https://kno.wled.ge/), an open-source solution for controlling LEDs with ESP microcontrollers. We extend our gratitude to the WLED community for their outstanding work.*

---

## Release GLORB 0.14.4-1.1

Released: 2024-12-20

Firmware for the [GLORB](https://glorb.me/) smart lamp 

By SNRGY Studios AB, Gothenburg, Sweden

### 🌟 What's New

- Custom coordinate mappings and util functions
- Custom Wave effect
- GLORB filter option in the WLED interface
- Enable/disable feature for the GLORB and Bluetooth modules

### ⚡ Improvements

- Fixed crashes on preset handling using Bluetooth
- Fixed flickering on preset handling, OTA updates and factory reset
- Updated Frizzles, Black Hole, Swirl and Tartan effects

### ⚠️ Important Notes

- DO NOT install other custom firmware or standard WLED builds unless you are certain of the correct board configuration. Incorrect configurations during firmware updates can brick your device
- If experiencing issues, try restarting the device (power cycle) and/or the mobile app

### 🙏 Credits

* Thanks to @novacom34 and @vinegod (Novacom Studios) for their work on the BLE module and the iOS app integration
* Thanks to all our beta testers for their valuable feedback

*This firmware is based on the [WLED project](https://kno.wled.ge/), an open-source solution for controlling LEDs with ESP microcontrollers. We extend our gratitude to the WLED community for their outstanding work.*

---

## Release GLORB 0.14.4-1.0

Released: 2024-10-08

Firmware for the [GLORB](https://glorb.me/) smart lamp 

By SNRGY Studios AB, Gothenburg, Sweden

### 🌟 What's New

- Integration of core WLED features (v0.14.4)
- GLORB module with customised WLED effects and default configurations
- Bluetooth control via lampOS module and SNRGY mobile app

### ⏳ Known Issues

* LED flickering may occur when accessing the device via Bluetooth
* Crashes may occur on preset deletion and handling using Bluetooth

### ⚠️ Important Notes

- DO NOT install other custom firmware or standard WLED builds unless you are certain of the correct board configuration. Incorrect configurations during firmware updates can brick your device
- If experiencing issues, try restarting the device (power cycle) and/or the mobile app

### 🙏 Credits

* Thanks to @novacom34 and @vinegod (Novacom Studios) for their work on the BLE module and the iOS app integration
* Thanks to all our beta testers for their valuable feedback

*This firmware is based on the [WLED project](https://kno.wled.ge/), an open-source solution for controlling LEDs with ESP microcontrollers. We extend our gratitude to the WLED community for their outstanding work.*