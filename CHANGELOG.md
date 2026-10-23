# Changelog

Material changes to the ARISE Framework™ control library and crosswalks. Control and requirement IDs are permanent; see [framework/controls/README.md](framework/controls/README.md) for stability rules.

## v2.1.0 — 2026-10-23

Crosswalk correction release. The control library (controls, requirements, taxonomy) is unchanged from v2.0.0.

### Fixed

- **Truncated rationales.** In v2.0.0, rationale text in many crosswalks was cut off at the first comma because of a delimiter fault in the export pipeline. Every affected crosswalk has been regenerated from corrected source mappings and now carries the complete rationale.
- **Retired control IDs.** 88 crosswalk rows referenced control IDs that are not in the published library (for example `D.IA`, `D.AE-04`, `I.OD-02`, `M.MO-*`, `P.AC.I-*`, `S.VR-02`). All crosswalk rows now resolve to a published control or taxonomy node. Internal Audit is referenced as `V.IA`, and vendor risk as `M.RM-01`.
- **ISO/IEC 27701 file name.** `arise-to-iso-22701.csv` is renamed `arise-to-iso-27701.csv` to match the standard's actual number. Update any links or tooling that point to the old path.
- Idaho crosswalk column `Regualtion` is renamed `Regulation`, and the US States AI Consciousness crosswalk no longer has a trailing empty column.

### Changed

Mappings were re-reviewed and corrected in the following crosswalks. Row counts are mapped rows; one control can appear on more than one row when it maps to several external clauses.

| Source | File | v2.0.0 rows | v2.1.0 rows |
|--------|------|------:|------:|
| AIUC-1 Certificate | `arise-to-aiuc-1-certificate.csv` | 74 | 69 |
| BSI C5 :2020 | `arise-to-bsi-c5-2020.csv` | 82 | 127 |
| California AB 2013 & SB 942 (Private Sector AI Governance) | `arise-to-california-ab-2013-sb-942-private-sector-ai-governance.csv` | 8 | 8 |
| California SB 53 (Transparency in Frontier AI Act) | `arise-to-california-sb-53-transparency-in-frontier-ai-act.csv` | 8 | 8 |
| Colorado AI Act | `arise-to-colorado-ai-act.csv` | 10 | 11 |
| Colorado SB 26-189 | `arise-to-colorado-sb-26-189.csv` | 6 | 6 |
| ETSI Standard - EN 304 223 - V2.1.1 | `arise-to-etsi-standard-en-304-223-v2-1-1.csv` | 44 | 43 |
| EU 2016/679 (GDPR) | `arise-to-eu-2016-679-gdpr.csv` | 25 | 35 |
| EU AI Act | `arise-to-eu-ai-act.csv` | 57 | 73 |
| ForHumanity CORE | `arise-to-forhumanity-core.csv` | 75 | 75 |
| ForHumanity Cybersecurity | `arise-to-forhumanity-cybersecurity.csv` | 55 | 55 |
| Health Sector Coordinating Council (HSCC) AI TPR  and Supply Chain | `arise-to-health-sector-coordinating-council-hscc-ai-tpr-and-supply-ch.csv` | 50 | 49 |
| HIPAA Security Rule | `arise-to-hipaa-security-rule.csv` | 24 | 35 |
| Idaho (SB 1227 & SB 1297) | `arise-to-idaho-sb-1227-sb-1297.csv` | 10 | 10 |
| ISO 27001 | `arise-to-iso-27001.csv` | 71 | 98 |
| ISO 42005 | `arise-to-iso-42005.csv` | 6 | 7 |
| ISO 42006 | `arise-to-iso-42006.csv` | 4 | 4 |
| ISO 5259 | `arise-to-iso-5259.csv` | 3 | 4 |
| Local Law 144 - NYC | `arise-to-local-law-144-nyc.csv` | 5 | 5 |
| NIST 800-53 | `arise-to-nist-800-53.csv` | 83 | 91 |
| NIST AI RMF | `arise-to-nist-ai-rmf.csv` | 65 | 65 |
| OECD Due Diligence Guidance for Responsible AI | `arise-to-oecd-due-diligence-guidance-for-responsible-ai.csv` | 14 | 14 |
| OMB M-25-21 | `arise-to-omb-m-25-21.csv` | 5 | 7 |
| PCI DSS v4.0 | `arise-to-pci-dss-v4-0.csv` | 27 | 38 |
| prEN 18229-2 -- Trustworthiness Part 2 (Art. 15 accuracy) | `arise-to-pren-18229-2-trustworthiness-part-2-art-15-accuracy.csv` | 128 | 128 |
| prEN 18284 -- Data Quality & Governance (Art. 10) | `arise-to-pren-18284-data-quality-governance-art-10.csv` | 128 | 128 |
| prEN 18286 -- QMS for HRAIS (Art. 17) | `arise-to-pren-18286-qms-for-hrais-art-17.csv` | 128 | 128 |
| Singapore Model AI Governance Framework | `arise-to-singapore-model-ai-governance-framework.csv` | 16 | 16 |
| Texas Responsible AI Governance Act (HB 2060 / TRAIGA) | `arise-to-texas-responsible-ai-governance-act-hb-2060-traiga.csv` | 7 | 7 |
| TX TRAIGA - HB 149 | `arise-to-tx-traiga-hb-149.csv` | 7 | 7 |
| US States AI Consciousness | `arise-to-us-states-ai-consciousness.csv` | 32 | 32 |
| US States Deepfake & AI Harassment | `arise-to-us-states-deepfake-ai-harassment.csv` | 5 | 5 |

`arise-to-iso-42001.csv` and `arise-to-iso-27701.csv` only received the control ID corrections above. The rest of the crosswalks are unchanged.

### Release metadata

- `CITATION.cff` version bumped to 2.1.0, and `crosswalks/README.md` index row counts updated.

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
