# Steam Link for OpenXR Android

This is a mirror of the Steam Link APK for standalone Android VR headsets that support OpenXR. It works like [Meta Quest application](https://www.meta.com/experiences/steam-link/5841245619310585/), but is [developed by Valve](https://store.steampowered.com/news/app/250820/view/514096230384533859) to "allow users of unsupported headsets to explore compatibility and available features," and [may work](https://bsky.app/profile/corbin.io/post/3mzeomdpln22t) on Android XR devices.

**[Download APK from SteamVR Public Channel](https://github.com/corbindavenport/steam-link-vr/raw/refs/heads/main/steamlinkvr-release-stable.apk)**

**[Download APK from SteamVR Beta Channel](https://github.com/corbindavenport/steam-link-vr/raw/refs/heads/main/steamlinkvr-release-beta.apk)**

The APKs are copied from the SteamVR package on Steam using [DepotDownloader](https://github.com/steamre/depotdownloader), and checked every 24 hours with GitHub Actions.

If you would like to get the APKs on your own, see the below instructions.

### Get the APK from Steam on a PC

This is the official method for obtaining the APKs.

1. Install [SteamVR](https://store.steampowered.com/app/250820/SteamVR/) in Steam, if you haven't already.
2. Right-click SteamVR in Steam's games list and Select Properties.
3. Click Installed Files > Browse, then navigate to this path: `drivers/vrlink/resources/android-steamlinkvr-release.apk`

If you want the APK from the beta channel of SteamVR, switch to it from the "Game Versions & Betas" tab of the Properties window.

### Get the APK with DepotDownloader

If you can't install Steam or SteamVR, like on a Mac, you can use [DepotDownloader](https://github.com/steamre/depotdownloader). After it's installed, open a Terminal and switch to where you want the downloaded files, like your Desktop folder:

```shell
cd ~/Desktop
```

Then run this command to download the ["OpenVR Content" depot package](https://steamdb.info/depot/250824/) from Steam:

```shell
DepotDownloader -app 250820 -depot 250824 -dir "download"
```

If you have an authentication error, try adding `-qr` to the command to log in with Steam Guard.

The APK will be located at this path:

```
download/drivers/vrlink/resources/android-steamlinkvr-release.apk
```

If you want the APK from the beta channel of SteamVR, run the DepotDownloader command with `-branch "beta"`.