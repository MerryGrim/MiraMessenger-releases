# Mira Messenger — LAMBDADEV

Official Android Release distribution for **Mira Messenger 0.10.0**.
Permanent package: **chat.mira.messenger**. Android 8.0+, arm64-v8a/x86_64.
Application sources remain in the owner's private repository.

- [Download Release APK](https://github.com/MerryGrim/MiraMessenger-releases/releases/latest/download/MiraMessenger-release.apk)
- [Release update manifest](https://github.com/MerryGrim/MiraMessenger-releases/releases/latest/download/update-manifest-release.json)
- [Checksums](https://github.com/MerryGrim/MiraMessenger-releases/releases/latest/download/SHA256SUMS.txt)
- [Previous releases](https://github.com/MerryGrim/MiraMessenger-releases/releases)

Release includes camera/gallery photos and videos, files, voice messages,
one-point location, native Matrix polls, formatted text, replies, edits, reactions,
and backward history pagination. The compact composer grows only for multiline
text. Circular avatars appear across the app; profile photos can be selected,
cropped in a round pan/zoom editor, uploaded or removed. Profile avatars are public
Matrix media; message attachments use native SDK encryption in E2EE rooms.

Release also retains Matrix/E2EE messaging, voice/video calls, Firebase or the own-server
push transport, message checkmarks and GitHub background update checks/downloads.
One check means server acceptance; two require another participant's public read
receipt (at least one participant in a group). Matrix has no standard phone-delivery
acknowledgement. Notification deduplication applies within one installation;
cross-device notification dismissal is not implemented.

Version 0.10.0 (code12) updates Release 0.9.0 in place with the same permanent key.
The permanent package installs separately from the archived .debug MVP. Keep old data
until the required encrypted history is accessible in the new app. Sign in and
restore available Matrix keys; a login password alone cannot recover lost E2EE keys.
Later Release versions replace this same package with the existing permanent key
and a higher versionCode. APK size, SHA-256, package/version and certificate are
checked before installation. Android requires the user's installation confirmation.

Firebase requires reachable Google services; the own-server option works without
Google and uses an Android foreground listener. Delivery can be delayed by device
or network restrictions. Redaction cannot erase other devices' or servers' copies.

Public signing-certificate SHA-256:
`7e1a6e2805adb106e7e2f28e0dd956b9ce819f1e04a0964b27a3f46459ec5cf0`.
This is the existing permanent certificate; no new private key was generated.

Bundled Element Call has its own license. See [LICENSE-NOTICE.md](LICENSE-NOTICE.md)
and [SOURCE.md](SOURCE.md) for its official license and exact upstream source.
Keeping Mira's Git repository private does not grant a commercial Element license.

В 0.10.0: обычные и секретные DM, сведения о комнате и профиле, Matrix SAS, правила уведомлений, отдельные страницы настроек. Одна основная кнопка завершения звонка, звук в меню, исправленная очистка сессии. Ключи требуются для E2EE-истории; проверка эмуляторов не устанавливает причину выключения физического телефона.
