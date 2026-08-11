# Artha Business Suite v1.0.9 — Refreshed Release Manifest

**Active package refresh:** `artha-v1.0.9-r5`  
**Source commit:** `243c0d6edc276133e92cdd593d70f1f8c4922c5e`  
**Public-site overlay:** `artha-v1.0.9-r5-site` at `e908a4d7341622510285fedf587c2331b931ae34`  
**Release date:** 2026-08-11

This is the active, controlled evaluation package set. The macOS, Windows and static web-application artifacts were rebuilt from the r5 source baseline. The Android artifact is retained from r3. The prior active r4 desktop/public-site copies and r3 retained web export are preserved unchanged under `../../99-Archive/Release-Refreshes/v1.0.9-r4-20260811/`.

## Included platform artifacts

| Artifact | Validation completed | Current release status |
|---|---|---|
| `Artha-Business-Suite-macOS-Apple-Silicon-1.0.9.zip` | r5 rebuild; ZIP extraction and embedded app code-signature integrity verified | Ad-hoc signed; Developer ID signing/notarization remains a controlled activity |
| `Artha Business Suite Setup 1.0.9.exe` | r5 NSIS x64 installer generated | Authenticode signing and Windows-host installation verification remain controlled activities |
| `Artha-Business-Suite-Android-internal-1.0.9.apk` | r3 internal Gradle build, embedded JavaScript bundle and APK signature archive verification | Debug-signed internal evaluation build for arm64 devices; not a production or store-distribution package |
| `Artha-Web-Export-v1.0.9.zip` | r5 static web export with a hosting-safe consumer store entry at `/store?slug=merchant-store` | Requires the intended HTTPS hosting, domain and operational configuration |

## Associated company materials

- Current public website ZIP: `../../05-Website/v1.0.9/Artha-Public-Website-v1.0.9.zip`
- Corporate presentation: `../../08-Brand-Media/v1.0.9/Artha_Business_Suite_Corporate_Presentation_v1.0.9.pptx`
- Corporate presentation PDF: `../../08-Brand-Media/v1.0.9/Artha_Business_Suite_Corporate_Presentation_v1.0.9.pdf`
- Refreshed source archive: `../../99-Archive/Source-Releases/Artha-Business-Suite-v1.0.9-r5-site-source.zip`

## Integrity records

The exact platform package SHA-256 values are recorded in `SHA256SUMS.txt`. Additional release-material checksums are listed in the Company Integrity Manifest.
