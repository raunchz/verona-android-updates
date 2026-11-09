# Verona Yatırım Android downloads

This public repository distributes signed APK builds only. The Android source repository remains private.

The app checks [latest.json](https://raw.githubusercontent.com/raunchz/verona-android-updates/main/latest.json) when opened and periodically in the background. It verifies the advertised APK's package, version, SHA-256, and signing certificate before opening Android's installer. Android asks the user to confirm installation.

Current baseline: **1.0.18**. Install [VeronaYatirim-1.0.18.apk](https://raw.githubusercontent.com/raunchz/verona-android-updates/main/releases/VeronaYatirim-1.0.18.apk) once to enable GitHub-based update checks.

## Publishing a future APK

1. Upload the signed APK under `releases/VeronaYatirim-<version>.apk`.
2. Update `latest.json` with the new `versionCode`, `versionName`, raw APK URL, lowercase SHA-256, exact byte size, and release notes.
3. Commit both changes to `main`. Phones will find the update on app launch or their next background check.

Keep the APK package name `com.veronayatirim.portal` and signing certificate unchanged. Android requires the user to confirm installation.
