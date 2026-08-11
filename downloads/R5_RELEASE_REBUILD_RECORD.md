# Artha v1.0.9 r5 — Consumer Storefront Release Record

**Source tag:** `artha-v1.0.9-r5`  
**Source commit:** `243c0d6edc276133e92cdd593d70f1f8c4922c5e`  
**Build date:** 11 August 2026

## Included refresh

- A public static-host entry at `/store?slug=merchant-store` is emitted in the web export.
- Merchants can edit customer-facing storefront announcement and section titles; show, hide and reorder sections; set their HTTPS web-host address; preview the consumer app; and share the complete consumer URL.
- The consumer storefront uses the published builder configuration for the hero, catalogue mode, story and contact blocks.

| Artifact | SHA-256 |
|---|---|
| `Artha-Business-Suite-macOS-Apple-Silicon-1.0.9.zip` | `031a02a74687fb6d575733f600fdb5f20f6ddee23a56c824290b3d1e43401917` |
| `Artha Business Suite Setup 1.0.9.exe` | `4f1ece10438770f0e47ce54c6c709545fbde3676b51d6c7b046b944cad8b41cb` |
| `Artha-Web-Export-v1.0.9.zip` | `15778f156401e58663c2afa64c173d7d3578c5c3aaefed29ae223e82d3b9e94c` |

The same three artifacts and their checksum file are staged in `../../05-Website/official-site/downloads/`.

## Distribution boundary

These are controlled evaluation artifacts. macOS is ad-hoc signed, not notarized. Windows has not yet had Authenticode signing or a clean Windows-host/SmartScreen acceptance. The web export needs an HTTPS host chosen and controlled by Artha before customer distribution.
