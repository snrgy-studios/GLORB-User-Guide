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

## Hardware Issues

### Physical Issues
Loose panels
- Caused during shipping
- Check <a href="#" onclick="openVideoModal(); return false;">instruction video</a> on how to reattach panels
- Inform us on our [support email](mailto:support@glorb.me)

### Electronics Issues
Faulty power supply
- Could cause boot issues
- Try another 5V/3A power supply
- Contact us on our [support email](mailto:support@glorb.me)

Dead LEDs
- Can be caused by faulty LEDs or assembly error
- For a DIY fix to misaligned LEDs, you might be able to open the panel and push it back into place using this <a href="#" onclick="openVideoModal(); return false;">panel video</a>
- Either way, contact us on our [support email](mailto:support@glorb.me)

## Firmware Issues

### Animations
- Swirl effect stops running in sound reactive mode (sound reactive by default)

## Mobile App

### SNRGY App (iOS)
- Warranty registration and display is not fully set up yet. We will get this sorted soon.
- App doesn't display the correct firmware version after update. If no error is shown, the update is successful.
- Issue with auto-updating screens on state changes. 
  - For now, restart the app if encountering issues. 
- Issue with setting boot preset (iOS). 
  - For now, go to WLED Controls and note the ID of the preset you want to use as boot preset. Then continue to Config → LED Preferences → "Apply preset [ID] at boot". 
  - Set your preset ID and save the page. If this generates an error, change Maximum Current from 0 to 5000 before saving. 

## Reporting Issues
Found a bug not listed here? Help us improve:
- Join our [Discord Community](https://discord.com/invite/hnQ5V2GNjh)
- Email [support@glorb.me](mailto:support@glorb.me)

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