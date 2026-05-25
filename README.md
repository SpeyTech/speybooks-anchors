# SpeyBooks Anchor Chain

Public cryptographic audit chain anchors for SpeyBooks (AX-CRY-001).

Each file in `anchors/` is a daily SHA-256 snapshot of all organisation
chain terminal states. The `latest-anchor.txt` file is an append-only
log of every anchor date and hash.

## Verification

```bash
tsx scripts/verify-anchor.ts anchors/YYYY-MM-DD.json
```

## GPG Signing Key

Commits are signed with key `5513BE575627151D72EB3DF91C98AC2AFFCB0951`.

## Scope

Anchors are periodic (daily). See AX-CRY-001 in the SpeyBooks kernel
documentation for the full threat model and scope limitations.
