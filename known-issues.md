---
layout: default
title: Known Issues
---

<div class="back-nav">
  <a href="{{ site.baseurl }}/">← Back to Guide</a>
</div>

# Known Issues

This page lists currently known issues with GLORB hardware, firmware, and apps. For solutions to common problems, see our [Troubleshooting Guide]({{ site.baseurl }}/troubleshooting).

## Important Notice

Before reporting any issues, please ensure you are running the latest versions:

### Check Your Versions
1. **GLORB Firmware**: [Update to latest version]({{ site.baseurl }}/firmware)
2. **Mobile Apps**: See [Quick Links]({{ site.baseurl }}/#quick-links) for app downloads

See our [Release Notes]({{ site.baseurl }}/releases) for details on the latest improvements and fixes.

## GLORB Hardware

### Physical Issues
- Loose panels
  - Caused during shipping
  - Check <a href="#" onclick="openVideoModal(); return false;">instruction video</a> on how to reattach panels
  - Inform us on our [support email](mailto:support@glorb.me)

<div class="modal phone-video" id="videoModal">
    <div class="modal-content">
        <button class="close-modal" onclick="closeVideoModal()">×</button>
        <video controls>
            <source src="{{ site.baseurl }}/assets/videos/panel-fix.mov" type="video/mp4">
            Your browser does not support the video tag. 
            <a href="{{ site.baseurl }}/assets/videos/panel-fix.mov">Download the video</a>
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

### Electronics Issues
- Faulty power supply
  - Could cause boot issues
  - Try another power supply with the same specs (5V/3A)
  - Contact us on our [support email](mailto:support@glorb.me)
- Dead LEDs
  - Can be caused by faulty LEDs or assembly error
  - Contact us on our [support email](mailto:support@glorb.me)

## GLORB Firmware

### Animations
- Swirl effect stops running in sound reactive mode

## Mobile App

### SNRGY App (iOS)
- Warranty registration is not fully set up yet
- App doesn't display the correct firmware version after update
- Issue with auto-updating device/control screen on state changes
- Issue with setting boot preset using WiFi

## Reporting Issues
Found a bug not listed here? Help us improve:
- Join our [Discord Community](https://discord.com/invite/hnQ5V2GNjh)
- Email [support@glorb.me](mailto:support@glorb.me)