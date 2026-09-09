# Issuance Evidence

**Acceptance criterion 8:** Provide evidence that credentials were issued.

> **Status:** 🟡 **Provided — awaiting review.** The
> [anonymized issuance register](anonymized-issuance-register.md) evidences **23 credentials
> issued**, plus an anonymized **issuer dashboard** screenshot ([`screenshots/`](screenshots/))
> and an anonymized **verifier dashboard** screenshot with a documented verification limitation
> ([`verification-evidence/`](verification-evidence/)). **Per-credential detail screenshots were
> withheld** because they exposed holder DIDs / credential IDs; they are held in
> `.private-input/` pending fuller redaction. This folder holds only **anonymized, redacted**
> material.

## Contents

| Item | Purpose |
|------|---------|
| [anonymized-issuance-register.md](anonymized-issuance-register.md) | Per-participant issuance/verification record, keyed by participant code only. |
| [`screenshots/`](screenshots/) | Redacted dashboard/wallet screenshots showing issuance. |
| [`verification-evidence/`](verification-evidence/) | Redacted evidence that issued credentials verify successfully. |

## Redaction checklist (required before any file is added here)

Every screenshot, log, or artifact placed in this folder must have the following removed or
masked:

- [ ] Names and email addresses
- [ ] Student IDs and any institutional identifiers
- [ ] Wallet addresses
- [ ] Full DIDs (mask to a non-resolvable partial, or remove)
- [ ] Private keys, seed phrases, mnemonics
- [ ] Session tokens, API keys, bearer tokens
- [ ] Unredacted credential identifiers / serial numbers
- [ ] QR codes that encode any of the above

Raw, unredacted source files stay in `.private-input/` (git-ignored) and are never published.

## Evidence status categories

Evidence in this folder is labelled with one of:

- ✅ **Completed evidence** — present, anonymized, verifiable here.
- 🟡 **Provided — awaiting review** — supplied and published, not yet reviewer-verified.
- ⛔ **Awaiting project input** — not yet supplied.
- 🔭 **Planned future work** — described as future activity, not milestone evidence.
