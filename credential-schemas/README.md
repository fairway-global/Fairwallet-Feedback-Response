# Credential Schemas

**Acceptance criterion 5 (part):** Publish the credential schemas.

> **Status:** ✅ **Published.** The two ACDC schemas used in the pilot are published in full
> under [`schemas/`](schemas/). Only **schema definitions** (field names, types, structure)
> are published — **no populated credentials or participant data**. Schema SAIDs are public
> schema identifiers, not per-person credential identifiers.

## Schemas vs. templates

FairWallet separates **schemas** from **credential templates**:

- A **schema** is the reusable ACDC data definition, identified by a **Schema SAID**.
- A **credential template** is a configuration built *on top of* a schema. **Multiple
  templates can reuse a single schema**, each with its own **display name**, **template ID
  (UUID)**, selected/configured fields, and issuance settings (e.g. auto-issue). A template
  UUID is **not** a schema SAID.

## Published schemas

| Schema title | File | Schema SAID | Credential type | Version |
|--------------|------|-------------|-----------------|---------|
| Graduate Trainee Program (GTP) | [`schemas/graduate-trainee-program.schema.json`](schemas/graduate-trainee-program.schema.json) | `EBsQYagqI26-K6hgqrTWg77Zto64RL0B_O4AgkyvUW92` | `GraduateTraineeProgramGTPCredential` | 1.0.0 |
| FaydaVerifiedAutoIssue | [`schemas/fayda-verified-auto-issue.schema.json`](schemas/fayda-verified-auto-issue.schema.json) | `EHYYZFJas0_cgo3nA1_BeeyWRIzyWqic3pM-LdYmL_R6` | `FaydaVerifiedAutoIssueCredential` | 1.0.0 |

## Template → schema mapping (as used in the pilot)

| Credential template (display name) | Cohort | Template ID (UUID) | Underlying schema (SAID) | Credentials issued |
|------------------------------------|--------|--------------------|--------------------------|--------------------|
| Graduate Trainee Program (GTP) | IE Networks | *(not supplied)* | Graduate Trainee Program (GTP) — `EBsQYag…UW92` | 10 |
| Fundamental Sales Technique | Jasper Ethiopia | `afac71ee-8641-41ee-9140-ef03465b8042` | **FaydaVerifiedAutoIssue** — `EHYYZFJas…LdYmL_R6` | 13 |

**Note on "Fundamental Sales Technique":** this is **not a separate schema**. It is a
credential *template* record (display name "Fundamental Sales Technique") built on the reusable
**FaydaVerifiedAutoIssue** schema. Template configuration reported for the pilot: auto-issue
after Fayda verification **enabled**, **6** configured fields, **13** credentials issued,
template created/updated **2026-05-22 00:09:22**.

Evidence of this template-to-schema mapping (platform screenshot):
[`evidence/`](evidence/) — ⛔ **awaiting upload** (see that folder's note).

## About the schema contents

Both schemas follow the ACDC top-level structure (`v`, `d`, `u`, `i`, `ri`, `s`, `a`) with an
`a` (attributes) block. The attributes blocks define **personal-data fields** — `fayda_id`,
`name`, `email`, `phone_number`, `birthdate`, `gender` (GTP also adds `Cohort`, `Start Period`,
`End Period`). These are **field definitions only**; this repository publishes **no** credential
carrying real values, and any example credential added later will use **synthetic/redacted**
values.

## Publication rules for this folder

- Schemas are published **exactly as supplied**, only reformatted for readability — field
  names and structure are not invented.
- Example credentials (if added) must use **synthetic or redacted** values. Never publish a
  real holder's data, real holder AID, or an unredacted credential SAID.

## Still to supply

- The **GTP template** metadata (UUID / configuration), if you want it documented like the
  Fundamental Sales Technique template.
- Optional: one **sanitized example credential** per schema for [`examples/`](examples/).
