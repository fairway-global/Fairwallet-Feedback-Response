# Credential Issuing Flow

**Acceptance criterion 7:** Publish schematics of the credential-issuing model.

> **Status:** 🟡 **Provided — awaiting review.** The sequence below reflects the confirmed
> issuance steps supplied by the project team. Credentials are ToIP **ACDC**s issued over
> **IPEX**; identifiers are KERI **AIDs**.

## Issuance sequence (confirmed)

```mermaid
sequenceDiagram
    autonumber
    actor P as Participant
    participant FW as FairWallet (holder)
    participant ISS as Issuer — Issuance UI + Credential Server (Signify-TS + KERIA)

    P->>FW: Install and set up FairWallet
    FW->>FW: Create KERI Autonomic Identifier (AID)
    Note over P,ISS: Identity checked using Fayda or RID before issuance
    FW->>ISS: Establish OOBI connection
    ISS->>ISS: Select participant connection and credential schema
    ISS->>ISS: Enter and review credential attributes
    ISS->>ISS: Create and sign the ACDC credential
    ISS-->>FW: Offer credential (IPEX grant)
    FW-->>P: Review credential
    P->>FW: Accept credential
    FW-->>ISS: Send IPEX Admit; store credential in wallet
```

## Step descriptions (confirmed)

1. The participant installs and sets up FairWallet.
2. The participant creates a KERI Autonomic Identifier in FairWallet.
3. The participant's identity is checked using Fayda or RID before issuance.
4. The participant and issuer establish an OOBI connection.
5. The issuer selects the participant connection and credential schema.
6. The issuer enters and reviews the credential attributes.
7. The Credential Server creates and signs the ACDC credential.
8. The credential is offered to the participant through IPEX.
9. The participant reviews and accepts the credential in FairWallet.
10. FairWallet sends an IPEX Admit response and stores the credential.

> Cardano was not involved in this flow during the pilot — see
> [System Architecture → Use of Cardano in the pilot](system-architecture.md#use-of-cardano-in-the-pilot).

## Related

- [System Architecture](system-architecture.md)
- [Credential Verification Flow](credential-verification-flow.md)
- Evidence that issuance actually occurred (23 credentials):
  [issuance-evidence/](../issuance-evidence/README.md)
