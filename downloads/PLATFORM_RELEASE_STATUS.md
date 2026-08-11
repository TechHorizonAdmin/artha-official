# Platform Release Status — v1.0.9 Refreshed Set

| Platform | Artifact status | What is verified | External gate |
|---|---|---|---|
| Web | r5 static application export built | Expo web export with hosting-safe `/store` consumer entry | Approved HTTPS host/domain, operational monitoring |
| macOS Apple Silicon | r5 ZIP built and archive-verified | App bundle structure and ad-hoc code signature | Developer ID signing + Apple notarization |
| Windows x64 | r5 NSIS installer built | Installer generation | Authenticode certificate + Windows-host install/SmartScreen validation |
| Android arm64 | r3 self-contained internal APK retained | Gradle internal build, embedded app JavaScript bundle and signature archive verification | Production keystore, clean-device runtime proof and store distribution |
| iOS | Expo project configuration at v1.0.9 | Source configuration | Mac/iOS build environment, Apple certificate/profile and device/App Store proof |

No platform is represented as store-distributed or production-signed unless its external signing gate is separately evidenced.
