# Assumptions Register

> Assumptions are reviewed at Phase 1 exit. A `Validated` assumption is supported sufficiently for the stated purpose; it is not automatically a universal biological fact.

| Assumption ID | Description | Reason | Related Module | Risk if Wrong | Validation Method | Phase 1 Review | Status |
|---|---|---|---|---|---|---|---|
| ASM-001 | الدراسة موجهة أساسًا لمزرعة تجارية هدفها إنتاج الزغاليل/الحمام اللاحم، وليس للهواية أو السباق أو الزينة. | Scope adopted in Phase 0 and maintained through Phase 1. | Overall Scope | Scope drift. | User-approved project scope + Phase 1 evidence focus. | Phase 1 research remained consistently aligned with commercial meat/squab production. | Validated |
| ASM-002 | الممارسات التشغيلية تختلف بين المزارع، لذلك لا تمثل ممارسة واحدة جميع المزارع. | Prevent local practice becoming a universal rule. | All Domain Modules | Incorrect business rules and benchmarks. | Compare multiple sources, systems, breeds and Egyptian evidence. | Strongly supported: housing, cycle timing, market reference, identification, early weaning and performance vary by context. | Validated |
| ASM-003 | النظام النهائي سيحتاج إلى الاحتفاظ بتاريخ تشغيلي كافٍ لتحليل الأداء، لكن مستوى هذا التاريخ لم يُحدد بعد. | Repeated pair/clutch/squab performance implies value in history. | Production / Performance / Audit | Later design may be under/over-specified. | Resolve after production and reporting analysis. | Phase 1 strengthens the need for historical event context, but exact retention/granularity is a future system-design decision. | Provisional |
| ASM-004 | التقنية المستهدفة Laravel 12 + PHP 8.2+ + Filament 4 + MySQL مناسبة كسياق مبدئي، بشرط ألا تفرض نموذجًا على المجال. | Future technical constraint supplied by project owner. | Technical Architecture | Domain requirements may call for architectural adjustment. | Re-evaluate in Phase 7 after System Analysis. | Not a domain assumption and was not tested in Phase 1. | Provisional |

## Phase 1 Assumption Review Conclusion

- `ASM-001` and `ASM-002` are **Validated** for continuing the study.
- `ASM-003` remains **Provisional** because Phase 1 confirms the value of history but not its software representation or retention policy.
- `ASM-004` remains **Provisional** and must not influence domain modeling before the technical-design phase.
- No Phase 1 assumption was rejected.
