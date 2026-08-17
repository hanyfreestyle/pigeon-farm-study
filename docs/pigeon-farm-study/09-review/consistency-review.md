# Consistency Review

## Purpose

هذا الملف مخصص لتسجيل ومراجعة التعارضات بين المصادر، أو بين نتائج المراحل، أو بين Business Rules والقرارات التصميمية.

## Current Status

- **Phase:** Phase 1B
- **Conflicts / Variability Items Identified:** 9
- **Unresolved Consistency Issues:** Context-dependent items carried forward
- **Review Status:** Phase 1A + Phase 1B evidence conflicts documented; no software decisions made.

## Conflict Register

| Conflict ID | Topic | Source / File A | Source / File B | Description | Resolution | Status |
|---|---|---|---|---|---|---|
| CON-001 | Egg / reproductive cycle length | BMC Veterinary Research 2025; local Egyptian/Indonesian references | White Mirthys / other production studies; early-weaning experimental groups | Reported cycle length varies substantially and can be shortened by early separation. | Treat cycle length as contextual; preserve breed, definition and rearing method. | Open — Contextual Resolution |
| CON-002 | Natural parental rearing vs early artificial rearing | Natural/28-day parent-reared production | Early-weaning / hatch-day separation research | Early separation can increase breeder throughput while changing squab growth, mortality, labor and welfare. | Separate breeder throughput from squab outcomes; no approach declared universally superior. | Open — Requires Target-System Validation |
| CON-003 | Housing model and commercial suitability | Egyptian commercial mud dovecote / wooden loft survey | Cage vs communal fly-pen comparative research | Different systems are commercially real but differ in control and output. | Do not select one universal housing model. | Open — Field Validation Required |
| CON-004 | Summer production / seasonality | Breeding-cycle review describing non-seasonal breeding | Egyptian heat-stress evidence showing summer reproductive depression | Non-seasonal biology can coexist with heat-driven production decline. | Treat heat/environment as modifiers, not mandatory seasonal shutdown. | Open — Contextual Resolution |
| CON-005 | Sexual maturity vs breeding readiness | Reviews: ~6–7 month maturity region | Egyptian strain/body-weight evidence | Biological maturity does not define one commercial admission threshold. | Keep maturity and operational readiness conceptually separate. | Open — Field Validation Required |
| CON-006 | Incubation start anchor | Literature commonly reports ~18-day incubation | Two eggs laid ~48 h apart and incubation behavior changes through clutch completion | Sources often omit whether count starts from first egg, second egg, or sustained incubation. | Preserve observed egg/hatch dates; do not assume one anchor. | Open — Phase 3 Definition Needed |
| CON-007 | Weaning vs market age | Traditional 3–4 week parent-reared literature | Early-separation systems | Separation, physiological independence and sale/slaughter age can be different events. | Keep concepts separate. | Open — Contextual Resolution |
| CON-008 | Hatch-to-next-lay interval | Local Egyptian/Zagel strain data | White Mirthys and early-separation data | Timing differs strongly by strain and management, changing overlap intensity. | Treat next-lay timing as contextual and event-observed. | Open — Contextual Resolution |
| CON-009 | Molt as production interruption | Annual molt evidence | Pigeon reproduction/molt evidence showing overlap and temporary molt interruption | Molt does not automatically equal complete reproductive shutdown. | Treat molt as a production modifier unless local evidence supports a stronger rule. | Open — Field Validation Required |

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
- Different lifecycle anchors used to define a cycle or interval.

يجب الاحتفاظ بالسياق قبل محاولة توحيد الأرقام.
