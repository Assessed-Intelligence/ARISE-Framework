# Changelog

Material changes to the ARISE Framework™ control library and crosswalks. Control and requirement IDs are permanent; see [framework/controls/README.md](framework/controls/README.md) for stability rules.

## v2.0.0 — 2026-10-08

### Added

- 64 new prioritized requirements across 17 existing controls. The published library grows from 889 to 953 requirements.

| Control | Domain | Title | v1.0.0 | v2.0.0 |
|---------|--------|-------|-------:|-------:|
| `G.GV.A-06` | GOVERN | Transparency | 4 | 7 |
| `G.GV.S-03` | GOVERN | Response & Resilience Standards | 7 | 10 |
| `G.GV.S-04` | GOVERN | AI Standards | 9 | 15 |
| `G.LR-02` | GOVERN | Intellectual Property (IP) Management | 9 | 15 |
| `G.RM-02` | GOVERN | Risk Appetite and Tolerance | 7 | 10 |
| `G.ST.B` | GOVERN | System Boundaries | 6 | 9 |
| `G.ST.S-03` | GOVERN | Regulatory Scope | 5 | 11 |
| `M.DV-01` | MANAGE | AI System Lifecycle | 8 | 11 |
| `M.PR` | MANAGE | Privacy Program | 8 | 11 |
| `M.RM-01` | MANAGE | Third-Party Risk Management | 9 | 13 |
| `M.RP` | MANAGE | Reporting | 8 | 11 |
| `I.DG-01` | IDENTIFY | Data Mapping | 7 | 10 |
| `P.AC.S-01` | PROTECT | Datasets & Tagging | 7 | 10 |
| `P.AC.S-02` | PROTECT | AI-Specific Attack Vectors | 8 | 14 |
| `P.DS-01` | PROTECT | Classification & Handling | 8 | 11 |
| `R.LL` | RESPOND | Incident Lessons Learned | 6 | 9 |
| `V.TE-02` | VALIDATE | Evaluation | 8 | 11 |

### Changed

- `requirement_count` updated in `framework/controls/*.csv` for the controls above.
- Requirement totals updated in `README.md` and `framework/controls/README.md`.
- `CITATION.cff` version bumped to 2.0.0.

### Unchanged

- No controls, taxonomy nodes, or requirements were added, retired, or renumbered beyond the additions above. Existing requirement text and priority tiers are unchanged.
- Crosswalks are unchanged and remain mapped at the control level.

## v1.0.0 — 2026-07-11

- Initial public release: 128 controls, 889 requirements, 38-node taxonomy, and 40 crosswalks.
