# Artha Business Suite v1.0.9 — Package Revision r4

Prepared on 13 October 2026 from the organized Artha completion workspace.

Revision r4 supersedes r3 for new evaluations. The application version remains 1.0.9; r4 identifies the business-engine verified, desktop-startup repaired cross-platform package revision.

## Application package set

| Platform | Package | SHA-256 | Verified status |
| --- | --- | --- | --- |
| macOS Apple Silicon | `Artha-Business-Suite-macOS-Apple-Silicon-1.0.9.zip` | `ca1ffe01003f8229426d7b37546ca1121656254960ff3e1106a027915fc92a4f` | Archive integrity, ad-hoc code signature and embedded production-host checks pass |
| Windows x64 | `Artha-Business-Suite-Windows-portable-1.0.9-x64.zip` | `7660fd1c0d441b1770babda8dc0089afb4a5c4b5123c9878e558b0144f752fbf` | Portable archive integrity and embedded production-host checks pass |
| Windows x64 installer | `Artha-Business-Suite-Windows-Setup-1.0.9-x64.exe` | `fd24ae4a25b738af98155bce7666f62fa93f57db9743c146857f93a23f716068` | NSIS installer built from the verified Windows payload; unsigned |
| Linux x64 | `Artha-Business-Suite-Linux-1.0.9-x86_64.AppImage` | `72956dac00e8bc8d74db0d7c67841a300cfb30b199132d5617e3432a363aab3d` | ELF/AppImage structure and executable-bit checks pass |
| Debian/Ubuntu amd64 | `Artha-Business-Suite-Linux-1.0.9-amd64.deb` | `21e4d11014c3bb1c2b555c1f8003aff1b21b302a1ab3f54db3e1fddc06e1dd8e` | Debian archive structure and embedded production-host checks pass |
| Android arm64 | `Artha-Business-Suite-Android-internal-1.0.9-arm64.apk` | `c218d151d34228f987b8871d8ea85136fa796cfb7f81f07339a1451f06a840a1` | arm64-only internal APK; production host audited; APK v2 debug signature verified |
| Web | `Artha-Web-Application-unsigned-1.0.9.zip` | `ff4d66beab7c6b900df56978e3e1eda944855862686313f11e186a7b7c8b5bad` | Static merchant and storefront export; production-only host pass |

The GitHub Release will include the machine-readable `SHA256SUMS.txt` covering these seven application artifacts and the public website source snapshot.

## r4 corrections and verification

- All 31 business types pass live staging setup and exact inventory, CRM and point-of-sale terminology checks.
- The registry resolves 29 data models across 10 operating archetypes with no extended type silently falling back to the generic Retail model.
- The staging database replays 111 migrations and verifies 140 of 140 public tables under RLS with 193 policies.
- The macOS desktop startup path now selects an available local port, waits for the embedded server and keeps diagnostic logs.
- Production and staging exports remain isolated; the production verifier rejects staging-host contamination.
- macOS, Windows, Linux, Android and web targets were rebuilt after the corrections.

## External release boundaries

The approved production rollout and separately approved policy-parity cleanup passed on 15 October 2026. Production and staging both have 140/140 RLS-enabled public tables, 193 policies and zero named drift policies, with no pending migration, seed or role change. This remains an unsigned evaluation package line: Apple Developer ID signing/notarization, Windows Authenticode signing, Android production keystore/AAB, clean-device acceptance on target operating systems, provider-authorized payment and GST submission, messaging delivery, and physical printer/scanner acceptance remain separate controlled release gates.
