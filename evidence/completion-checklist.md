# Completion Checklist

A working tracker of exactly what is needed to move each Catalyst acceptance criterion to
reviewer-verifiable **Complete**, plus the outstanding evidence items.

> **Definition of Complete:** an item is **Complete only when a reviewer can open the
> corresponding public, privacy-safe evidence.** Being *described* in a report is **not**
> Complete. Because this repository is **not yet published at a public URL**, no item can be
> Complete today — the realistic ceiling is **Ready for review** until the repo is public.

## Status legend

- **Missing** — evidence not yet supplied.
- **Partial** — some evidence present; specific pieces still required.
- **Ready for review** — content present, anonymized, and privacy-safe in the repo; awaiting a
  public URL (and reviewer verification).
- **Complete** — reviewer can open public, privacy-safe evidence. *(None yet — no public URL.)*

---

## Part 1 — Acceptance criteria

### Criterion 1 — Collect and analyze feedback from all 20 pilot participants and stakeholders
- **Status:** Ready for review
- **Evidence available:** [feedback-analysis.md](../feedback/feedback-analysis.md), [participant-coverage.md](../feedback/participant-coverage.md) — 27 valid responses (20 participants + 7 stakeholders).
- **Evidence still required:** public URL; note that coverage is 20 of 25 participants (not full).
- **Repository destination:** `feedback/`
- **Responsible party:** Fairway team (data) · Repo maintainer (publish)
- **Privacy/redaction check:** ✅ Anonymized (R-codes); raw in `.private-input/`.
- **Public-link check:** ❌ Pending public repository URL.

### Criterion 2 — Cover satisfaction, issues encountered and suggestions
- **Status:** Ready for review
- **Evidence available:** [feedback-analysis.md](../feedback/feedback-analysis.md) (satisfaction, ranked problems, suggestion themes).
- **Evidence still required:** public URL.
- **Repository destination:** `feedback/feedback-analysis.md`
- **Responsible party:** Fairway team · Repo maintainer
- **Privacy/redaction check:** ✅ Anonymized.
- **Public-link check:** ❌ Pending public repository URL.

### Criterion 3 — Document at least three key areas for improvement
- **Status:** Ready for review
- **Evidence available:** [improvement-and-iteration-plan.md](../improvements/improvement-and-iteration-plan.md) — 3 areas + 1 watch item, each evidence-linked.
- **Evidence still required:** public URL.
- **Repository destination:** `improvements/`
- **Responsible party:** Fairway team · Repo maintainer
- **Privacy/redaction check:** ✅ Anonymized.
- **Public-link check:** ❌ Pending public repository URL.

### Criterion 4 — Scaling strategy, technical requirements and adoption roadmap
- **Status:** Ready for review
- **Evidence available:** [scaling-plan.md](../scaling-strategy/scaling-plan.md), [adoption-roadmap.md](../scaling-strategy/adoption-roadmap.md) — 4 phases, 15 requirements, 9-milestone roadmap (proposed future).
- **Evidence still required:** public URL.
- **Repository destination:** `scaling-strategy/`
- **Responsible party:** Fairway team · Repo maintainer
- **Privacy/redaction check:** ✅ No personal data.
- **Public-link check:** ❌ Pending public repository URL.

### Criterion 5 — Publish credential schemas and technical implementation evaluation
- **Status:** Partial
- **Evidence available:** [two schemas](../credential-schemas/README.md) published; [technical-evaluation.md](../technical-implementation/technical-evaluation.md) (implementation + performance evaluation).
- **Evidence still required:** Fundamental Sales Technique **template screenshot**; `key_management` and `revocation` details; public URL.
- **Repository destination:** `credential-schemas/`, `credential-schemas/evidence/`, `technical-implementation/`
- **Responsible party:** Fairway technical · Repo maintainer
- **Privacy/redaction check:** ✅ Schemas are definitions only (no populated data); screenshot to be redaction-checked on arrival.
- **Public-link check:** ❌ Pending public repository URL.

### Criterion 6 — Publish partnership strategies and implementation
- **Status:** Partial
- **Evidence available:** [partnership-and-adoption-model.md](../partnership-strategy/partnership-and-adoption-model.md) (strategy, partners, implementation, Fayda scope).
- **Evidence still required:** redacted **IE Networks** agreement; redacted **Jasper Ethiopia** agreement; **LinkedIn** pilot-evidence URLs; redacted proof of **approved Fayda test API** access; public URL.
- **Repository destination:** `partnership-strategy/` (+ `partnership-strategy/evidence/` to be created for redacted docs)
- **Responsible party:** Fairway team · Repo maintainer
- **Privacy/redaction check:** ⚠️ Redact names/signatures/contacts in agreements before publishing.
- **Public-link check:** ❌ Pending public repository URL.

### Criterion 7 — Publish schematics of the credential-issuing model
- **Status:** Ready for review
- **Evidence available:** [system-architecture.md](../technical-implementation/system-architecture.md), [credential-issuing-flow.md](../technical-implementation/credential-issuing-flow.md), [credential-verification-flow.md](../technical-implementation/credential-verification-flow.md) (confirmed Mermaid diagrams).
- **Evidence still required:** public URL.
- **Repository destination:** `technical-implementation/`
- **Responsible party:** Fairway technical · Repo maintainer
- **Privacy/redaction check:** ✅ No personal data.
- **Public-link check:** ❌ Pending public repository URL.

