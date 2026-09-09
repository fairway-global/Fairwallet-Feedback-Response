# FairWallet — Cardano Catalyst Final Milestone Evidence

**Product:** FairWallet · **Organization:** Fairway · **Milestone:** Evaluation and Iteration

This repository is the reviewer-facing evidence package for the final milestone of the
FairWallet project on Project Catalyst. It documents the pilot evaluation, the feedback
analysis, the technical implementation, the credential-issuance evidence, and the scaling,
partnership and close-out materials required for milestone acceptance.

> **Status of this repository:** Scaffolded and awaiting project data. Sections marked
> **`⛔ Awaiting project input`** are placeholders and **do not** constitute submitted
> evidence. They will be populated only from data supplied by the project team and will be
> published in anonymized, publication-safe form.

---

## Project at a glance

| Field | Value |
|-------|-------|
| Project title | Leveraging National ID system in Ethiopia for more scalable adoption of Cardano in identity solutions |
| Catalyst fund | Fund 12 |
| Challenge category | Cardano Use Cases: Concept |
| Project ID | 1200143 |
| Milestone | 4 — Evaluation and Iteration |
| Organization | Fairway |
| Product | FairWallet |
| Funding requested | 95,000 ADA |
| Milestone 4 budget | 14,250 ADA |
| Pilot location | Bole Bulbula, Addis Ababa, Ethiopia |
| Pilot date | 22 May 2026 |
| Participants | 20 target · 25 project-stated actual *(to be substantiated by the pilot records)* |
| Participant groups | Students and IT talents · Pilot organizers · Institutional stakeholders |
| Partner institutions | Jasper Ethiopia · IE Networks *(partnership detail awaited — see [partnership model](partnership-strategy/partnership-and-adoption-model.md))* |

