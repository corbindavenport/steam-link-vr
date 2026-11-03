# steam-link-vr

This is a mirror of the Steam Link APK for generic OpenXR Android headsets, since the [official download](https://media.steampowered.com/steamlink/android/latest/steamlink-android.apk) is only for the phone and tablet version. A GitHub Action fetches the latest version every 24 hours.

**[Download APK from SteamVR Public Channel](https://github.com/corbindavenport/steam-link-vr/raw/refs/heads/main/steamlinkvr-release-stable.apk)**

**[Download APK from SteamvR Beta Channel](https://github.com/corbindavenport/steam-link-vr/raw/refs/heads/main/steamlinkvr-release-beta.apk)**

You can also get the APK from the source through one of the below methods.

### Get the APK from Steam on a PC

This is the official method for obtaining the VR APK.

1. Install [SteamVR](https://store.steampowered.com/app/250820/SteamVR/) in Steam, if you haven't already.
2. Right-click SteamVR in Steam's games list and Select Properties.
3. Click Installed Files > Browse, then navigate to this path: `drivers/vrlink/resources/android-steamlinkvr-release.apk`

### Get the APK with DepotDownloader

If you can't install Steam or SteamVR, like on a Mac, you can use [DepotDownloader](https://github.com/steamre/depotdownloader). After it's installed, open a Terminal and switch to where you want the downloaded files, like your Desktop folder:

```shell
cd ~/Desktop
```

Then run this command to download the ["OpenVR Content" depot package](https://steamdb.info/depot/250824/) from Steam:

```
DepotDownloader -app 250820 -depot 250824
```

If you have an authentication error, try adding `-qr` to the command to log in with Steam Guard.

The APK will be located at this path:

```
depots/250824/25998080/drivers/vrlink/resources/android-steamlinkvr-release.apk
```