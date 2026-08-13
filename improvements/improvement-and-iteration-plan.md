# Improvement & Iteration Plan

**Acceptance criterion 3:** Document at least three key areas for improvement.

> **Status:** 🟡 **Provided — awaiting review.** Each improvement area below is traced to
> specific evidence in the [Feedback Analysis](../feedback/feedback-analysis.md) and, where
> relevant, the [Issuance Register](../issuance-evidence/anonymized-issuance-register.md).
> Nothing here is invented; proposed changes are recommendations, not completed work.

Evidence base: 27 valid responses (20 participants + 7 organizers/stakeholders), survey period
23 July – 13 August 2026.

## Improvement area 1 — Onboarding, wallet setup & ease of use

| Field | Detail |
|-------|--------|
| Evidence source | **Wallet installation is the most-reported participant problem (4 of 20)**; 3 participants needed help to install (`with_help`); *"Instructions were unclear"* (2 of 20); stakeholder improvements: *"the system must be easy as much as possible"*, *"be accessible to many people"*; specific UX asks: *"writing down the key phrase is tiring — copy and paste should be possible"*, *"make the app work on older devices"*. |
| Problem observed | First-time install/setup was the biggest friction point; some users needed help; recovery-phrase entry and older-device support were pain points. |
| Proposed change | Simplify install/setup, add clear step-by-step in-app guidance, ease recovery-phrase handling, and improve support for lower-end/older devices. |
| Priority | High |
| Status | 🔭 Planned (recommendation) |

## Improvement area 2 — Credential verification & QR reliability

| Field | Detail |
|-------|--------|
| Evidence source | Stakeholders rated **verification the weakest pilot stage** (2 of 7 "Fair", the only stage with any "Fair"); participants reported *"Verification did not work"* (2 of 20); a verifier operator's top improvement was *"the QR code must be improved"*. |
| Problem observed | Verification/QR presentation was less reliable than issuance; self-reported success is qualified by explicit failures. |
| Proposed change | Harden the verification/QR presentation path; improve error handling and retries; add clearer verification status feedback; end-to-end test each schema. |
| Priority | High |
| Status | 🔭 Planned (recommendation) |

## Improvement area 3 — Connectivity resilience & performance

| Field | Detail |
|-------|--------|
| Evidence source | *"Internet or device problem"* (3 of 20 participants) and organizer-observed *"Internet or device problems"* (2 of 7); participants: *"improve stable Wi-Fi network"*, *"reduce processing delays"*, *"faster transaction loading times"*, *"speed of the system"*. |
| Problem observed | Performance and success were sensitive to network/device conditions; processing felt slow to some users. |
| Proposed change | Improve tolerance to poor connectivity (retries / resumable steps), optimize processing latency, and set expectations in-app during slow operations. |
| Priority | Medium–High |
| Status | 🔭 Planned (recommendation) |

## Watch item (growing signal) — Data correctness, privacy & security

| Field | Detail |
|-------|--------|
| Evidence source | A participant reported *"Credential information was incorrect"* and a *"Privacy or security concern"*; a stakeholder observed *"Privacy or security concerns"*; the issuer operator's single most important improvement was *"I need it to be very secure, so that we rely on it fully"*. |
| Problem observed | A small but **cross-cutting** (participant + stakeholder) signal around data correctness, privacy and security — notable because the schemas embed personal data (incl. national ID). |
| Proposed change | Add a holder review/confirmation step before acceptance; strengthen and document security controls; publish a clear privacy/data-handling note; apply data minimization. |
| Priority | Elevated watch |
| Status | 🔭 Planned (recommendation) |

## Iteration summary

The best-evidenced priorities for the next FairWallet iteration are **onboarding/wallet-setup
ease** (now the top-reported problem), **verification/QR reliability**, and
**connectivity/performance**, with a growing **privacy/security** watch item. Overall sentiment
was positive (satisfaction 4.30/5; 14 of 20 would use it again; institutional value 4.57/5;
5 of 7 stakeholders judged it ready for a larger pilot), so these are refinements on a working
pilot rather than fixes to a failed one. These three areas are carried directly into **Phase 1
of the [scaling plan](../scaling-strategy/scaling-plan.md)**.
