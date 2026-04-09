---
layout: default
title: Initial Setup
---

<div class="back-nav">
  <a href="/">← Back to Guide</a>
</div>

# Setting Up Your GLORB

## First-Time WiFi Connection

### Bluetooth
<div class="platform-card">
    <h3>📱 Using SNRGY App</h3>
    <ol>
        <li>Open the <a href="https://apps.apple.com/us/app/snrgy/id6587549578">SNRGY app</a> and select your device on the start screen</li>
        <li>Go to Modes → Connect to WiFi</li>
        <li>Wait for the WiFi scan to complete</li>
        <li>Choose your network and enter your password</li>
        <li>Wait for connection (see <a href="#verifying-connection">Verifying Connection</a>)</li>
    </ol>
</div>

### GLORB Access Point
<div class="platform-card">
    <h3>🤖 Using WLED</h3>
    <ol>
        <li>When powered on, your GLORB creates its own WiFi access point (AP)</li>
        <li>Connect to <code>WLED-AP</code> (or <code>GLORB-AP</code>) in your WiFi list
            <ul>
                <li>Password: <code>wled1234</code> (or <code>glorb1234</code>) if prompted</li>
            </ul>
            <div class="img-center"><img src="/assets/images/wled-ap.png" alt="WLED Access Point"></div>
        </li>
        <li>Click "WiFi Settings" in the popup that appears
            <ul>
                <li>Go to <code>http://4.3.2.1</code> in a browser if not automatically redirected</li>
            </ul>
            <div class="img-center"><img src="/assets/images/wled-welcome.png" alt="WLED Welcome Screen"></div>
        </li>
        <li>Enter your network name (SSID) and password under "Connect to existing network". Press "Save & Connect" and go back to your home network.
            <ul>
                <li>NOTE: Leave everything else as is, especially do not touch the WiFi sleep settings!</li>
            </ul>
            <div class="img-center"><img src="/assets/images/wled-wifi.png" alt="WLED WiFi Settings"></div>
        </li>
        <li>Wait for connection (see <a href="#verifying-connection">Verifying Connection</a>)</li>
    </ol>
</div>

## Verifying Connection

<div class="platform-card">
    <h3>📱 Using SNRGY App</h3>
    <ol>
        <li>Restart the SNRGY app</li>
        <li>Select your device and go to Settings (⚙️)</li>
        <li>Check for an IP address in info section
            <ul>
                <li>IP address listed → successful connection</li>
                <li>No IP address → retry connection process</li>
            </ul>
        </li>
    </ol>
</div>

<div class="platform-card">
    <h3>🤖 Using WLED Native App</h3>
    <ol>
        <li>Your GLORB device should appear in the <a href="https://play.google.com/store/apps/details?id=ca.cgagnier.wlednativeandroid&hl=en">WLED Native app</a> with a listed IP address</li>
        <li>You can also access it through your browser at <code>http://[IP_ADDRESS]</code></li>
    </ol>
</div>

## Troubleshooting Connection Issues

<div class="platform-card">
    <h3>⚠️ Common Issues</h3>
    <ul>
        <li>Make sure you have Bluetooth enabled (iOS)</li>
        <li>Try restarting your GLORB and/or the app</li>
        <li>Check that your WiFi password is correct</li>
        <li>Ensure your network is 2.4GHz (5GHz networks are not supported)</li>
        <li>See our full <a href="/troubleshooting#connection-issues">troubleshooting guide</a></li>
    </ul>
</div> 