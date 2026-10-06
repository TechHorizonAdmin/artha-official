# Artha Business Suite v1.0.9 — Final Unsigned Evaluation Release

Prepared on 6 October 2026 from the frozen Artha completion workspace.

## Package set

| Platform | Package | SHA-256 | Status |
| --- | --- | --- | --- |
| macOS Apple Silicon | `mac/Artha-Business-Suite-macOS-Apple-Silicon-1.0.9.zip` | `c90c588a1b4ed88ee142ea56d642eb801c5689194c187e7f0240788f0e8ef5a1` | Ad-hoc signed; unsigned evaluation package |
| Windows x64 | `windows/Artha-Business-Suite-Windows-portable-1.0.9-x64.zip` | `05815f5249f556a90deddcfac7b1e5abda66c14b0af014363f4030bbc8ebb6d2` | Portable unsigned evaluation package |
| Linux x64 | `linux/Artha-Business-Suite-Linux-1.0.9-x86_64.AppImage` | `51717827a81cb113e72acc779e89caf39b17d11cb7a61e3a93541c79eeeca93c` | AppImage structure verified |
| Debian/Ubuntu amd64 | `linux/Artha-Business-Suite-Linux-1.0.9-amd64.deb` | `23361043fdd71b3a479bf68c93c3cfbdd3e77ad94fcbbab432490c287aa3b261` | Debian package structure verified |
| Android arm64 | `android/Artha-Business-Suite-Android-internal-1.0.9-arm64.apk` | `fb38b2d64cde49d7c48ff125415fa72ab7f17cf87923145cb285be42565a8017` | Internal/debug-signed APK |
| Web | `web/Artha-Web-Application-unsigned-1.0.9.zip` | `db1f3b684e1690b2c7c22c5467595b81e3c0ec254fef9dfd809eba9ef4794d87` | Static merchant and storefront export |
| Public website | `website/Artha-Public-Website-unsigned-1.0.9.zip` | `6a6bf76dbd80592e1c8c6f88f1614ba994efd08e9ba8e6a8573a7fcb3d362b0e` | Self-contained website archive with downloads |

`SHA256SUMS.txt` is the machine-readable checksum source for this package set.

## Recorded validation evidence

- 109 database migrations replayed successfully on the dedicated Artha staging project.
- Row-level security enabled on all 139 public tables.
- 192 row-level security policies present.
- Zero missing policy-backed API grants in the staging audit.
- Anonymous access to protected data denied.
- Two-tenant isolation rollback test passed.
- Retail lifecycle rollback test passed for GST validation, sale and items, stock consumption, payment, customer metrics, sale journal, return/restock, and reversal journals.
- Specialised engine smoke tests passed for restaurant modifiers, service availability, gym plan validation, pharmacy batch/prescription, electronics serials, and production-batch lifecycle.
- Public-website, release-candidate, and staging-database verification suites passed from the organized completion workspace.

## Release boundaries

This is the final unsigned evaluation set. It is suitable for controlled installation, demonstration, customer validation, and clean-machine acceptance testing. It is not represented as an Apple-notarized, Authenticode-signed, Play Store-signed, or Linux-distribution-signed store release.

Before unrestricted commercial distribution, complete publisher signing/notarization, clean-device acceptance, production credentials, payment-provider approval, statutory/GST authorization, and physical printer/scanner tests applicable to the deployment.
