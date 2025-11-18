# Security policy

## Reporting a vulnerability
- Please email: security@warp-genesis-omega.example
- Include: affected files, reproduction steps, logs, and environment details.
- We respond within 72 hours and coordinate responsible disclosure.

## Supported versions
- Only tagged releases (vX.Y.Z) are eligible for security support.
- `main` requires GPG-signed commits and protected reviews.

## Handling secrets
- No private keys, seeds, or wallets may be stored in the repository.
- Use OS-keystore/GPG; never commit `.key`, `.pem`, `.wallet`, or ENV files with secrets.

## Build integrity
- All releases publish SHA256 checksums and detached GPG signatures.
- Verification scripts are in `scripts/security/`.

## Incident response
- Immediate freeze of protected branches, key rotation, and signed advisory.
- Postmortem published in `docs/security/postmortems/`.
