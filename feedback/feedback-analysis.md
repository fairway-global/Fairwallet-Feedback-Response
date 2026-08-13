# Feedback Analysis

**Acceptance criteria 1 & 2:** Analyze feedback from pilot participants and stakeholders,
covering **satisfaction**, **issues encountered**, and **suggestions**.

> **Status:** 🟡 **Provided — awaiting review.** All figures below are calculated from the
> anonymized survey exports (retained in `.private-input/`, git-ignored). Every metric shows
> its **denominator**. No answers were invented; missing / not-applicable values are excluded
> from the relevant denominator rather than guessed.

## How to read this analysis — four distinct kinds of statement

- **Survey finding** — what respondents self-reported in the feedback forms.
- **System record** — what the platform's credential export shows (e.g. 23 credentials issued).
- **Organizer observation** — what organizers/stakeholders observed (kept separate from
  participant experience; an observation is never presented as participant feedback).
- **Missing / unconfirmed** — not collected or not yet supplied.

## Data provenance & consent

- Two survey exports: a **participant (student)** form and an **organizer/stakeholder** form.
- **Consent-gated:** responses without clear consent to use anonymized feedback were excluded.
  - Student form: **23 submitted → 20 valid** (3 excluded: two "No", one contradictory
    "Yes, No").
  - Organizer/stakeholder form: **7 submitted → 7 valid** (all consented).
- **Total valid responses: 27** (20 students + 7 organizers/stakeholders).
- **Survey period:** 23 July – 13 August 2026 (earliest to latest valid response).
- Responses are keyed to anonymous codes (`R01`…). The code↔row relationship is **not
  published**. The forms did not collect names/emails; open-ended text was checked and carries
  no identifying information.

## Headline metrics (with denominators)

| Metric | Value | Denominator / basis |
|--------|-------|---------------------|
| Total valid responses | **27** | 20 students + 7 organizers/stakeholders |
| Participant response coverage | **20 of 25** coordinated participants (80%) | 25 coordinated (10 IE + 15 Jasper); 23 submitted, 3 excluded for consent |
| Overall satisfaction (participants) | **4.30 / 5** | mean of 20 participant ratings |
| Ease-of-use rating | **Not collected** | the participant form had **no** ease-of-use question — cannot be calculated (see note) |
| Wallet-setup success | **18 of 19** who attempted (15 easily + 3 with help) | 20 participants; 1 not attempted excluded; 1 did not complete |
| Credential receipt (survey) | **17 of 18** who attempted reported receiving | 20 participants; 2 not attempted excluded; 1 did not complete |
| Credentials issued (system record) | **23** | platform export — see [issuance register](../issuance-evidence/anonymized-issuance-register.md) |
| Verification success (survey) | **18 of 19** who attempted reported success | 20 participants; 1 not attempted excluded (see caveat below) |
| Would use FairWallet again (participants) | **14 Yes · 5 Maybe · 1 No** | 20 participants |
| Perceived usefulness (participants) | **11 Very useful · 7 Useful · 2 Not sure** | 20 participants |
| Institutional value (stakeholders) | **4.57 / 5** | mean of 7 stakeholder ratings |
| Readiness for a larger pilot (stakeholders) | **5 Yes · 2 Maybe · 0 No** (rating mean 4.0/5) | 7 stakeholders; rating 4–5→yes, 3→maybe, 1–2→no |
| Institution would participate again | **6 Yes · 1 Maybe** (conditional) | 7 stakeholders |

> **Ease-of-use note:** the participant survey measured step completion (install / receive /
> verify) and overall satisfaction, but did **not** ask a standalone ease-of-use question, so
> an average ease-of-use score is **not available**. If desired, it could be approximated from
> the step-completion answers — but that would be a derived proxy, not a reported figure, so it
> is left as *Not collected*.

## Satisfaction

- **Survey finding:** mean overall satisfaction **4.30 / 5** across 20 participants.
  Distribution: ten ratings of **5**, eight of **4**, one of **3**, and one low outlier of **1**.
- Participant **perceived usefulness** of a digitally verifiable credential was high: **11 of
  20** "Very useful", **7** "Useful", **2** "Not sure".
- **Stakeholders** rated the pilot stages (n=7): Planning **7 Excellent**; Onboarding **3
  Excellent / 4 Good**; Issuance **4 Excellent / 3 Good**; Verification **4 Excellent / 1 Good
  / 2 Fair**; Technical support **5 Excellent / 2 Good**. Verification remains the **weakest-
  rated stage** (the only stage with "Fair" ratings).
- Main institutional benefit cited (n=7): **faster credential issuance (4)**, reduced
  credential fraud (2), reduced administrative work (1).

## Issues encountered

Participant-reported and organizer-observed problems are reported **separately**.

**Participant-reported problems** — 13 of 20 reported "No problems"; 7 reported at least one:

| Problem | Count |
|---------|-------|
| Wallet installation | 4 |
| Internet or device problem | 3 |
| Instructions were unclear | 2 |
| Verification did not work | 2 |
| QR code or connection | 1 |
| Credential information was incorrect | 1 |
| Privacy or security concern | 1 |

> **Wallet installation** is now the single most-reported participant problem, and
> **connectivity** ("internet or device") is second — both reinforcing the onboarding and
> connectivity improvement areas.

**Organizer-observed problems** (n=7, *observations — not participant experience*): 3 "No
significant problems", 2 "Internet or device problems", 1 "Other", 1 "Privacy or security
concerns".

**Verification caveat (survey vs. records vs. observation):** step-based self-report shows
**18 of 19** participants who attempted verification succeeded, **but** two participants
flagged *"Verification did not work"* and stakeholders rated **verification the weakest stage
(2 of 7 "Fair")**. A system record of issuance does **not** by itself prove verification
succeeded. Verification reliability is therefore treated as a **key improvement area**, not a
solved item.

**Privacy / security signal:** one participant reported a "Privacy or security concern", one
stakeholder observed "Privacy or security concerns", and the issuer operator's single most
important improvement was *"I need it to be very secure…"* — a small but cross-cutting signal,
notable because the credential schemas embed personal data (incl. national ID).

## Suggestions (open-ended themes)

Recurring, evidence-based themes from participant and stakeholder free-text (identifying
information removed, meaning preserved):

1. **Simpler / clearer onboarding** — "make it simple for other users", "instructions were
   unclear", "the system must be easy as much as possible"; specific: *"writing down the key
   phrase is tiring — copy and paste should be possible"*.
2. **Device & connectivity support** — "make the app work on older devices", "improve stable
   Wi-Fi network", "internet or device problem".
3. **Speed / performance** — "reduce processing delays", "faster transaction loading times",
   "speed of the system".
4. **Verification / QR reliability** — "the QR code must be improved", "verification did not
   work".
5. **Security & trust** — "I need it to be very secure so that we rely on it fully".
6. **Scale it up** — "try it on a larger scale like universities and colleges", "try it on
   more users", "let there be continuity".

## Evidence-based improvement areas

Three or more improvement areas, each traced to the evidence above, are documented in the
[Improvement & Iteration Plan](../improvements/improvement-and-iteration-plan.md).
