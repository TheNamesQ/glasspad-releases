# GlassPad privacy policy

*Last updated 12 October 2026*

**No accounts · No ads or tracking · No GlassPad servers · Home network only by default**

GlassPad turns your phone into a touchpad and remote for display glasses and plays your own videos on them. This policy explains what the app accesses, why, and where that information goes. In short: it stays on your phone and goes only to servers you add yourself.

## Information the developer collects

None. GlassPad has no accounts, advertising, analytics or crash-reporting services, and the developer runs no servers that the app contacts. The developer does not receive, sell or share any of your data.

## Videos on your phone

With your permission, GlassPad reads the videos stored on your phone to list and play them on your glasses. If you don't grant access, you can still pick single videos with Android's own picker. When you choose to delete a video, Android asks you to confirm first.

## Notifications

If you turn on notification access, GlassPad reads your phone's notifications only to show them on your glasses and to send replies you type. Notifications are kept in memory while the app runs. They are not saved, uploaded or shared. You can turn access off at any time in Android settings.

## Servers you add

GlassPad can connect to a Jellyfin media server, SMB network shares and Home Assistant that you set up yourself. It connects only to the addresses you enter, and only to stream your media, browse your files or control the devices you choose.

- Passwords and access tokens are encrypted on the phone with a key held in its secure hardware. Your Jellyfin password is used once to sign in and is not stored.
- By default GlassPad only connects to servers on your home network or VPN (private addresses such as 192.168.x.x, `.local` names and VPN addresses such as Tailscale). Anything else is refused unless you turn on "Allow internet servers" in Settings › Privacy & network.

## Stored on your phone

GlassPad stores your settings, watch progress, a list of recently played items, cached thumbnails and a small error log in its own private storage. The error log leaves your phone only if you choose "Share diagnostics", which opens Android's share sheet so you decide where it goes. Uninstalling GlassPad deletes all of this.

## Permissions

- **Videos / storage:** list and play your videos.
- **Network:** reach the servers you add. Android requires this permission even for home-network connections.
- **Notifications:** show the "Playing on glasses" notification with playback controls.
- **Foreground service and wake lock:** keep a video playing with the phone screen dimmed.
- **Notification access** (optional, turned on by you): mirror notifications to the glasses.

## Children

GlassPad is not directed at children under 13 and does not knowingly collect information from anyone.

## Changes

If this policy changes, the updated version will be posted here with a new date.

## Contact

Questions about privacy: open an issue in this repository.
