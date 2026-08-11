# Artha Business Suite v1.0.9 — Refreshed Release Record

**Status:** Artha company release, refreshed 2026-08-11.  
**Active release tag:** `artha-v1.0.9-r5`.  
**Historical baseline:** The original v1.0.9 package set remains preserved in the company archive.

## What changed in this refresh

- The Reports Engine Export action now creates a real, tenant-scoped CSV for Financial, Profit & Loss, GST, Inventory, Staff and Customer reports. CSV cells are protected against spreadsheet formula injection.
- Browser export downloads a file and Electron opens a save dialog. On native mobile, the current permitted fallback is an explicit share flow; it is not represented as a device-file download.
- PDF export uses browser/Electron print-to-PDF paths where available, with the existing native share-file fallback retained.
- An exact barcode/SKU scan immediately adds the matched product to the POS cart; scan failures stay visible and actionable.
- The Android artifact is now a self-contained `internal` arm64 evaluation build with its JavaScript bundle embedded. The prior debug developer shell is archived and is no longer in the active release folder.
- The public product website’s release hub now points to the refreshed packages and includes the product-tour media library.
- Migrations 2026081009–2026081013 are deployed to the linked project: safe branch-stock foundation, authoritative branch inventory writers, storefront fulfilment-branch inventory, business-local accounting dates and protected branch lifecycle controls.
- A business-type change now explicitly remains within the current business; a separate business is created through a separate tenant setup path. Branch management adds safe main-branch assignment and stock-aware retirement instead of destructive deletion.
- A dedicated consumer-store entry is emitted at `/store?slug=merchant-store`, so plain static hosts can serve a public, mobile-first storefront without a dynamic-route rewrite.
- The merchant storefront builder now edits customer-facing announcements and section titles, controls section visibility and saves the public-store base address used to generate a shareable HTTPS customer URL.
- The public storefront now renders the published builder’s announcement, product selection mode, story and contact blocks rather than treating the builder as merchant-only metadata.
- The macOS, Windows and static web-application artifacts were rebuilt from r5. The Android artifact remains r3; the public website and its download copies are refreshed for r5.

## Verified gates

Typecheck, formatting, tenant-context, desktop-security, file-export and commerce contract checks passed against the r5 source state on 2026-08-11. The consumer route was opened from a plain static server with no browser errors. The macOS ZIP passed archive extraction and embedded ad-hoc code-signature integrity verification. The Windows NSIS installer was freshly built. The static web export contains `store/index.html`; the Android evidence remains from r3.

## Important limits

This is not a claim that external payment, GSP/GST, messaging, hardware, platform signing/notarization, Windows clean-device acceptance, iOS distribution or commercial/legal diligence is certified. Those gates require real providers, controlled devices or owner evidence and remain recorded separately.
