# Artha v1.0.9 — Refreshed Package Installation Guide

All active evaluation packages are in this `04-Releases/v1.0.9` folder. Verify each download against `SHA256SUMS.txt` before using it.

## Included artifacts

- **macOS Apple Silicon:** `Artha-Business-Suite-macOS-Apple-Silicon-1.0.9.zip`
- **Windows x64:** `Artha Business Suite Setup 1.0.9.exe`
- **Web:** `Artha-Web-Export-v1.0.9.zip`
- **Android arm64 internal evaluation:** `Artha-Business-Suite-Android-internal-1.0.9.apk` — self-contained, debug-signed, and not a production/store package.

## macOS

1. Extract the ZIP and move `Artha Business Suite.app` to Applications.
2. The package is ad-hoc signed, not Developer ID notarized. Follow organizational endpoint policy; use a controlled evaluation Mac or provide a Developer ID identity for a notarized build.
3. Open the application, sign in with a controlled evaluation account, and run the POS, stock, print and export flow.

## Windows

1. Run the x64 NSIS installer on a controlled Windows test host.
2. Verify SmartScreen/Authenticode behavior independently. A signing certificate and a Windows verification host are required before claiming production install certification.
3. Test login, POS, export and print paths under a non-production evaluation identity.

## Android

1. Use a controlled arm64 Android evaluation device and install the internal APK through the organization’s approved testing method.
2. The package carries the application bundle; it is not the prior developer shell and does not need a development server to load the application code.
3. Use a controlled evaluation account. Do not treat debug signing as production or store approval.

## Web

The ZIP is a static Expo web export. Serve it through an approved HTTPS origin configured with the intended Supabase environment. Do not place `.env` files, credentials or real customer data in the archive or hosting configuration.

## Acceptance checklist

- Version shown is 1.0.9.
- Exact barcode/SKU scan auto-adds the product to the cart.
- Sale/return changes stock as expected for the authorized branch.
- Report export creates the expected CSV for the selected report tab; receipt/label export uses the permitted print/export flow.
- Tenant/role switching remains within allowed context.
- No test account, secret, real payment, real customer data or provider credential is placed in evidence screenshots.
