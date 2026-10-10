# Artha Business Suite v1.0.9 — Package Revision r2

Prepared on 10 October 2026 from the organized Artha completion workspace.

Revision r2 supersedes the 6 October package set. The application version remains 1.0.9; r2 identifies the corrected cross-platform packaging revision.

## Package set

| Platform | Package | SHA-256 | Verified status |
| --- | --- | --- | --- |
| macOS Apple Silicon | `mac/Artha-Business-Suite-macOS-Apple-Silicon-1.0.9.zip` | `ebac727a9337204208b835394abafa08ac3a0b1fb1dbb87b53c9ac0face627b5` | Ad-hoc signature and archive integrity pass; embedded production host pass; packaged app launched and read-only live modules tested |
| Windows x64 | `windows/Artha-Business-Suite-Windows-portable-1.0.9-x64.zip` | `0c26dbc2e8341b07d4b4beed61cabf8d7b70f246d922b67309aec56cd0ebc2c6` | Portable archive integrity and embedded production host pass |
| Windows x64 installer | `windows/Artha-Business-Suite-Windows-Setup-1.0.9-x64.exe` | `ea8234f14041c13b2a67c3bdfbf26caf7dc578406a12c92c8d0a07f1c4e57d7c` | NSIS installer built from the same audited Windows application payload; unsigned |
| Linux x64 | `linux/Artha-Business-Suite-Linux-1.0.9-x86_64.AppImage` | `d7fac697a799b26ae7f769fc8767ad2162849e44ef7fda2d37f3acbf097b8704` | Built from the same verified Linux payload as the deb; executable format pass |
| Debian/Ubuntu amd64 | `linux/Artha-Business-Suite-Linux-1.0.9-amd64.deb` | `4cacd7610f85e8492e2cc1f040210a9e89a572e6b2d80bd1e3837b09fe8d8ad3` | Debian structure and embedded production host pass |
| Android arm64 | `android/Artha-Business-Suite-Android-internal-1.0.9-arm64.apk` | `fb38b2d64cde49d7c48ff125415fa72ab7f17cf87923145cb285be42565a8017` | Self-contained internal/debug-signed APK; embedded production host pass |
| Web | `web/Artha-Web-Application-unsigned-1.0.9.zip` | `e43f02ac065f547cbac110ae822727d73bbfaf3f787175ab0b72060d04748abd` | Static merchant and storefront export; embedded production host pass |

`SHA256SUMS.txt` is the machine-readable checksum source for these seven downloadable application artifacts.

## r2 repair

The earlier desktop and web packages did not contain Artha's required public service configuration and displayed a missing-configuration error. Revision r2 fixes the build pipeline, adds fail-closed environment checks, and audits the exported and packaged payloads before release. The earlier package set remains preserved only as a superseded historical record.

## Validation evidence

- TypeScript and the approved quality baseline pass.
- All 24 module, business-engine, commerce, security, GST, payment, printing, export, automation and service contract suites pass.
- Dedicated staging verification passes for all 109 migrations, database lint, all 139 public tables under RLS, tenant isolation, the retail sale/return lifecycle, and specialised engine smoke journeys; synthetic data was rolled back.
- The Business Type Engine presents all 31 configured business experiences, including retail, wholesale, distribution, manufacturing, grocery, boutique, restaurant/cafe/bakery, salon/spa/gym, pharmacy/clinic/hospital, electronics, fashion, hardware, agriculture, food processing, automobile/repair, construction, professional services, education, real estate and generic service/other profiles.
- The repaired macOS package was live-tested read-only against Artha production for sign-in/session loading, dashboard, POS, inventory, customers, purchases, returns, GST, accounting, reports, storefront status and Business Type Engine.

## External release boundaries

This remains an unsigned evaluation package line. Apple Developer ID notarization, Windows Authenticode/installer signing, Android production signing/AAB, clean-device acceptance on target Windows/Linux/Android machines, provider-authorized payment and GST submission, messaging delivery, and physical printer/scanner acceptance require their respective identities, services or hardware.
