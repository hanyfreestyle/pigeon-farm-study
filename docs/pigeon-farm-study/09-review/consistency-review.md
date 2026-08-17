# Consistency Review

## Purpose

هذا الملف مخصص لتسجيل ومراجعة التعارضات بين المصادر، أو بين نتائج المراحل، أو بين Business Rules والقرارات التصميمية.

## Current Status

- **Phase:** Phase 1A
- **Conflicts / Variability Items Identified:** 4
- **Unresolved Consistency Issues:** 4 contextual issues carried forward
- **Review Status:** Phase 1A research contradictions documented; no software decisions made.

## Conflict Register

| Conflict ID | Topic | Source / File A | Source / File B | Description | Resolution | Status |
|---|---|---|---|---|---|---|
| CON-001 | Egg / reproductive cycle length | BMC Veterinary Research 2025; local Egyptian/Indonesian references | Silver King / other production studies; early-weaning experimental groups | Reported cycle length varies from roughly 51–53 days in some local systems to around 37–39 days in others, and can be shortened dramatically by hatch-day separation/early rearing interventions. | Treat cycle length as contextual; preserve breed, definition and rearing method. Do not create a universal constant. Detailed lifecycle definition deferred to Phase 1B/3. | Open — Contextual Resolution |
| CON-002 | Natural parental rearing vs early artificial rearing | Natural/28-day parent-reared production | Early-weaning / hatch-day separation research | Early separation can increase breeder reproductive throughput while reducing squab growth and, at hatch-day separation in the cited Egyptian experiment, increasing mortality. | Separate breeder throughput from squab growth/survival/economic/welfare outcomes. No single approach declared superior. | Open — Requires Target-System Validation |
| CON-003 | Housing model and commercial suitability | Egyptian commercial mud dovecote / wooden loft survey | Cage vs communal fly-pen comparative research | Commercial production exists in communal Egyptian systems, while one controlled study reported higher productivity/economics for pair cages than communal pens under its conditions. | Do not select a universal housing model. Validate target Egyptian farm types and analyze workflows per housing model. | Open — Field Validation Required |
| CON-004 | Summer production / seasonality | 2023 breeding-cycle review describing pigeons as non-seasonal breeders | Egyptian 2018 heat-stress study showing reduced egg production, fertility and hatchability in summer heat stress | “Non-seasonal breeder” can coexist with strong environmentally driven summer production decline. | Reject the simplistic claim of mandatory biological summer shutdown; treat heat/environment as performance modifiers and validate local severity. | Open — Contextual Resolution |

## Review Rule

أي تعارض مؤثر يظهر لاحقًا يجب تسجيله هنا، مع عدم إخفائه أو حسمه بتخمين غير موثق.

### Interpretation Rule

ليس كل اختلاف رقمي بين مصدرين تناقضًا علميًا. قد يكون الاختلاف نتيجة:

- Breed / strain.
- Housing system.
- Parent load (number of squabs reared).
- Natural vs artificial incubation or weaning.
- Season / temperature / lighting.
- Diet.
- Breeder age.
- Different definitions or denominators for the same named metric.

يجب الاحتفاظ بالسياق قبل محاولة توحيد الأرقام.
