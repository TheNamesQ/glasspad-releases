<p align="center">
  <img src="assets/banner.png" alt="GlassPad" width="720">
</p>

# GlassPad (beta)

**Your phone is the remote. Your glasses are the screen.**

GlassPad is a free Android app for VITURE display glasses. It shows a big-screen home and video player on the glasses, and turns your phone into a touchpad, air mouse or simple remote to control it.

> **Beta.** This is an early build for people who like trying new things. Expect rough edges, and please report them. See [Feedback](#feedback).

**[⬇ Download the latest APK](../../releases/latest)**

---

## What it does

- **Three ways to control it:** touchpad (like a laptop), air mouse (point the phone), or remote (taps and swipes for play, seek and volume).
- **Plays your videos** from the phone, SMB network shares (NAS or computer) and Jellyfin, with continue watching, subtitles, audio tracks, playback speed and skip intro.
- **Phone screen dims** while the video keeps playing on the glasses, to save battery.
- **Home Assistant tiles** in the player: switch lights and scenes without leaving the video.
- **Notifications on the glasses** (optional), with quick replies.
- **Backup and restore** of all settings to one file, with an optional password for saved passwords and tokens.

## Requirements

- Android 10 or newer.
- A phone that sends video over USB-C (DisplayPort Alt Mode). Most recent Pixels and Samsung Galaxy S phones do. Many budget phones don't.
- VITURE glasses. Other USB-C display glasses that act as a plain external screen should work too, but are untested.

## Install

1. On your phone, open the **[latest release](../../releases/latest)** and download `GlassPad-…-beta.apk`.
2. Open the file. If Android asks, allow your browser or file manager to **install unknown apps**.
3. Open GlassPad, follow the short welcome steps, then plug in the glasses.

**Updating:** install the new APK over the old one. Your settings are kept.

**Get notified of updates:** add this repository to [Obtainium](https://github.com/ImranR98/Obtainium) (paste the URL of this page). It will tell you when a new version is out.

### Verify the download (optional)

Each release has a `.sha256` file with the APK's checksum. All builds are signed with the same key:

```
SHA-256 signing certificate:
16:4B:A8:28:EF:E8:32:6F:6F:A9:80:0C:52:15:94:C0:41:C5:BE:95:D4:04:05:5C:2A:00:E2:E4:A3:F5:94:19
```

You can check it with `apksigner verify --print-certs GlassPad-…-beta.apk`, or with apps like *App Manager*.

## Permissions, and why

| Permission | Why |
|---|---|
| Videos | List and play the videos on your phone. Optional: without it you can still pick single videos with Android's picker. |
| Network | Reach the servers you add (Jellyfin, SMB, Home Assistant). |
| Notifications | The "Playing on glasses" notification with playback controls. |
| Notification access *(optional, off until you turn it on)* | Show your phone's notifications on the glasses and send replies. |
| Foreground service, wake lock | Keep the video playing while the phone screen is dimmed. |

## Privacy

- No accounts, ads, analytics or tracking. GlassPad does not contact any server run by the developer, and has no idea how many people use it.
- By default it only connects to servers on your **home network or VPN** (for example 192.168.x.x, `.local` names, Tailscale). Internet servers have to be allowed in Settings › Privacy & network.
- Passwords and tokens are encrypted on the phone.

Full policy: [PRIVACY.md](PRIVACY.md)

## Feedback

- **Found a bug?** [Open an issue](../../issues/new/choose). In GlassPad, Settings › About › **Share diagnostics** creates a short report (no passwords or tokens) you can paste in.
- **Have an idea?** Open a feature request the same way.

What's new in each version: [CHANGELOG.md](CHANGELOG.md)

---

GlassPad is an independent app. It is not made by, affiliated with or endorsed by VITURE. VITURE is a trademark of its owner.

The app is free to use and is provided as is, without warranty.
