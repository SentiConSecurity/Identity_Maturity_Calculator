# Changelog

All notable changes to the Identity Maturity Calculator are documented in this file.

The workbook itself is versioned independently in its filename (e.g. `Identity_Maturity_Assessment_v2.0.xlsx`); this file tracks what changed and why, for anyone tracking the project on GitHub.

## v1.0.0 — Initial Public Release

Originally published December 18, 2018 on johnmasserini.com.

## v2.0.0 — Initial Public Release

This is the first version of the Identity Maturity Calculator published to GitHub, alongside full documentation, and wiki content in support of the book ***Building the Enterprise Identity Infrastructure***

- 9-domain, 36-question identity security maturity assessment, scored on a 0–5 scale adapted from the SEI-CMMI framework.
- Domains: Identity Foundations & Data Quality, Identity Governance & Lifecycle, Access Architecture & Authentication, Privileged & Elevated Access, Non-Human & Workload Identity, Identity Security Operations, Contextual Trust & Adaptive Access, AI & Autonomous Identity, and Identity Technical Debt.
- Domain Radar spider chart with automatic per-domain averaging.
- Priority View tab that dynamically re-sorts all 36 questions lowest-score-first to drive remediation planning.
- Input validation (whole numbers, 0–5) and a red-amber-green color scale on all score entry cells.
- Full documentation set: README, wiki (Directions, Maturity Levels, Rationale, References), and reproducible Python build scripts.

> **Note:** this repository's history begins at v2.0.0 of the workbook. 

---

### Versioning Convention

This project follows a simplified `MAJOR.MINOR.PATCH` convention for the workbook itself:

- **MAJOR** — structural changes: a domain added/removed/renamed, a question added/removed, or a change to the scoring scale.
- **MINOR** — content changes that don't alter structure: reworded questions or expectations, new guidance in Instructions, chart styling changes.
- **PATCH** — corrections: typo fixes, formula fixes, formatting-only changes.

Each release should be tagged in git (`git tag v2.0.0`) and published as a [GitHub Release](https://github.com/SentiConSecurity/Identity_Maturity_Calculator/releases) with the workbook attached as a binary asset — do not rely on GitHub's auto-generated source archives, which won't contain the `.xlsx` file unless it's committed to the repository.