### Criterion 8 — Provide evidence that credentials were issued
- **Status:** Partial
- **Evidence available:** [anonymized-issuance-register.md](../issuance-evidence/anonymized-issuance-register.md) — 23 credentials issued (system export).
- **Evidence still required:** **system-side verification evidence** (or a clearly documented limitation); redacted **issuance-dashboard screenshot**; redacted **successful-presentation / verification screenshot**; public URL.
- **Repository destination:** `issuance-evidence/`, `issuance-evidence/screenshots/`, `issuance-evidence/verification-evidence/`
- **Responsible party:** Fairway technical · Repo maintainer
- **Privacy/redaction check:** ⚠️ Redact DIDs/AIDs, credential IDs, names, national IDs in screenshots.
- **Public-link check:** ❌ Pending public repository URL.

### Criterion 9 — Produce a close-out report and video
- **Status:** Partial
- **Evidence available:** [final-closeout-report.md](../closeout/final-closeout-report.md) (assembled §1–§12); [closeout-video-script.md](../closeout/closeout-video-script.md).
- **Evidence still required:** **close-out video URL**; demo video URL (if separate); public URL.
- **Repository destination:** `closeout/`
- **Responsible party:** Fairway team · Repo maintainer
- **Privacy/redaction check:** ✅ Report anonymized; video must be privacy-checked before linking.
- **Public-link check:** ❌ Pending public repository URL.

---

## Part 2 — Outstanding evidence items

| # | Item | Status | Destination | Responsible | Privacy/redaction | Public-link |
|---|------|--------|-------------|-------------|-------------------|-------------|
| 1 | Close-out video URL | 🟡 Recorded (held off-repo) | `closeout/final-closeout-report.md` §10 | Fairway team | Privacy-check video before linking | Needs a **stable public link** (e.g. YouTube/Vimeo unlisted or a direct file) — a Drive **folder** link is not used |
| 2 | Public repository URL | ✅ Done | GitHub repo settings | Repo maintainer | n/a | Repo is public |
| 3 | System-side verification evidence *or* documented limitation | ✅ Documented limitation | `issuance-evidence/verification-evidence/README.md` | Fairway technical | n/a (text) | In repo |
| 4 | Redacted issuance-dashboard screenshot | 🟡 Held off-repo (Drive) | `issuance-evidence/screenshots/` | Fairway technical | **Not yet verified** — download locally, Claude views & confirms redaction, then commit | Needs verified file in repo |
| 5 | Redacted successful-presentation / verification screenshot | 🟡 Held off-repo (Drive) | `issuance-evidence/verification-evidence/` | Fairway technical | **Not yet verified** — same flow as #4 | Needs verified file in repo |
| 6 | Demo video URL (if separate) | ⛔ Not applicable / not supplied | `closeout/final-closeout-report.md` §10 | Fairway team | Privacy-check | — |
| 7 | Fundamental Sales Technique template screenshot | ⛔ Missing | `credential-schemas/evidence/` | Fairway technical | Redact any identifiers | Needs verified file in repo |
| 8 | Redacted IE Networks agreement (MoU) | 🟡 Held off-repo (Drive MoU folder) | `partnership-strategy/evidence/` | Fairway team | **Not yet verified** — redact names/signatures/contacts, then commit | Needs verified file in repo |
| 9 | Redacted Jasper Ethiopia agreement (MoU) | 🟡 Held off-repo (Drive MoU folder) | `partnership-strategy/evidence/` | Fairway team | **Not yet verified** — redact names/signatures/contacts | Needs verified file in repo |
| 10 | LinkedIn pilot-evidence URL | ✅ Provided | `partnership-strategy/partnership-and-adoption-model.md` | Fairway team | Public post | In repo |
| 11 | Proof of approved Fayda test API access | 🟡 Verbal confirmation only | `partnership-strategy/partnership-and-adoption-model.md` | Fairway team | n/a | Confirmed verbally (Telegram) + public API docs; **no formal artifact** — documented as such |
| 12 | Reason two Jasper participants did not receive credentials | ✅ Provided | `feedback/participant-coverage.md` | Fairway team | n/a | In repo (no smartphone / incomplete setup) |
| 13 | Decision on the 15 May credential (keep/exclude) | ⛔ Pending decision | `issuance-evidence/anonymized-issuance-register.md` | Fairway team | n/a | — |
| 14 | Duplicate-attendee handling | 🟡 Counted once — confirm | `issuance-evidence/anonymized-issuance-register.md` | Fairway team | n/a | — |
| 15 | Missing-ID attendee handling | 🟡 Noted — confirm | `feedback/participant-coverage.md` | Fairway team | n/a | — |
| 16 | Final operational-facts JSON | ⛔ Not supplied | `.private-input/` (raw) → derived docs | Fairway team | Anonymize before deriving | n/a (raw stays private) |

---

## How to reach Complete

1. **Publish the repository** at a public URL (item 2) — this unblocks the public-link check for
   every "Ready for review" item.
2. **Supply the redacted evidence artifacts** (items 3–11) into their destinations, redaction-
   checked.
3. **Provide the video URL(s)** (items 1, 6) and confirm the open decisions (items 12–15).
4. Re-verify each criterion; update statuses here and in the
   [Evidence Index](evidence-index.md) and [README](../README.md).
