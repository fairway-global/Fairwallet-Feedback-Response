# Scaling Plan & Technical Requirements

**Acceptance criterion 4 (part):** Develop a detailed scaling strategy and technical
requirements.

> **Status:** 🟡 **Provided — awaiting review.** Everything in this document is a **proposed
> future roadmap** — not a commitment, a current capability, or completed work. All scales,
> timeframes and activities are targets.

> ### ⚠️ Important conditions (as stated by the project team)
> - **Production Fayda access has NOT been granted.** The pilot used approved **test** API
>   access only.
> - **Cardano Backer was NOT enabled in the pilot.**
> - **Any production Cardano use remains conditional** on successful **preprod** testing, cost
>   assessment, security review, and legal approval. It must be described as *planned* until a
>   preprod deployment produces verifiable technical evidence.

## Vision

Scale FairWallet from a 25-person pilot into reliable, privacy-preserving digital credential
infrastructure for Ethiopian employers, training providers and educational institutions. The
platform will connect approved Fayda identity verification with institution-issued ACDC
credentials controlled by holders, while introducing Cardano-backed KERI integrity **only after
controlled technical testing and validation**.

## Target segments

- Ethiopian employers operating graduate and trainee programs
- Universities and higher-education institutions
- Technical and vocational training providers
- Professional certification organizations
- Institutions that need trusted credential verification
- Public-sector identity and education stakeholders

## Scaling phases (proposed)

| Phase | Objective | Target scale | Timeframe |
|-------|-----------|--------------|-----------|
| **1 — Pilot stabilization** | Resolve onboarding, connectivity and verification problems found in the pilot | 25 → 100 participants (existing partners) | 0–3 months |
| **2 — Expanded institutional pilot** | Validate repeatable onboarding, issuance and verification across cohorts | 100–500 participants, 3–5 institutions | 3–6 months |
| **3 — Multi-institution deployment** | Operate a secure multi-tenant service with common governance | 500–5,000 holders, multiple institutions | 6–12 months |
| **4 — Production adoption** | Sustainable service with formal governance, support and SLAs | 5,000+ holders, continuing issuance | 12–18 months |

### Phase 1 activities — directly addressing the three pilot findings

Phase 1 maps one-to-one to the evidence-based
[improvement areas](../improvements/improvement-and-iteration-plan.md) from the feedback
analysis:

| Pilot finding (Dataset 6) | Phase 1 activities |
|---------------------------|--------------------|
| **1. Verification & QR reliability** | Improve QR connection and credential-presentation reliability; complete verification evidence; add clearer success/error messages. |
| **2. Onboarding clarity & ease** | Improve wallet-installation and onboarding instructions; add clearer progress messages; train partner staff to support participants. |
| **3. Connectivity & performance** | Introduce retry handling for unreliable connectivity; add clearer progress/status feedback. |
| *(supporting)* | Test credential correction and revocation procedures; complete operational documentation. |

### Later-phase activities (summary)

- **Phase 2:** apply for appropriate Fayda **production** access; institution roles/access
  controls; reusable onboarding/training materials; schema approval & versioning; monitoring &
  audit reporting; measured completion rates; incident-escalation procedures.
- **Phase 3:** multi-tenant issuer/verifier administration; institution reporting & audit; load
  / security / recovery testing; documented integration APIs; **test Cardano Backer on
  preprod** and measure reliability/cost/benefit; independent security & privacy review.
- **Phase 4:** move approved Fayda workflows to production; SLAs & formal support; production
  key-management & disaster recovery; credential governance; **decide on production Cardano
  backing based on preprod evidence, cost and legal review**; sustainable pricing/operating
  model; publish reusable guidance.

## Technical requirements

| Requirement | Rationale | Priority |
|-------------|-----------|----------|
| Approved Fayda **production** API access | Pilot used test access; production needs formally approved access & conditions | must-have |
| Reliable wallet onboarding & guided setup | Feedback identified installation difficulties and unclear instructions | must-have |
| Reliable QR connection & credential-presentation workflow | QR/verification reliability was a main improvement area | must-have |
| Low-bandwidth support, retries & recoverable operations | Connectivity problems must not cause permanent failure | must-have |
| Multi-tenant issuer & verifier administration | Institutions need separated users, credentials, schemas, records, permissions | must-have |
| Role-based access control & institutional approval workflow | Only authorized staff should issue/request/revoke | must-have |
| Production-grade issuer key management | Signing keys need managed storage, controls & recovery | must-have |
| Credential correction, status & revocation procedures | Institutions need controlled correction/revocation | must-have |
| Monitoring, audit logs & operational reporting | Evidence of events without exposing unnecessary personal data | must-have |
| Privacy, consent & data-retention controls | Fayda-linked data needs minimization, access control & retention rules | must-have |
| Schema registry, versioning & governance | Reusable schemas/templates must be documented & managed | must-have |
| Backup & disaster recovery | Recover issuer config without compromising holder-controlled credentials | must-have |
| Scalable issuance processing & load testing | Larger cohorts need reliable concurrent issuance | should-have |
| Cardano Backer **preprod** integration | Cardano backing was not enabled; test on preprod & evaluate before any production claim | should-have |
| Documented institutional integration APIs | Larger institutions may connect student/HR/certification systems | should-have |

## Risks & mitigations

| Risk | Mitigation |
|------|------------|
| Fayda production access delayed or not approved | Keep test/production separated; complete requirements early; never use test access for production users |
| Cardano backing presented as operational before tested | Describe as *planned* until preprod produces verifiable evidence |
| Unreliable connectivity interrupts onboarding/exchange | Retries, resumable operations, clearer status, low-bandwidth testing |
| Institutional signing keys lost or compromised | Managed key protection, restricted authorization, audit logs, recovery, separation of duties |
| Personal information exposed via logs/reports/evidence | Data minimization, access controls, retention rules, anonymization, publication review |
| Incompatible or duplicative institutional schemas | Governed schema registry with ownership, review, reuse & versioning |
| Participants need more assistance than institutions can provide | Short guided onboarding, trained support staff, monitor drop-off |
| Verification results inconsistent or unclear | Define success criteria, improve messages, end-to-end test every schema |

_The phased adoption timeline is in [adoption-roadmap.md](adoption-roadmap.md)._
