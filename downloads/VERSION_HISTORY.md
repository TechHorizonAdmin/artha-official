# Artha package version history

## Current public evaluation release — v1.0.9 package revision r4 (15 October 2026)

- Live-tests all 31 business types, including exact inventory, CRM and POS terminology, against 29 resolved data models and 10 operating archetypes.
- Originally shipped after 111 staging migrations; the separately verified policy-parity repair brings the current canonical/production history to 112 while preserving the r4 application packages.
- Repairs the macOS desktop startup path and rebuilds macOS, Windows, Linux, Android arm64 and web packages from the verified production-only export.
- Preserves the production/staging export-cache isolation and purchase paid/due balance controls introduced in r3.
- Published under GitHub tag `v1.0.9-unsigned-r4` after the verified production rollout and policy-parity repair.

## Superseded candidate — v1.0.9 package revision r3 (12 October 2026)

- Corrected purchase paid/due balance consistency at application and database layers.
- Added production/staging export-cache isolation and cross-environment rejection checks.
- Preserved for release evidence; r4 is the current candidate.

## Previous public release — v1.0.9 package revision r2 (10 October 2026)

- Corrected production client configuration in desktop and web packages.
- Added pre-build, post-export and packaged-payload configuration audits.
- Published under GitHub tag `v1.0.9-unsigned-r2`.

## Superseded — v1.0.9 final unsigned (6 October 2026)

- Preserved for historical evidence.
- Do not distribute: desktop and web payloads were missing required service configuration.

## Historical — v1.0.8 and earlier

- Retained only as product and release history.
- Not the current download line.
