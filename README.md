# Verona Yatırım Android downloads

This public repository distributes signed APK builds only. The Android source repository remains private.

The app checks [latest.json](https://raw.githubusercontent.com/raunchz/verona-android-updates/main/latest.json) when opened and periodically in the background. It verifies the advertised APK's package, version, SHA-256, and signing certificate before opening Android's installer. Android asks the user to confirm installation.

Current baseline: **1.0.18**. Install [VeronaYatirim-1.0.18.apk](https://raw.githubusercontent.com/raunchz/verona-android-updates/main/releases/VeronaYatirim-1.0.18.apk) once to enable GitHub-based update checks.
