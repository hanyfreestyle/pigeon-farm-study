# Pigeon Farm Management System — Master Study File

> Central source of truth for study status, decisions, evidence policy, scope, risks, assumptions, open questions, and phase transitions.

## Project Vision

دراسة وتحليل وتصميم نظام متكامل لإدارة مزارع الحمام التجاري مع التركيز على **Commercial Meat Pigeon / Squab Production**. يبدأ المشروع بفهم المجال والعمليات الفعلية ثم ينتقل لاحقًا إلى Business Analysis وData Modeling وSystem Design وMVP وTechnical Architecture.

## Study Objectives

- فهم مجال إنتاج الزغاليل التجاري بصورة موثقة.
- توثيق دورة الإنتاج والعمليات والقرارات التشغيلية.
- فصل الحقائق البيولوجية عن الممارسات التشغيلية المتغيرة.
- فهم Domain Entities قبل أي Software Entities.
- استخراج Business Rules لاحقًا من التحليل لا من الافتراضات.
- الوصول إلى Data Model وSystem Design مبنيين على الواقع التشغيلي.
- تعريف MVP واضح بعد اكتمال التحليل السابق له.

## Scope

### In Scope

**Commercial Meat Pigeon / Squab Production** مع دراسة الجوانب المشتركة من أنماط تربية أخرى فقط عندما تكون لازمة لفهم المجال الأساسي.

### Out of Scope During Domain Research

- Database Design / ERD.
- Software Entities / Models.
- Migrations.
- Status Enums.
- APIs / UI / Filament.
- MVP implementation.
- Software Architecture.
- Coding.

## Study Methodology

**Research → Domain Understanding → Operational Analysis → Business Analysis → Business Rules → Data Modeling → System Design → MVP Definition → Technical Architecture → Final Review**

المبدأ الحاكم: **التحليل يولّد التصميم، وليس العكس.**

## Study Phases

| Phase | Name | Status | Files | Dependencies | Review Status | Notes |
|---|---|---|---|---|---|---|
| Phase 0 | Study Initialization | Completed | `MASTER.md`, review files, placeholders | None | Approved by transition | Initialization complete. |
| Phase 1 | Domain Research | Completed — Awaiting Review | `01-domain-research/*`, review files, `DOMAIN-BASELINE.md` | Phase 0 | User Review Required | Exit criteria met; not Approved yet. |
| Phase 2 | Farm Structure & Core Domain | Pending | `02-farm-structure/*` | Phase 1 approval | Pending | Do not start before user approval. |
| Phase 3 | Production Analysis | Pending | `03-production/*` | Phases 1–2 | Pending | Egg, hatch, squab and performance analysis. |
| Phase 4 | Health & Feed | Pending | `04-health-feed/*` | Phases 1–3 | Pending | Health, treatments, mortality, feed. |
| Phase 5 | Operations & Finance | Pending | `05-operations-finance/*` | Phases 1–4 | Pending | Inventory, purchasing, sales, financials. |
| Phase 6 | System Analysis | Pending | `06-system-analysis/*` | Phases 1–5 | Pending | KPIs, reports, alerts, roles, rules, domain events. |
| Phase 7 | Technical Design | Pending | `07-technical-design/*` | Phase 6 | Pending | Data model, relationships, architecture, audit. |
| Phase 8 | MVP Definition | Pending | `08-mvp/*` | Phases 6–7 | Pending | MVP and future AI. |
| Phase 9 | Final Review & Consolidation | Pending | `09-review/*`, `FINAL-STUDY.md` | Phases 1–8 | Pending | Final consolidation after approvals. |

## Phase 1 Subphase Progress

