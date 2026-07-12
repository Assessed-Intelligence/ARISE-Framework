# ARISE Control Library

The ARISE Framework™ control library: 128 controls across seven domains, with 889 prioritized requirements published in full. The library is organized as a taxonomy; 38 parent nodes group related controls (see `../taxonomy.csv`), and every control belongs to one of the seven domains.

## Structure

- `controls/{domain}.csv` — the 128 controls, one file per domain
- `requirements/{domain}.csv` — all 889 requirements, keyed to their control, with priority tiers
- `../taxonomy.csv` — the 38 parent nodes that organize the control hierarchy

## Domain Summary

| Domain | Controls | Requirements |
|--------|----------|--------------|
| GOVERN | 43 | 295 |
| MANAGE | 13 | 102 |
| IDENTIFY | 11 | 80 |
| PROTECT | 23 | 158 |
| DETECT | 11 | 74 |
| RESPOND | 17 | 116 |
| VALIDATE | 10 | 64 |
| **Total** | **128** | **889** |

## Controls Schema

| Column | Description |
|--------|-------------|
| `control_id` | Stable identifier (e.g., `G.AC-01`, `D.AD`) |
| `parent_id` | Parent taxonomy node, where one exists |
| `domain` | One of: GOVERN, MANAGE, IDENTIFY, PROTECT, DETECT, RESPOND, VALIDATE |
| `title` | Short control name |
| `objective` | What the control is intended to ensure, stated as an outcome |
| `requirement_count` | Number of requirements for the control |

## Requirements Schema

| Column | Description |
|--------|-------------|
| `requirement_id` | Stable identifier (e.g., `D.AD-req-01`) |
| `control_id` | The control this requirement belongs to |
| `priority` | Priority tier assigned by the framework; tier 1 is foundational |
| `requirement` | The requirement statement |

Implementation rationale, evidence requirements, and annotated framework mappings are maintained by Assessed Intelligence and available through engagements and commercial licensing.

## Stability Rules

Control and requirement IDs are permanent; a retired item is marked deprecated rather than reused. Adopters may rely on these IDs as stable references in policies, crosswalks, and tooling.

---

ARISE™ – Assurance of Responsible, Innovative & Secure Environments © Assessed Intelligence LLC
