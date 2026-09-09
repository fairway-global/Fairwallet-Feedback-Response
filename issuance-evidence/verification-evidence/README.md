# Verification Evidence

**Acceptance criterion 8 (verification side).**

> **Status:** 🟡 Documented limitation + redacted screenshots to be added.

## Documented limitation (system-side verification)

Comprehensive **system-side verification records covering all 23 issued credentials are not
available.** During the pilot:

- **Some participants did not have a smartphone**, so they could not install FairWallet and go
  through the credential-presentation/verification step on their own device.
- **Some participants did not complete wallet setup or issuance**, so no verification could
  follow for them.

As a result, verification was exercised for a subset of participants rather than the entire
cohort, and a complete system-side verification log for every issued credential was not captured.

This is stated as an honest limitation. It is **distinct** from the survey self-report in the
[Feedback Analysis](../../feedback/feedback-analysis.md) (18 of 19 respondents who *attempted*
verification reported success). **The survey figure is not a system-wide verification rate for
all 23 issued credentials.**

## Redacted screenshots

**Present:** `Redacted verifier dashboard activity.png` — an anonymized verifier-workspace
dashboard (aggregate activity; contact name blurred; a `@test.com` operator account). No holder
DIDs, credential IDs, or personal data.

**Withheld (not published):** a "completed verification" detail screenshot and per-participant
credential-detail screenshots exposed holder DIDs / credential IDs / names; they are held in
`.private-input/` (git-ignored) and are **not** published. Verification is therefore evidenced
by this dashboard, the documented limitation above, and the survey self-report in the
[feedback analysis](../../feedback/feedback-analysis.md) (18 of 19 respondents who attempted).
