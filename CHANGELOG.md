# Changelog

## 0.51.0

New
- **Cinema mode:** watch inside a dark cinema hall. Open it from the new Cinema button in the player.
  - Three screen sizes: the screen grows on the wall, the hall stays put
  - Room light presets: Dim, Medium, High, Bright
  - Auto dim: the lights fade to dark when the film starts (5 to 30 seconds, you pick how dark) and come back up on pause
- **Picture in picture:** shrink the playing video into a small window and keep browsing. Click it to go back to full screen.
- The app has more memory headroom for high-bitrate videos

Fixed
- Crash after marking a Jellyfin movie as watched and going back to the library

## 0.44.1

- Fixed: the app could crash when using the previous / next buttons in the player, when Up next started the next video, or when Jellyfin switched to server transcoding
- Fixed: 10-second skips right after a stream starts no longer jump back to the beginning

## 0.44.0

First public beta.

- Home screen with clock, battery and notifications, continue watching and app tiles
- Control with touchpad, air mouse or remote, plus optional edge strips for scrolling, volume and seeking
- Videos from the phone, SMB network shares and Jellyfin
- Player with subtitles, audio tracks, speed, skip intro, up next and previous / next buttons
- Home Assistant tiles on the glasses and in the player, with several Home Assistant servers supported
- Notifications on the glasses with quick replies (optional)
- Backup and restore of settings, with an optional password for secrets
- Home-network-only by default
- Settings › About: report a problem and see new versions
