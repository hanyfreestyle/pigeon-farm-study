# Risk Register

| Risk ID | Description | Probability | Impact | Mitigation | Related Phase | Phase 1 Review | Status |
|---|---|---|---|---|---|---|---|
| RSK-001 | القفز مبكرًا إلى تصميم الجداول أو Software Entities قبل فهم المجال. | Medium | High | Domain-First rule + approved baseline before technical modeling. | Phases 1–7 | Reduced by completing Phase 1 baseline; remains relevant until Data Modeling. | Active — Reduced |
| RSK-002 | اعتبار ممارسة مزرعة واحدة Business Rule عامة. | High | High | Keep practice/context/evidence classification and field validation. | Phases 1–6 | Phase 1 confirmed major variation by housing, breed and management. | Active |
| RSK-003 | الاعتماد على مصادر ضعيفة أو تجارية منفردة لمعلومة مهمة. | Low-Medium | High | Evidence policy; prioritize peer-reviewed/official sources. | Phases 1–6 | Phase 1 used a strong academic/official base with source limitations documented. | Controlled — Monitor |
| RSK-004 | Scope Creep نحو الهواية/السباق/الزينة أو مواضيع لاحقة. | Medium | Medium | Future Research Queue + phase boundaries. | All Phases | Scope stayed aligned in Phase 1. | Active — Controlled |
| RSK-005 | تضارب المصطلحات أو استخدام نفس المصطلح بمعانٍ مختلفة. | Medium | High | Normalized terminology + Ambiguous Domain Terms section. | Phases 1–6 | Significantly reduced by Phase 1C; Production Cycle/Weaning/Hatchability still require explicit context. | Active — Reduced |
| RSK-006 | بناء MVP كأداة تسجيل فقط قبل فهم القرارات التشغيلية. | Medium | High | Delay MVP until Domain + System Analysis and tie features to decisions. | Phases 6–8 | Not yet addressed by design; Phase 1 improves future basis. | Active |
| RSK-007 | تمثيل Production Cycle كدورة غير متداخلة. | Medium | Very High | Phase 1B/1C established overlapping cycles as baseline; Phase 3 must define analytical anchors. | Phases 1B–7 | Domain misunderstanding substantially mitigated; software risk remains. | Active — Reduced |
| RSK-008 | نقل intensive/industrial practices من سياق أجنبي إلى مصر باعتبارها الوضع القياسي. | High | High | Separate biology from practice; preserve Egyptian evidence and validate target farms. | Phases 1–6 | Still important; early weaning and controlled pair systems are not assumed to be universal locally. | Active |
| RSK-009 | استخدام benchmark واحد للعمر/الوزن/الدورة/الخصوبة دون سياق. | High | High | Benchmark classification and context requirements. | Phases 1–7 | Phase 1C classified stable ranges vs context-dependent observations. | Active — Reduced |
| RSK-010 | تفسير انخفاض الصيف كتوقف موسمي بيولوجي إلزامي. | Low-Medium | High | Treat heat/environment as modifiers and validate local magnitude. | Phases 1 / 4 / 6 | Conceptual contradiction resolved; local operational severity remains open. | Active — Reduced |
| RSK-011 | اعتبار رقم القفص/العش هوية دائمة للطائر أو الزوج. | Medium | High | Keep individual/pair/location identification separate; validate local practice in Phase 2. | Phases 1B–2 / 7 | Phase 1 clarified the distinction; target practice remains unknown. | Active |

## Phase 1 Risk Review Conclusion

Phase 1 reduced the largest **knowledge-structure risks**: premature modeling, cycle linearization, terminology ambiguity and benchmark universalization. The main remaining risks now depend on **field validation and later domain/system analysis**, especially housing models, local identification, market specification, pair/replacement rules and Egyptian operational practices.
