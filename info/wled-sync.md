---
layout: default
title: WLED Sync Guide
---

<div class="back-nav">
  <a href="{{ site.baseurl }}/">← Back to Guide</a>
</div>

# Understanding WLED Sync

The sync feature allows multiple GLORBs on the same network to synchronize their colors and effects. When enabled, changes made to one GLORB automatically apply to all other GLORBs on the network.

> **Note:** Sync only affects triggered state changes - patterns still generate independently on each device.

## How It Works

GLORBs communicate using UDP messages to share updates about:
- Current colors and effects
- Brightness levels
- Effect settings

## Sync Settings

Find more detailed sync settings in Settings → WLED Controls → Config → Sync Interfaces. Remember to restart your GLORB after making any changes.

### Sync Groups

Create independent clusters of GLORBs using sync groups. Assign each device a group number (1-8) to control which GLORBs sync together.

Each device can be configured as:
- **Send & Receive:** Broadcasts and responds to updates (default)
- **Receive Only:** Only listens for updates
- **Send Only:** Only broadcasts changes

### Important Settings
- **Send notifications on direct change:** Controls default sync state after reboot
- **UDP packet retransmissions:** Adjust how many packets are sent to the other devices
  - Higher (3-5): More reliable but uses more bandwidth
  - Lower (0-2): Faster but risk of packets getting lost 

<div style="text-align: center;">
    <img src="{{ site.baseurl }}/assets/images/sync_setup.jpeg" alt="WLED Sync Settings" style="width: 80%; max-width: 500px;">
</div>

## Troubleshooting

If sync isn't working properly:
- Confirm all devices share the same network
- Try toggling sync off and on
- Restart the app and devices
- Increase UDP retransmissions if sync is unreliable
- Verify router supports network broadcast traffic

> **Remember:** Stable network connections provide the best sync performance.