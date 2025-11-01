---
layout: default
title: Firmware Updates
---

<div class="back-nav">
  <a href="/">← Back to Guide</a>
</div>

# Updating Your GLORB Firmware

## SNRGY App
<div class="platform-card">
    <h3>📱 Using the SNRGY App</h3>
    <ol>
        <li>Open the <a href="https://apps.apple.com/us/app/snrgy/id6587549578">SNRGY app</a> and select your GLORB device on the start screen</li>
        <li>Navigate to Settings (⚙️)</li>
        <li>Make sure the device is connected to WiFi (see <a href="/setup#verifying-connection">Verifying WiFi Connection</a>)</li>
        <li>Go to Firmware updates and select the latest release</li>
        <li>Select the bin file under Assets. Press Update and wait for completion</li>
    </ol>
</div>

## Web Installer
<div class="platform-card">
    <h3>🌐 Using the Web Installer</h3>
    <ul>
        <li>You will need a Chrome/Edge browser and a USB-C port
            <ul>
                <li>Make sure your computer is plugged into a power source for best results</li>
            </ul>
        </li>
        <li>Visit the <a href="https://snrgy-studios.github.io/GLORB-WebInstaller/">GLORB Web Installer</a> and follow the instructions
            <ul>
                <li>See our <a href="#" onclick="openVideoModal(); return false;">video guide</a> for a step-by-step walkthrough</li>
            </ul>
        </li>
    </ul>
</div>

<div class="modal" id="videoModal">
    <div class="modal-content">
        <button class="close-modal" onclick="closeVideoModal()">×</button>
        <video controls>
            <source src="/assets/videos/glorb-web-installer.mp4" type="video/mp4">
            Your browser does not support the video tag.
        </video>
    </div>
</div>

<script>
function openVideoModal() {
    document.getElementById('videoModal').classList.add('active');
}

function closeVideoModal() {
    const modal = document.getElementById('videoModal');
    const video = modal.querySelector('video');
    video.pause();
    modal.classList.remove('active');
}

// Close modal when clicking outside
document.getElementById('videoModal').addEventListener('click', function(e) {
    if (e.target === this) closeVideoModal();
});
</script>
