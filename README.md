# Saya Beats

Saya Beats is a custom Android music app for streaming music with YouTube Music as the backend. This build is based on the open-source SimpMusic project and is rebranded for SHNWAZ.

## Links

- GitHub repo: https://github.com/shnwazdeveloper/Saya-Beats
- Developer profile: https://github.com/shnwazdeveloper
- Website: https://shnwazdeveloper.github.io
- Source base: https://github.com/maxrave-dev/SimpMusic

## What Changed

- Renamed the visible app name to Saya Beats.
- Changed the Android application id to `com.shnwazdeveloper.sayabeats`.
- Updated About, review, Discord, backup, and update links for Saya Beats.
- Added this README, ABOUT, and CHANGELOG for the custom project.
- Kept the GPL-3.0 license and upstream attribution.

## Release APK

Use JDK 21 and the Android SDK. The release build is not a debug APK.

```bash
./gradlew androidApp:assembleRelease
```

Signed release APKs are produced with:

```bash
KEYSTORE_PATH=./saya-beats.jks KEYSTORE_PASSWORD=... KEY_ALIAS=sayabeats KEY_PASSWORD=... ./build_and_sign_apk.sh --release --foss
```

The signed APK output is under:

```text
androidApp/build/outputs/apk/release/
```

The local signing key is intentionally ignored by Git. Keep the same key safe if you want future Saya Beats updates to install over this release.

## License

Saya Beats is based on SimpMusic and remains licensed under GPL-3.0. See [LICENSE](LICENSE).

Original project credit: Tuan Minh Nguyen Duc / maxrave-dev and SimpMusic contributors.
