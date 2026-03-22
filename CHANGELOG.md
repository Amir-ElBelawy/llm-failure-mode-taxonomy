# Changelog

A running record of additions, revisions, and reclassifications to the taxonomy.
Entries are listed newest first. Each version corresponds to a tagged release on GitHub.

The taxonomy is a living document — models update, new failure modes emerge, and
existing mechanisms get better explanations as more sessions accumulate. This log
exists so readers can see what changed and why, not just what the current state is.

---

## [v1.0] — 2026-03-20 — Initial public release

**Archive:** 204 DeepSeek sessions + 21 Claude sessions — 2023–2026

### Added
- **Category 1 — Context & Memory** (4 failure modes)
  - 1.1 Context Drift
  - 1.2 Role Collapse
  - 1.3 History Misreading
  - 1.4 Session State Loss

- **Category 2 — Output Quality** (5 failure modes)
  - 2.1 Surface Reading
  - 2.2 Preamble Bloat
  - 2.3 Theoretical vs Operational Output
  - 2.4 Premature Conclusion
  - 2.5 Compression Bias

- **Category 3 — Identity & Persona** (4 failure modes)
  - 3.1 Anthropomorphization Drift
  - 3.2 Persona Misrepresentation
  - 3.3 Character Softening Under Pressure
  - 3.4 Persona Over-Commitment

- **Category 4 — Safety & Compliance** (3 failure modes)
  - 4.1 Over-Refusal
  - 4.2 Consent Frame Blindness
  - 4.3 Scope Miscalculation

- **Category 5 — Reasoning** (4 failure modes)
  - 5.1 Reasoning Shortcuts
  - 5.2 False Confidence
  - 5.3 Confirmation Loop
  - 5.4 Motivated Reasoning

- **Category 6 — Calibration** (4 failure modes)
  - 6.1 Speed-Depth Tradeoff
  - 6.2 Update-Induced Degradation
  - 6.3 Inference Offloading
  - 6.4 Linguistic Hedging Overload

- **Category 7 — Cross-Platform Behavioral Differences** (2 failure modes)
  - 7.1 Platform-Specific Safety Profiles
  - 7.2 Alignment-Quality Inversion

- Summary table covering all 26 failure modes with prevalence and single-session flags
- Diagnostic flowchart (Mermaid) for real-time failure identification
- Methodology note on active monitoring vs post-hoc analysis
- Disclosure: complete unfiltered archive — no sessions pre-selected for study

### Notes
- Category 6 entries (Calibration) are upstream causes, not terminal failure modes —
  documented separately because users need to diagnose them to understand why other
  failures appear or worsen
- Cross-platform claims in Category 7 are qualified throughout due to archive
  imbalance (204 DeepSeek vs 21 Claude sessions)
- Update-Induced Degradation (6.2) observed once — included because the diagnostic
  value outweighs the limited sample

---

## Versioning convention

Versions follow this logic for a research taxonomy rather than software:

| Increment | Meaning |
|---|---|
| Major (v2.0) | New category added, or significant structural reorganization |
| Minor (v1.1) | New failure mode added within an existing category |
| Patch (v1.0.1) | Mechanism revised, example updated, wording corrected |

Community contributions that add a new failure mode increment the minor version.
Mechanism corrections or example updates increment the patch version.
The contributor's name appears in both the entry and the changelog entry for that version.

---

*Amir El Belawy — Mansoura University*