**Public links:** [Product site](https://www.fairwallet.et/) ·
[Catalyst proposal](https://projectcatalyst.io/funds/12/cardano-use-cases-concept/leveraging-national-id-system-in-ethiopia-for-more-scalable-adoption-of-cardano-in-identity-solutions) ·
[Milestones](https://milestones.projectcatalyst.io/projects/1200143/milestones) ·
[Source repository](https://github.com/fairway-global/fairway-veridian-wallet)

> The participant figure is a project-stated count. It is context, **not** feedback-coverage
> evidence — coverage is substantiated separately from the pilot and feedback datasets.

---

## How to review this repository

Reviewers should start with the **[Acceptance Criteria Traceability](#acceptance-criteria-traceability)**
table below. Each row links directly to the repository document that carries the evidence for
that criterion, and shows the current status of that evidence.

For a single consolidated view of every artifact, see the
**[Evidence Index](evidence/evidence-index.md)**. For exactly what is still needed to move each
criterion to reviewer-verifiable **Complete**, see the
**[Completion Checklist](evidence/completion-checklist.md)**.

---

## Status legend

This repository uses one consistent set of status labels. A label is never a claim that
work is finished unless it is explicitly **Completed evidence**.

| Label | Meaning |
|-------|---------|
| ✅ **Completed evidence** | Evidence is present, anonymized, and verifiable in this repository. |
| 🟡 **Provided — awaiting review** | Evidence has been supplied and published, but has not yet been reviewer-verified. |
| ⛔ **Awaiting project input** | No evidence yet. The section is a placeholder only. |
| 🔭 **Planned future work** | Described as a future activity, not presented as completed milestone evidence. |

---

## Acceptance Criteria Traceability

| # | Acceptance criterion | Required evidence | Repository document | Current status |
|---|----------------------|-------------------|---------------------|----------------|
| 1 | Collect and analyze feedback from all 20 pilot participants and stakeholders | Coverage record for all participants and stakeholders; analysis of results | [participant-coverage.md](feedback/participant-coverage.md) · [feedback-analysis.md](feedback/feedback-analysis.md) | 🟡 Provided — awaiting review *(27 valid responses; 20 of 25 participants (80%) + 7 stakeholders)* |
| 2 | Cover satisfaction, issues encountered and suggestions | Analysis broken down by satisfaction, issues and suggestions | [feedback-analysis.md](feedback/feedback-analysis.md) | 🟡 Provided — awaiting review |
| 3 | Document at least three key areas for improvement | Three or more evidence-based improvement areas | [improvement-and-iteration-plan.md](improvements/improvement-and-iteration-plan.md) | 🟡 Provided — awaiting review *(3 areas + 1 watch item)* |
| 4 | Develop a detailed scaling strategy, technical requirements and adoption roadmap | Scaling plan, technical requirements, adoption roadmap | [scaling-plan.md](scaling-strategy/scaling-plan.md) · [adoption-roadmap.md](scaling-strategy/adoption-roadmap.md) | 🟡 Provided — awaiting review *(4 phases, 15 tech requirements, 9-milestone roadmap — proposed future)* |
| 5 | Publish the credential schemas and technical implementation evaluation | Credential schema definitions; technical evaluation | [credential-schemas/](credential-schemas/README.md) · [technical-evaluation.md](technical-implementation/technical-evaluation.md) | 🟡 Provided — awaiting review *(2 schemas ✅; template screenshots ✅; evaluation incl. key-mgmt/revocation ✅)* |
| 6 | Publish partnership strategies and implementation | Partnership strategy and implementation status | [partnership-and-adoption-model.md](partnership-strategy/partnership-and-adoption-model.md) | 🟡 Provided — awaiting review *(LinkedIn ✅; redacted MoUs ✅; Fayda = verbal test-access)* |
| 7 | Publish schematics of the credential-issuing model | Diagram(s) of the credential-issuing model | [credential-issuing-flow.md](technical-implementation/credential-issuing-flow.md) · [system-architecture.md](technical-implementation/system-architecture.md) | 🟡 Provided — awaiting review *(architecture, issuing & verification diagrams confirmed)* |
| 8 | Provide evidence that credentials were issued | Anonymized issuance register, screenshots, verification evidence | [anonymized-issuance-register.md](issuance-evidence/anonymized-issuance-register.md) · [issuance-evidence/](issuance-evidence/README.md) | 🟡 Provided — awaiting review *(23 issued; issuer/verifier dashboards ✅; verification limitation documented; per-credential detail withheld)* |
| 9 | Produce a close-out report and video | Close-out report; close-out video (script + link) | [final-closeout-report.md](closeout/final-closeout-report.md) · [closeout-video-script.md](closeout/closeout-video-script.md) | 🟡 Report complete (§1–§12); close-out video ✅ linked |

---

## Repository structure

```
fairwallet-catalyst-final-milestone/
├── README.md                      ← you are here (reviewer entry point)
├── input-schemas/                 ← JSON templates for supplying project data
├── feedback/                      ← surveys, coverage and feedback analysis
├── technical-implementation/      ← evaluation + architecture / flow diagrams
├── credential-schemas/            ← published credential schema definitions
├── issuance-evidence/             ← anonymized proof credentials were issued
├── improvements/                  ← key improvement areas and iteration plan
├── partnership-strategy/          ← partnership and adoption model
├── scaling-strategy/              ← scaling plan and adoption roadmap
├── closeout/                      ← close-out report and video script
└── evidence/                      ← consolidated evidence index
```

The `.private-input/` directory (git-ignored) holds the **raw, unredacted data** supplied by
the project team. It is **never published**. All documents in this repository are generated
in anonymized, publication-safe form from that raw input.

---

## Data handling and privacy

This repository is public. To protect participants and stakeholders, the following rules are
enforced across every published document:

- Only **anonymized** information is published (e.g. participant codes such as `P01`).
- The repository never publishes names, emails, student IDs, wallet addresses, full DIDs,
  private keys, seed phrases, tokens, or unredacted credential identifiers.
- Raw or sensitive source material is stored only in `.private-input/`, which is excluded
  from version control via [`.gitignore`](.gitignore).
- Screenshots and logs must be redacted before being added to published folders.

See [issuance-evidence/README.md](issuance-evidence/README.md) for the specific redaction
checklist applied to evidence artifacts.

---

## How this repository is populated

Content is produced from structured input supplied by the project team, one dataset at a
time, using the templates in [`input-schemas/`](input-schemas/). The intake order is:

1. Project metadata
2. Pilot and credential-issuance results
3. Technical implementation
4. Actual credential schemas
5. Partnership information
6. Participant and stakeholder feedback
7. Scaling and adoption strategy
8. Close-out report and video information

No statistics, feedback, partnerships, dates, links, or accomplishments are invented. Where
data has not yet been supplied, the section shows **`⛔ Awaiting project input`**.
