---
layout: default
title: Firmware Updates
---

<div class="back-nav">
  <a href="{{ site.baseurl }}/">← Back to Guide</a>
</div>

# Updating Your GLORB Firmware

## iOS Users
<div class="platform-card">
    <h3>📱 Using the SNRGY App</h3>
    <ol>
        <li>Open the <a href="https://apps.apple.com/us/app/snrgy/id6587549578">SNRGY app</a> and select your GLORB device on the start screen</li>
        <li>Navigate to Settings (⚙️)</li>
        <li>Make sure the device is connected to WiFi (see <a href="{{ site.baseurl }}/setup#verifying-connection">Verifying WiFi Connection</a>)</li>
        <li>Go to Firmware updates and select the latest release</li>
        <li>Select the bin file under Assets. Press Update and wait for completion</li>
    </ol>
</div>

## Android Users
<div class="platform-card">
    <h3>🤖 Using WLED</h3>
    <ol>
        <li>Download the latest firmware release: <a href="{{ site.baseurl }}/releases/GLORB_0.14.4-1.1.bin">GLORB_0.14.4-1.1.bin</a></li>
        <li>Use either:
            <ul>
                <li>WLED Native app (mobile) - <a href="https://play.google.com/store/apps/details?id=ca.cgagnier.wlednativeandroid&hl=en">Download</a></li>
                <li>WLED Web interface (desktop) - <code>http://[your-device-ip]</code></li>
            </ul>
        </li>
        <li>Navigate to Settings → Security & Updates</li>
        <li>Under "Manual OTA Update", click "Browse"</li>
        <li>Select the downloaded firmware file</li>
        <li>Click "Update" and wait for completion</li>
    </ol>
</div>

## Web Installer
<div class="platform-card">
    <h3>🌐 Using Web Installer</h3>
    <ol>
        <li>You need a Chrome/Edge browser and a USB-C port</li>
        <li>Visit the <a href="https://snrgy-studios.github.io/GLORB-WebInstaller/">GLORB Web Installer</a> and follow the instructions</li>
    </ol>
</div>
