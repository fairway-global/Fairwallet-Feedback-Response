# Technical Implementation Evaluation

**Acceptance criterion 5 (part):** Publish the technical implementation evaluation.

> **Status:** 🟡 **Provided — awaiting review.** The technical *implementation* is documented as
> confirmed by the project team, and the **performance evaluation** (§ "Evaluation against pilot
> use") is now synthesized from the system record and feedback results. `key_management` and
> `revocation` details remain ⛔ awaiting.

## Overview

FairWallet issues **ToIP Authentic Chained Data Container (ACDC)** credentials on a **KERI**
(Key Event Receipt Infrastructure) foundation. Participant identifiers are **KERI Autonomic
Identifiers (AIDs)** rather than W3C DIDs. Credentials are serialized with **CESR** and
exchanged over the **IPEX** protocol; peer connections are bootstrapped with **OOBIs**. The
holder wallet is **FairWallet**; issuance and verification are driven by Fairway UIs and a
custom **Credential Server** using **Signify-TS** against a **KERIA Cloud Agent**, backed by
six standard KERI witnesses. See the [system architecture](system-architecture.md),
[issuing flow](credential-issuing-flow.md) and
[verification flow](credential-verification-flow.md).

## Technology summary

| Aspect | Detail |
|--------|--------|
| Credential standard | ToIP ACDC, supported by KERI (Key Event Receipt Infrastructure) |
| Credential format | Self-addressing ACDC serialized with CESR; exchanged via the IPEX protocol |
| DID method | Not applicable — uses KERI Autonomic Identifiers (AIDs), not W3C DIDs (e.g. not `did:prism`) |
| Role of Cardano | **Not used in the pilot.** Optional Cardano Backer anchoring of Key Event Logs is supported by the architecture but was not enabled (see below) |
| Issuer component | Fairway Credential Issuance UI + custom Credential Server (Signify-TS + KERIA Cloud Agent) |
| Holder wallet | FairWallet (KERI edge wallet) |
| Verifier component | Fairway Request Presentation interface + Credential Server (Signify-TS + KERIA) |
| Key management approach | Issuer signing keys (KERI AIDs) are managed within the **KERIA deployment** on the project's **Firebase-hosted** server infrastructure; production-grade managed key storage, rotation and recovery are a scaling requirement |
| Revocation approach | ACDC **credential status registry** (`ri`) on KERIA provides the basis for revocation; controlled correction/status/revocation procedures were not a pilot focus and are a scaling requirement |

## Use of Cardano in the pilot

Stated plainly for reviewers, exactly as confirmed by the project team:

- Cardano was **not directly used** in the deployed pilot environment.
- The pilot ran KERIA with **six standard KERI witnesses**; no Cardano Backer, Cardano node,
  or Ogmios service was running.
- **No credentials, personal information, or credential hashes were stored on Cardano** during
  the pilot.
- The Veridian architecture supports **optional Cardano Backer integration** for anchoring
  KERI Key Event Receipt Logs — **not enabled** in this pilot.

## Component responsibilities

| Component | Responsibility | Technology |
|-----------|----------------|------------|
| FairWallet | Holder edge wallet; creates the AID, receives/holds/presents credentials | KERI edge wallet (Signify) |
| Credential Issuance UI | Issuer operator interface (connection, schema, attributes) | Fairway |
| Credential Server | Creates/signs ACDCs; drives IPEX issuance and presentation | Custom (Signify-TS) |
| Request Presentation UI | Verifier operator interface | Fairway |
| KERIA Cloud Agent | Cloud KERI agent for wallet, issuer and verifier | KERIA |
| KERI witnesses (×6) | Receipt/availability of key events (Key Event Logs) | Standard KERI witnesses |
| Cardano Backer | Optional Key Event Log anchoring — **not enabled in pilot** | Cardano (future) |

## Evaluation against pilot use

Evidence-based summary derived from the **system record** (credential export) and the
**survey findings** (24 valid responses). This is a synthesis from those sources, clearly
attributed; the project team may replace it with its own narrative.

**What worked**
- **Issuance at scale on KERI/ACDC:** the system record shows **23 credentials issued** across
  two schemas/cohorts on the pilot day — the core issue path performed.
- **Positive reception:** participant satisfaction **4.30/5**; **11 of 20** found a verifiable
  credential "Very useful"; stakeholders rated **issuance** and **technical support** highly
  (mostly Excellent/Good) and institutional value **4.57/5**.
- **Setup and receipt mostly worked:** **18 of 19** participants who attempted wallet setup
  succeeded (3 needed help); **17 of 18** who attempted reported receiving their credential.

**What was weaker**
- **Onboarding / wallet installation** was the top friction point: *"wallet installation"* was
  the most-reported participant problem (**4 of 20**), with several assisted setups and
  recovery-phrase/older-device pain points.
- **Verification/QR reliability** was the softest stage: stakeholders rated verification the
  **weakest stage (2 of 7 "Fair")**, and two participants reported *"Verification did not
  work"*. Self-reported verification success (**18 of 19** attempted) should be read with this
  caveat — and a **system record of issuance does not by itself prove verification**.
- **Connectivity/performance sensitivity:** "internet or device" problems appeared in both
  participant (**3 of 20**) and organizer (**2 of 7**) responses, plus requests to reduce
  processing delays.
- **Privacy/security signal:** a small cross-cutting signal (one participant, one stakeholder,
  and the issuer operator's top ask for stronger security) — relevant given the PII-bearing
  schemas.

These feed the [Improvement & Iteration Plan](../improvements/improvement-and-iteration-plan.md).

## Known limitations

- **Verification reliability** under real conditions needs hardening (see above).
- **Connectivity dependence:** the flow was sensitive to network/device conditions during the
  pilot.
- **No production Fayda access:** identity verification used the Fayda **test** API only.
- **No Cardano anchoring:** Key Event Logs were not anchored on Cardano in the pilot (optional
  future capability).
- **Key management:** pilot issuer keys are held within the KERIA/Firebase deployment;
  production-grade managed key storage, rotation, recovery and separation of duties are a
  scaling requirement (server-side evidence can be provided to reviewers on request).
- **Revocation:** supported in principle via the ACDC status registry (`ri`) but not exercised
  in the pilot; controlled revocation/correction is a scaling requirement.

## Related diagrams

- [System Architecture](system-architecture.md)
- [Credential Issuing Flow](credential-issuing-flow.md)
- [Credential Verification Flow](credential-verification-flow.md)

## Public references

- Source repository: <https://github.com/fairway-global/fairway-veridian-wallet>
- Product site: <https://www.fairwallet.et/>

Additional repositories and documentation: ⛔ Awaiting project input. *(The technical stack,
standards, DID method, and on-chain role are not inferred from the repository name and remain
⛔ Awaiting project input until confirmed via the technical-implementation dataset.)*
