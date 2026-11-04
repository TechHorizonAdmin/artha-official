# Platform Release Status — v1.0.9 Package Revision r4

| Platform | Artifact status | What is verified | External gate |
|---|---|---|---|
| Web | r4 static merchant and storefront export published | Production-only host configuration and checksum verified | Approved production hosting, monitoring, customer terms and operational acceptance |
| macOS Apple Silicon | r4 ZIP published | Archive and strict ad-hoc bundle-signature verification | Apple organisation enrolment, Developer ID signing, notarisation and clean-device acceptance |
| Windows x64 | r4 NSIS installer and portable ZIP published | Checksums and PE/NSIS structure verified | Organisation Authenticode signing and clean Windows install/upgrade/uninstall/SmartScreen acceptance |
| Linux x64 | r4 AppImage and Debian package published | Checksums, ELF/AppImage executable structure and Debian package structure verified | Company GPG release signature and supported-distribution clean-host acceptance |
| Android arm64 | r4 self-contained internal APK published | Checksum and internal/debug-signed evaluation status recorded | Company Play Console, production signing, AAB, closed testing and store review |
| iOS/iPadOS | No distributable package in r4 | Expo bundle identifier and tablet configuration exist | Full Xcode, Apple organisation signing assets, generated native project and real-device/TestFlight acceptance |

No platform is represented as store-distributed or publisher-signed unless its external signing gate is separately evidenced. The current public files are controlled evaluation artifacts.