| Subphase | Name | Status | Primary File | Notes |
|---|---|---|---|---|
| Phase 1A | Commercial Pigeon Farming Domain Research | Completed | `01-domain-research/commercial-pigeon-farming.md` | Commercial models, pair, nests, records, benchmarks, Egypt. |
| Phase 1B | Detailed Pigeon Production Lifecycle | Completed | `01-domain-research/production-lifecycle.md` | Detailed timeline, overlap, failures, events, Egyptian timing evidence. |
| Phase 1C | Domain Terminology, Evidence Consolidation & Validation Review | Completed — Awaiting Review | `01-domain-research/DOMAIN-BASELINE.md` | Baseline created; terminology/evidence/risks/assumptions/consistency reviewed. |

## Decision Log

| Decision ID | Date | Phase | Decision | Reason | Impact | Status |
|---|---|---|---|---|---|---|
| DEC-001 | 2026-08-17 | Phase 0 | Primary scope is Commercial Meat Pigeon / Squab Production. | Prevent scope drift. | Guides research and analysis. | Approved |
| DEC-002 | 2026-08-17 | Phase 0 | Do not design Software Entities or Database Tables before understanding Domain Entities and workflows. | Prevent premature design. | Data design becomes an output of analysis. | Approved |
| DEC-003 | 2026-08-17 | Phase 0 | Target technical context is Laravel 12 + PHP 8.2+ + Filament 4 + MySQL, without early implementation. | Preserve future technical context without driving domain analysis. | Re-evaluate in Phase 7. | Approved |
| DEC-004 | 2026-08-17 | Phase 0 → 1 | Explicit Phase 1A instruction authorized Phase 0 completion and transition to Phase 1. | Phase 0 requirements were complete. | Phase 1 began formally. | Approved |
| DEC-005 | 2026-08-17 | Phase 1C | Phase 1 Domain Baseline is complete enough for user review; remaining local uncertainties are preserved as Field Validation rather than blocking consolidation. | Core biology/lifecycle is coherent, while local operational choices remain intentionally open. | Phase 1 can be marked Completed — Awaiting Review, but not Approved. | Approved |

## Research Evidence Policy

Important information is classified as:

- **Verified Fact**
- **Strong Evidence**
- **Moderate Evidence**
- **Industry Practice**
- **Expert/Producer Practice**
- **Assumption**
- **Design Decision**
- **Open Question / Requires Field Validation**

Rules:

- Never convert an assumption into a fact without evidence.
- Record meaningful source conflicts rather than hiding them.
- Preserve context when numbers vary by breed, housing, management, climate, feeding, market or measurement definition.
- Prefer peer-reviewed, university, government, veterinary, agricultural and recognized professional sources.
- Blogs/forums may supplement practice discovery but not serve as the only evidence for critical facts.

## Source Tracking

```text
Source ID: SRC-XXX
Source: <Title>
URL: <URL>
Organization / Author: <Organization / Author>
Publication Date: <Date or Unknown>
Access Date: <Date>
Reliability: High | Medium | Low
Information Used: <Specific use>
Notes: <Limitations/context>
```

## Working Rules for Future Phases

1. Read `MASTER.md`.
2. Read related prior phase files.
3. Review `09-review/open-questions.md`.
4. Review `09-review/assumptions.md`.
5. Do not repeat approved research without a reason.
6. Do not change an Approved decision without a new Decision Log entry.
7. Record source contradictions.
8. Record new assumptions.
9. Record new open questions.
10. Update phase status and `STUDY-LOG.md` after every major task.

## Domain-First Design Rule

**Do not design Software Entities before understanding Domain Entities. Do not design Database Tables before the relevant workflows are analyzed.**

Examples such as `Pigeon = table` or `Pair = table` are prohibited assumptions until the appropriate technical-design phase.

## Phase 1 Domain Baseline — Approved for Review, Not Yet User-Approved

Primary consolidation file:

`docs/pigeon-farm-study/01-domain-research/DOMAIN-BASELINE.md`

Core Phase 1 conclusions:

