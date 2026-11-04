# Artha v1.0.9 r4 Evaluation Package Installation Guide

The active public evaluation release is package revision r4. Download only from the links on `https://arthabusiness.in/` or the GitHub release tagged `v1.0.9-unsigned-r4`, then verify every file against `SHA256SUMS.txt` before use.

## Included artifacts

- **macOS Apple Silicon:** `Artha-Business-Suite-macOS-Apple-Silicon-1.0.9.zip`
- **Windows x64 installer:** `Artha-Business-Suite-Windows-Setup-1.0.9-x64.exe`
- **Windows x64 portable:** `Artha-Business-Suite-Windows-portable-1.0.9-x64.zip`
- **Linux x64:** `Artha-Business-Suite-Linux-1.0.9-x86_64.AppImage`
- **Debian/Ubuntu amd64:** `Artha-Business-Suite-Linux-1.0.9-amd64.deb`
- **Web:** `Artha-Web-Application-unsigned-1.0.9.zip`
- **Android arm64 internal evaluation:** `Artha-Business-Suite-Android-internal-1.0.9-arm64.apk` — self-contained, debug-signed, and not a production/store package.

## macOS

1. Extract the ZIP and move `Artha Business Suite.app` to Applications.
2. The package is ad-hoc signed, not Developer ID notarized. Follow organizational endpoint policy; use a controlled evaluation Mac or provide a Developer ID identity for a notarized build.
3. Open the application, sign in with a controlled evaluation account, and run the POS, stock, print and export flow.

## Windows

1. Run the x64 NSIS installer on a controlled Windows test host.
2. Verify SmartScreen/Authenticode behavior independently. A signing certificate and a Windows verification host are required before claiming production install certification.
3. Test login, POS, export and print paths under a non-production evaluation identity.

## Linux

1. On a controlled x86-64 Linux test machine, verify the checksum before installation.
2. For AppImage, preserve the executable bit and launch only under the organisation's endpoint policy.
3. For Debian/Ubuntu, inspect the package metadata and install on a supported clean test host.
4. Complete login, POS, export, print and uninstall checks. The current artifacts are checksummed but not GPG-signed distribution packages.

## Android

1. Use a controlled arm64 Android evaluation device and install the internal APK through the organization’s approved testing method.
2. The package carries the application bundle; it is not the prior developer shell and does not need a development server to load the application code.
3. Use a controlled evaluation account. Do not treat debug signing as production or store approval.

## Web

The ZIP is a static Expo web export. Serve it through an approved HTTPS origin configured with the intended Supabase environment. Do not place `.env` files, service-role keys, signing keys, credentials or real customer data in the archive or hosting configuration.

## Acceptance checklist

- Version shown is 1.0.9.
- Exact barcode/SKU scan auto-adds the product to the cart.
- Sale/return changes stock as expected for the authorized branch.
- Report export creates the expected CSV for the selected report tab; receipt/label export uses the permitted print/export flow.
- Tenant/role switching remains within allowed context.
- No test account, secret, real payment, real customer data or provider credential is placed in evidence screenshots.
- The operator records the artifact hash, device/OS version, result and tester before approving any wider distribution.
