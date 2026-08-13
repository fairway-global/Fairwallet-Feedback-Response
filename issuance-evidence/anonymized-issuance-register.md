# Anonymized Issuance Register

**Acceptance criterion 8:** Evidence that credentials were issued.

> **Status:** 🟡 **Provided — awaiting review.** This register is generated from the
> platform's credential-issuance export (retained privately in `.private-input/`, git-ignored).
> It evidences **23 credentials issued** to the student cohort during the pilot. All
> identifiers — holder DIDs, credential IDs, and any personal data — are excluded; only
> anonymized participant codes and aggregate figures are published.

## What this dataset does and does not cover

- **Covers:** credential **issuance** for the student participant group (status `issued`).
- **Does not cover (⛔ awaiting):** wallet-setup outcomes, credential **verification**
  outcomes, dashboard/verification screenshots, and the demo video. These will be added when
  supplied.
- Organizers and institutional stakeholders were not credential-issued; they are covered by
  the feedback datasets, not this register.

## Aggregate issuance summary

| Cohort | Partner | Credential template | Credentials issued |
|--------|---------|---------------------|--------------------|
| Students and IT talents — IE Networks | IE Networks | Graduate Trainee Program (GTP) | 10 |
| Students and IT talents — Jasper | Jasper Ethiopia | Fundamental Sales Technique | 13 |
| **Total** | | | **23** |

**Issuance dates:** 22 credentials issued on **22 May 2026** (pilot day); 1 GTP credential
issued on **15 May 2026**. All records carry platform status `issued`.

## Per-participant register (anonymized)

Each row is one issued credential, keyed to an internal participant code only. "Verified" and
"Wallet setup" are marked `—` because they are **not present in this dataset** — they are not
assumed.

| Code | Group | Cohort | Credential template | Credential issued | Credential verified | Wallet setup |
|------|-------|--------|---------------------|-------------------|---------------------|--------------|
| P01 | Students and IT talents | IE Networks | Graduate Trainee Program (GTP) | ✅ Yes | — (not in dataset) | — (not in dataset) |
| P02 | Students and IT talents | IE Networks | Graduate Trainee Program (GTP) | ✅ Yes | — (not in dataset) | — (not in dataset) |
| P03 | Students and IT talents | IE Networks | Graduate Trainee Program (GTP) | ✅ Yes | — (not in dataset) | — (not in dataset) |
| P04 | Students and IT talents | IE Networks | Graduate Trainee Program (GTP) | ✅ Yes | — (not in dataset) | — (not in dataset) |
| P05 | Students and IT talents | IE Networks | Graduate Trainee Program (GTP) | ✅ Yes | — (not in dataset) | — (not in dataset) |
| P06 | Students and IT talents | IE Networks | Graduate Trainee Program (GTP) | ✅ Yes | — (not in dataset) | — (not in dataset) |
| P07 | Students and IT talents | IE Networks | Graduate Trainee Program (GTP) | ✅ Yes | — (not in dataset) | — (not in dataset) |
| P08 | Students and IT talents | IE Networks | Graduate Trainee Program (GTP) | ✅ Yes | — (not in dataset) | — (not in dataset) |
| P09 | Students and IT talents | IE Networks | Graduate Trainee Program (GTP) | ✅ Yes | — (not in dataset) | — (not in dataset) |
| P10 | Students and IT talents | IE Networks | Graduate Trainee Program (GTP) | ✅ Yes | — (not in dataset) | — (not in dataset) |
| P11 | Students and IT talents | Jasper Ethiopia | Fundamental Sales Technique | ✅ Yes | — (not in dataset) | — (not in dataset) |
| P12 | Students and IT talents | Jasper Ethiopia | Fundamental Sales Technique | ✅ Yes | — (not in dataset) | — (not in dataset) |
| P13 | Students and IT talents | Jasper Ethiopia | Fundamental Sales Technique | ✅ Yes | — (not in dataset) | — (not in dataset) |
| P14 | Students and IT talents | Jasper Ethiopia | Fundamental Sales Technique | ✅ Yes | — (not in dataset) | — (not in dataset) |
| P15 | Students and IT talents | Jasper Ethiopia | Fundamental Sales Technique | ✅ Yes | — (not in dataset) | — (not in dataset) |
| P16 | Students and IT talents | Jasper Ethiopia | Fundamental Sales Technique | ✅ Yes | — (not in dataset) | — (not in dataset) |
| P17 | Students and IT talents | Jasper Ethiopia | Fundamental Sales Technique | ✅ Yes | — (not in dataset) | — (not in dataset) |
| P18 | Students and IT talents | Jasper Ethiopia | Fundamental Sales Technique | ✅ Yes | — (not in dataset) | — (not in dataset) |
| P19 | Students and IT talents | Jasper Ethiopia | Fundamental Sales Technique | ✅ Yes | — (not in dataset) | — (not in dataset) |
| P20 | Students and IT talents | Jasper Ethiopia | Fundamental Sales Technique | ✅ Yes | — (not in dataset) | — (not in dataset) |
| P21 | Students and IT talents | Jasper Ethiopia | Fundamental Sales Technique | ✅ Yes | — (not in dataset) | — (not in dataset) |
| P22 | Students and IT talents | Jasper Ethiopia | Fundamental Sales Technique | ✅ Yes | — (not in dataset) | — (not in dataset) |
| P23 | Students and IT talents | Jasper Ethiopia | Fundamental Sales Technique | ✅ Yes | — (not in dataset) | — (not in dataset) |

## Calculated totals (from records above)

| Metric | Value | Calculation |
|--------|-------|-------------|
| Credentials issued (student cohort) | **23** | count of `status = issued` records |
| — via IE Networks (GTP) | 10 | count in IE Networks export |
| — via Jasper (Fundamental Sales Technique) | 13 | count in Jasper export |
| Student attendees recorded | 23 unique | attendee list, de-duplicated (24 rows − 1 duplicate) |
| Issuance coverage of recorded student attendees | 23 / 23 | credentials issued ÷ unique student attendees |
| Credentials verified | ⛔ Awaiting project input | not present in this dataset |
| Wallet-setup success rate | ⛔ Awaiting project input | not present in this dataset |

> Note: "23 / 23" reflects that every recorded student attendee has a corresponding issued
> credential (counts match 1:1 by cohort). It is **not** a claim about participants who may
> have attended without registering, nor about verification.

## Supporting artifacts

- Redacted issuance screenshots: [`screenshots/`](screenshots/) — ⛔ Awaiting project input.
- Verification evidence: [`verification-evidence/`](verification-evidence/) — ⛔ Awaiting project input.
- Source export (not published): retained in `.private-input/` (git-ignored).
