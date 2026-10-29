# GOLAN Browser 1.2.18

[العربية](README.ar.md)
[Usage and cost/PC FAQ](GUIDE.md)


The complete source ZIP, unchanged APK and SHA-256 checksums are [release assets](https://github.com/GOLAN2CODE/golan-browser/releases). Download and extract `Golan-Browser-1.2.18-source.zip` to obtain the full project, then run the commands below from the extracted source root. The GitHub landing page may contain documentation only.

Native Android WebView browser, package `com.ibngolan.browser`, Android 7.0/API 24 or later. The existing universal APK contains ARM64, ARMv7, x86 and x86_64 native payloads. It includes the multilingual tiny Whisper speech model; no separate Arabic model download is required for that bundled recognition path.

## Features

- Normal and private tabs, favorites, browsing history, downloads, light/dark themes and 21 interface locale configurations.
- Advertising/tracker blocking controls and an encrypted password vault using Android Keystore and biometric access.
- Native PDF viewing and local PDF text extraction; page/text translation tools.
- Local media workspace, supported-site media extraction using the bundled yt-dlp engine, audio extraction and subtitle/video translation tools.
- On-device speech transcription through the bundled compact Whisper runtime/model. Existing Vosk integration remains in the source.

## Install

Download `Golan_Browser_1.2.18_Universal_Arabic.apk` from the release assets, verify SHA-256 against `SHA256SUMS.txt`, then open it on the phone and allow installation from the selected source if Android requests it. The APK is the existing delivered signed binary, copied without alteration. A differently signed local build cannot update it in place.

## Build from source

Install JDK 17 or a compatible JDK, Android SDK 36 and the SDK build tools. Set `ANDROID_HOME` (or create your own ignored `local.properties` pointing to the SDK). From this directory on Windows:

```powershell
.\gradlew.bat assembleDebug
```

Output: `app/build/outputs/apk/debug/app-debug.apk`. Gradle downloads Gradle 8.14.3, Android Gradle Plugin 8.13.0 and pinned Maven dependencies on first use. Native payloads, their pinned source archives/build scripts, source model, and integrity manifests are included under `third_party/` and `app/src/main/assets/golan-asr/`; keep these files. The build verifies their recorded SHA-256 values. Native rebuild prerequisites and exact options are documented within the corresponding third-party directories.

Release builds deliberately require your own signing configuration. Use the included `signing.properties.example` or the `GOLAN_RELEASE_*` environment variables expected by `app/build.gradle`; keep your private key and passwords out of version control. The original signing key and credentials are excluded.

## Limits and privacy

Supported-site extraction is dependent on each site's formats, restrictions and changes; it is not universal and does not bypass DRM. Tiny-model speech recognition can make substantial mistakes with noise, names and dialects. Local inference does not imply that all browser operations are offline: websites, media requests and translation/provider paths may use the network. Review source and settings before processing sensitive material. Device compatibility and recognition quality are not guaranteed for every phone or language.

This publication snapshot copies the available 1.2.18 source and its required local payloads. No fresh build or device test was run during packaging, and bit-for-bit reproducibility against the delivered APK has not been established. Private data, screenshots, logs, backups, build caches and signing material are excluded.

## Licensing

No project-wide license declaration was found in the original browser root; no new license is asserted here. Included third-party notices and licenses remain authoritative for their respective components (including Whisper/model MIT, QuickJS MIT and WebP terms). Maven dependencies, FFmpeg/Python runtime contents and yt-dlp retain their own licenses. Public redistribution requires review of the complete corresponding-source and notice obligations for those bundled runtime components; the retained WebP and Whisper sources alone do not establish complete FFmpeg runtime license compliance.
