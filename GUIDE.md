# GOLAN Browser 1.2.18: usage guide

[العربية](GUIDE.ar.md) · [Project and downloads](README.md)

## Start with the right package

Install the existing universal APK from [Releases](https://github.com/GOLAN2CODE/golan-browser/releases), checking its SHA-256 against the supplied checksum file. Android 7/API24 or later is required. The package includes four processor architectures and the compact multilingual speech model. A matching signing certificate is needed to update an existing installation; a separately rebuilt APK can have a different certificate.

## Browse and keep useful pages

Use normal tabs for everyday browsing and private tabs for private browsing. Favorites keep useful addresses; history helps revisit pages. Choose the interface language and light or dark appearance to suit your reading. Advertising and tracker blocking controls can reduce unwanted requests, but site behavior varies and blocking may affect page functions. Private browsing is not anonymity from websites, network operators or services you sign into.

The password vault stores saved credentials using Android Keystore encryption and supports biometric access. Keep control of the phone and its unlock method. Do not treat the vault or private tabs as a guarantee against every compromised device or malicious website.

## Read, translate and work with media

The PDF tools display documents inside the app and can extract available PDF text locally. A scanned image does not automatically become selectable text. Page and text translation use network translation endpoints; sending text for translation is different from local speech recognition.

For media, start from a supported page or an actual media/subtitle file and use the available download, audio-extraction or translation tools. The bundled yt-dlp engine handles supported sites on the phone. Login state, site restrictions and upstream changes can affect results. This is not a universal downloader or a DRM bypass. Use content you are authorized to access.

The bundled Whisper path transcribes speech locally using a small model. Review the result before sharing or relying on names, numbers or subtitles. Noise, dialects and overlapping speakers can reduce accuracy. The separate microphone speech feature uses Android's installed recognition provider, which may use the network; it should not be confused with the bundled local-file recognizer.

## Permissions and practical limits

Microphone permission is relevant when recording or recognizing speech. Android file pickers and save/share flows determine which documents the app can read or export; older Android versions can require storage permission for download workflows. Biometric access depends on the device configuration. Grant a permission when you need its related feature and review Android settings if you change your mind. Websites and downloads still need connectivity, and larger media tasks use storage, battery and processing time.

## Cost and computer FAQ

**Does this use my paid AI account?** No personal paid AI API key or billing integration was found in the reviewed first-party source. The browser contains shared YouTube service identifiers for interoperability; these are not identified as your paid account key. This finding is a source review, not an inspection of your account billing.

**Does it need my PC or Codex?** No. After installation it runs on the phone without a running PC, this chat or Codex. Internet services, Android recognition providers and mobile-data charges can still apply.

This guide documents the available source and existing package. No new build or device verification was performed for these publication guides; identical rebuilding of the APK has not been established. See [third-party information](THIRD_PARTY.md) for component provenance and unresolved review questions.