1. Squab production is dependent on biparental reproduction and care.
2. Breeding pair is a central operational unit.
3. Two eggs is the dominant clutch pattern.
4. Egg laid, clutch completion, incubation start and hatch are distinct events.
5. Incubation is broadly stable around 17–20 days, while exact calculation anchor requires explicit definition.
6. Natural market/weaning references cluster around 3–4 weeks, but market readiness is contextual.
7. Production cycles can overlap: previous squabs may still be reared while the next clutch begins.
8. Double nest is a documented mechanism supporting overlap.
9. Failed cycles can restart differently from successful full rearing cycles.
10. Housing, identification, market specification, replacement rules, pair rules and benchmarks vary by context and require local validation.
11. Egyptian evidence is substantial enough to inform the baseline but not sufficient to standardize all current commercial practice nationally.

## Future Research Queue

| Queue ID | Topic | Recommended Phase | Status | Notes |
|---|---|---|---|---|
| FRQ-001 | Detailed egg-management workflow | Phase 3 | Partially Researched | Lifecycle basis exists; management detail later. |
| FRQ-002 | Detailed squab growth/weaning/market workflow | Phase 3 | Partially Researched | Requires market validation. |
| FRQ-003 | Disease, vaccination, treatment, quarantine, biosecurity | Phase 4 | Queued | No medical protocol defined yet. |
| FRQ-004 | Feed formulation and nutritional strategy | Phase 4 | Queued | Context-dependent. |
| FRQ-005 | Feed inventory/purchasing/supplier operations | Phase 5 | Queued | Operational/financial scope later. |
| FRQ-006 | Formal KPI definitions and benchmark normalization | Phase 6 | Queued | Must preserve formulas/context. |
| FRQ-007 | Software representation of bird/pair/nest/clutch/overlap | Phase 7 | Queued | Explicitly prohibited before domain/system analysis. |
| FRQ-008 | Artificial incubation / early-separation optional pathway | Phase 3 | Partially Researched | Adoption in target Egyptian farms requires validation. |

## Assumptions Summary after Phase 1

- ASM-001: Validated.
- ASM-002: Validated.
- ASM-003: Provisional.
- ASM-004: Provisional.

See `09-review/assumptions.md`.

## Risk Summary after Phase 1

The largest knowledge risks were reduced through consolidation, especially premature modeling, terminology ambiguity, linear-cycle assumptions and benchmark universalization. Field-dependent risks remain active around Egyptian production practice, housing, identification, market requirements, and operational thresholds.

See `09-review/risks.md`.

## Open Questions Priority

- **Must answer before Farm Structure:** OQ-001, OQ-002, OQ-014, OQ-016.
- **Must answer before Data Model:** OQ-003, OQ-007, OQ-008, OQ-017, OQ-018, OQ-020, OQ-021.
- **Must answer before MVP:** OQ-004, OQ-006, OQ-009, OQ-010, OQ-015, OQ-019.
- **Can defer:** OQ-005.
- **Optional:** OQ-011, OQ-012, OQ-013.

## Phase 1 Exit Criteria

- [x] Terminology reviewed.
- [x] Domain facts classified.
- [x] Major contradictions documented.
- [x] Production Lifecycle consolidated.
- [x] Overlapping cycles documented.
- [x] Egyptian context separated from international evidence.
- [x] Benchmarks classified.
- [x] Open Questions prioritized.
- [x] Assumptions reviewed.
- [x] Risks reviewed.
- [x] `DOMAIN-BASELINE.md` created.
- [x] Consistency Review completed.

## Current Study Position

- **Current phase:** Phase 1 — Domain Research.
- **Current status:** **Completed — Awaiting Review**.
- **Phase 1 approval status:** **Not Approved yet**.
- **Required next action:** User reviews/approves Phase 1 baseline.
- **Next recommended phase after approval:** **Phase 2 — Farm Structure & Pigeon Management Domain Analysis**.
- **STOP CONDITION:** Do not start Phase 2, Farm Structure Analysis, Database Design, Architecture, MVP or Coding until explicit user approval/instruction.
