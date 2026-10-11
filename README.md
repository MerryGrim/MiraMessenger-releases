# Mira Messenger APK releases

Public Android distribution channel for Mira Messenger. Application sources are stored in the owner's private repository.

The current MVP is **0.2.0-mvp** for Android 8.0+ (arm64-v8a and x86_64). It includes encrypted Matrix chats, voice/video calls through the configured homeserver's MatrixRTC service, and background APK update checks/downloads.

- [Download the latest APK](https://github.com/MerryGrim/MiraMessenger-releases/releases/latest/download/MiraMessenger.apk)
- [Update manifest](https://github.com/MerryGrim/MiraMessenger-releases/releases/latest/download/update-manifest.json)
- [Checksums](https://github.com/MerryGrim/MiraMessenger-releases/releases/latest/download/SHA256SUMS.txt)
- [Release history](https://github.com/MerryGrim/MiraMessenger-releases/releases)

Install the first APK over the earlier MVP. Do not uninstall Mira or clear its data to upgrade: local history keys are stored with application data. This MVP keeps the previous development signing certificate.

Mira checks updates daily and offers an immediate check inside the app. New versions download in the background; the APK's size, SHA-256, package, version and signing certificate are verified. Installation requires a separate tap and Android's confirmation. Android may defer background jobs.

Incoming calls require Mira to be open; offline push calling is not implemented yet. A password alone cannot recover lost encryption keys, and message redaction cannot guarantee removal of other participants' copies or backups.

Bundled Element Call has its own license. See [LICENSE-NOTICE.md](LICENSE-NOTICE.md) and [SOURCE.md](SOURCE.md) for its official license and exact upstream source. Keeping Mira's Git repository private does not grant a commercial Element license.