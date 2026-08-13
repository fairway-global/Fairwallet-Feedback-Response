# Final Close-out Report

**Acceptance criterion 9 (part):** Produce a close-out report.

> **Status:** 🟡 **Assembled — awaiting review.** This report is compiled from the supplied
> datasets. The **close-out video URL** is still ⛔ awaiting, and the documentation objective
> notes that final "published" status depends on a **public repository URL**.

## Executive summary

Fairway completed an Ethiopian pilot of Fayda-assisted digital credential issuance using
FairWallet, KERI Autonomic Identifiers, ACDC credentials, KERIA and the IPEX exchange protocol.
The pilot involved 25 participants associated with IE Networks and Jasper Ethiopia, with 23
credentials issued. Feedback analysis included 20 valid participant responses and 7 organizer or
institutional stakeholder responses. Participants reported average satisfaction of 4.30 out of 5,
while stakeholders rated institutional value at 4.57 out of 5. The pilot validated the
institutional issuance model while identifying wallet installation, onboarding clarity, QR and
verification reliability, and connectivity as the main improvement priorities. The pilot used
approved Fayda test API access. Production Fayda access and Cardano Backer integration were not
enabled and are documented as future, conditional roadmap activities.

## 1. Project summary

- **Project:** Leveraging National ID system in Ethiopia for more scalable adoption of Cardano in identity solutions
- **Product:** FairWallet
- **Organization:** Fairway
- **Catalyst fund / challenge:** Fund 12 — Cardano Use Cases: Concept *(Project ID 1200143)*
- **Milestone:** 4 — Evaluation and Iteration *(budget 14,250 ADA; project funding requested 95,000 ADA)*
- **Pilot location:** Bole Bulbula, Addis Ababa, Ethiopia
- **Pilot date:** 22 May 2026
- **Participants:** 20 target · 25 project-stated actual *(to be substantiated by pilot records)*
- **Participant groups:** Students and IT talents; Pilot organizers; Institutional stakeholders
- **Links:** [Product](https://www.fairwallet.et/) ·
  [Proposal](https://projectcatalyst.io/funds/12/cardano-use-cases-concept/leveraging-national-id-system-in-ethiopia-for-more-scalable-adoption-of-cardano-in-identity-solutions) ·
  [Milestones](https://milestones.projectcatalyst.io/projects/1200143/milestones) ·
  [Source](https://github.com/fairway-global/fairway-veridian-wallet)

## 2. Objectives and outcomes

Each stated objective with its outcome:

1. **Establish a partnership with an institutional National Identity provider** —
   **Partially achieved.** Fairway formally requested and received approved access to the Fayda
   test API, enabling technical integration and pilot testing. However, this did not constitute
   a formal long-term partnership, production-access agreement or endorsement by National ID
   Ethiopia. Formal production access and a longer-term institutional relationship remain future
   objectives.
2. **Integrate SSI-based identity verification with Fairway's platform** —
   **Achieved at pilot level.** Fayda test identity verification was integrated with Fairway's
   credential workflow. FairWallet used KERI Autonomic Identifiers, ACDC credentials, KERIA and
   IPEX for credential issuance and presentation. Successful Fayda verification could support
   automated issuance through configured credential templates.
3. **Test identity verification and credential issuance with IT talents** —
   **Achieved.** The pilot involved 25 participants from cohorts associated with IE Networks and
   Jasper Ethiopia, and platform records show 23 issued credentials. Among valid survey
   respondents, 18 of 19 participants who attempted verification reported successful completion.
   This survey result is **not** presented as a complete system-side verification record for all
   issued credentials.
4. **Evaluate the pilot, identify improvements, and develop a scaling strategy** —
   **Achieved.** Fairway analyzed valid feedback from 20 participants and 7 organizers or
   institutional stakeholders. The principal improvement areas were wallet installation and
   onboarding, QR and credential-verification reliability, and connectivity and performance.
   Privacy, security and credential-data correctness were retained as cross-cutting priorities.
   A four-phase scaling strategy, technical requirements, adoption roadmap and risk-mitigation
   plan were prepared.
5. **Publish documentation (partnership, technical, schemas, issuing model)** —
   **Prepared for publication.** The evidence repository documents partnership implementation,
   the KERI and ACDC architecture, credential-issuing and presentation flows, pilot schema
   definitions, template-to-schema relationships, pilot evaluation, improvement priorities and
   the proposed scaling roadmap. **Final publication status depends on making the repository
   publicly accessible and adding the remaining redacted evidence links.**

## 3. Pilot results

Summarized from the [Issuance Register](../issuance-evidence/anonymized-issuance-register.md).

- **23 verifiable credentials issued** to the student cohort on the Fairway / Veridian
  platform (status `issued`):
  - **10 ×** *Graduate Trainee Program (GTP)* — IE Networks cohort.
  - **13 ×** *Fundamental Sales Technique* — Jasper Ethiopia cohort.
- Issuance took place primarily on **22 May 2026** (pilot day), with one credential issued on
  15 May 2026.
- Every recorded student attendee (23 unique) has a corresponding issued credential.
- **System-side verification outcomes** for the issued credentials and supporting **redacted
  screenshots** are ⛔ awaiting and are not asserted here. Survey-based setup/verification
  results (self-reported by respondents) are in §4 and are **not** a system-wide verification
  record for all 23 credentials.

_Rates that depend on the feedback dataset (satisfaction, ease of use, verification) are in
§4._

## 4. Feedback summary

Summarized from the [Feedback Analysis](../feedback/feedback-analysis.md) (27 valid responses:
20 participants + 7 organizers/stakeholders; survey period 23 July – 13 August 2026).

- **Participant satisfaction 4.30 / 5**; **14 of 20** would use FairWallet again; **11 of 20**
  found a verifiable credential "Very useful".
- **Wallet setup:** 18 of 19 who attempted succeeded. **Credential receipt (survey):** 17 of 18
  who attempted. **Verification (survey):** 18 of 19 who attempted — *qualified* by two
  "verification did not work" reports and stakeholders rating verification the weakest stage.
- **Institutional value 4.57 / 5**; **5 of 7** stakeholders judged the solution ready for a
  larger pilot; **6 of 7** institutions would participate again (one conditionally).
- **Coverage:** 20 of 25 coordinated participants gave usable feedback (80%; 3 excluded for
  consent).

## 5. Key improvement areas

Summarized from the [Improvement & Iteration Plan](../improvements/improvement-and-iteration-plan.md).

1. **Onboarding, wallet setup & ease of use** — wallet installation was the top-reported
   problem; assisted setups; recovery-phrase and older-device friction.
2. **Credential verification & QR reliability** — weakest-rated stage; explicit verification
   failures reported.
3. **Connectivity resilience & performance** — network/device sensitivity; requests for faster
   processing.
- *Watch item:* data correctness, privacy & security (cross-cutting signal; relevant given
  schemas embed PII incl. national ID).

## 6. Technical implementation

Summarized from the [Technical Evaluation](../technical-implementation/technical-evaluation.md).

- Credentials are **ToIP ACDC**s on a **KERI** foundation; identifiers are KERI **AIDs** (not
  W3C DIDs). Serialization via **CESR**, exchange via **IPEX**, connections via **OOBI**.
- Holder wallet: **FairWallet**. Issuance/verification driven by Fairway UIs + a custom
  **Credential Server** (Signify-TS) against a **KERIA Cloud Agent** with **6 KERI witnesses**.
- **Cardano was not used in the pilot**; optional Cardano Backer anchoring of Key Event Logs
  is a supported but un-enabled future capability. No data was stored on-chain.
- Confirmed schematics: [architecture](../technical-implementation/system-architecture.md),
  [issuing flow](../technical-implementation/credential-issuing-flow.md),
  [verification flow](../technical-implementation/credential-verification-flow.md).
- **Credential schemas published:** two ACDC schemas —
  [Graduate Trainee Program (GTP)](../credential-schemas/schemas/graduate-trainee-program.schema.json)
  and [FaydaVerifiedAutoIssue](../credential-schemas/schemas/fayda-verified-auto-issue.schema.json).
  The "Fundamental Sales Technique" template reuses the FaydaVerifiedAutoIssue schema — see the
  [template → schema mapping](../credential-schemas/README.md).
- **Performance evaluation** (what worked / issues) is documented from the system record and
  feedback; `key_management` and `revocation` details remain ⛔ awaiting.

## 7. Partnerships

Summarized from the [Partnership & Adoption Model](../partnership-strategy/partnership-and-adoption-model.md).

- **IE Networks** (employer/training org) and **Jasper Ethiopia** (training org) each entered a
  formal pilot arrangement and coordinated the two student cohorts (10 and 15 participants
  respectively). Pilot cooperation status: **completed**.
- **National ID Ethiopia (Fayda):** Fairway obtained **approved access to the Fayda _test_ API
  only**, integrated for identity verification. This is **not** a formal partnership,
  endorsement, or production-access agreement, and no production Fayda access was held.
- Signed pilot documentation for IE Networks and Jasper Ethiopia **exists** (attested); redacted
  copies and public LinkedIn links are ⛔ awaiting supply before publication.
- Future work: continue the two institutional relationships, pursue production Fayda access and
  a formal long-term arrangement where required, and expand to further Ethiopian employers,
  universities and training providers.

## 8. Scaling and adoption

Summarized from the [Scaling Plan](../scaling-strategy/scaling-plan.md) and
[Adoption Roadmap](../scaling-strategy/adoption-roadmap.md). **All items are proposed future
roadmap, not commitments or current capability.**

- **Four phases** over ~18 months: pilot stabilization (25→100) → expanded institutional pilot
  (100–500, 3–5 institutions) → multi-institution deployment (500–5,000) → production adoption
  (5,000+).
- **Phase 1 directly addresses the three pilot findings** — verification/QR reliability,
  onboarding/ease, and connectivity/performance.
- **15 technical requirements** (production Fayda access, multi-tenant admin, RBAC, production
  key management, revocation, privacy/retention controls, schema governance, DR, etc.).
- **Conditions:** production Fayda access is **not** granted; **Cardano Backer was not enabled**
  and any production Cardano use is **conditional** on preprod testing, cost, security and legal
  review.

## 9. Milestone acceptance mapping

See the [Acceptance Criteria Traceability](../README.md#acceptance-criteria-traceability)
table and the [Evidence Index](../evidence/evidence-index.md).

## 10. Close-out video

Script: [closeout-video-script.md](closeout-video-script.md) · Close-out video link:
⛔ **Awaiting project input** · Demo video link: ⛔ Awaiting project input.

## 11. Lessons learned

1. Wallet installation and initial setup require simpler instructions, clearer device guidance
   and stronger participant support.
2. QR connection and credential-presentation workflows require explicit success states,
   recoverable retries and end-to-end reliability testing.
3. Connectivity limitations must be treated as a core product requirement for Ethiopian
   deployment rather than an exceptional failure.
4. Institutional staff training is necessary because participant success depends partly on
   timely local assistance.
5. Credential templates and credential schemas must be documented separately because several
   templates can reuse the same underlying schema.
6. Test API access demonstrates technical feasibility but must not be described as production
   access or a formal institutional partnership.
7. Credential issuance counts and verification outcomes should be recorded separately using
   system-side audit evidence.
8. Privacy, secure issuer-key management, credential correction and revocation must be
   strengthened before larger-scale adoption.
9. Cardano backing must be tested on preprod and supported by verifiable evidence before it is
   presented as an operational capability.

## 12. Acknowledgements

Fairway thanks IE Networks and Jasper Ethiopia for their formal pilot cooperation, cohort
coordination and institutional feedback. We thank all students, trainees, organizers and
institutional representatives who participated and provided feedback. We also acknowledge
National ID Ethiopia for granting access to the Fayda test API used for the technical pilot.
This acknowledgement does not imply formal endorsement or production approval. Fairway also
thanks the Cardano Catalyst community for supporting the project and its open documentation.

## Completion tracking

For the exact evidence still required to move each criterion to reviewer-verifiable **Complete**,
see the [Completion Checklist](../evidence/completion-checklist.md).
