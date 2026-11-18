# Ganymede Smart Client — Mobile

An Android phone client for [Ganymede](https://github.com/zibbp/ganymede), the Twitch VOD and
live stream archiver. Browse your channels and archived videos, keep playing in the background,
and save videos to the phone to watch offline.

This repository only hosts the release builds. Grab the latest APK from
[Releases](../../releases/latest).

## Install

Open this link on the phone, or scan the QR code:

**[ganymede-smart-client-mobile.apk](https://github.com/Nargarnd/ganymede-smart-client-mobile/releases/latest/download/ganymede-smart-client-mobile.apk)**

<img src="qr.png" alt="QR code for the latest APK" width="200">

1. The browser downloads the APK. Open it from the download notification.
2. Android asks you to allow your browser to install unknown apps. Allow it, go back and choose
   **Install**.
3. Open the app, enter your Ganymede server address (for example `http://192.168.1.10:4800`) and
   sign in.

That link always points to the newest release, so it never changes. Requires Android 7.1.1 or
newer.

## Updates

From version 0.1.2 on, the app checks this repository for new releases. Go to
**Settings → Check for updates**, or accept the prompt when it appears on startup.

The first time, Android will ask you to allow **Ganymede** to install unknown apps.

Updates install over the existing app and keep your server, sign-in and downloaded videos.

## Verifying a download

Each release lists the SHA-256 of its APK. You can check it with any hash app, or on a PC:

```powershell
Get-FileHash .\ganymede-smart-client-mobile.apk -Algorithm SHA256
```

## Upgrading from a build older than 0.1.2

Builds before 0.1.2 used a different application id, so 0.1.2 installs as a separate app.
Videos saved for offline viewing in the old app stay there and are deleted when you uninstall
it, so download them again in the new app before removing the old one.
