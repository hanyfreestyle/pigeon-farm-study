# نظام إدارة مزارع الحمام — الملف الرئيسي للدراسة

> المصدر المركزي المعتمد لحالة الدراسة والقرارات وسياسة الأدلة والنطاق والانتقال بين المراحل.

## رؤية المشروع

دراسة وتحليل وتصميم نظام متكامل لإدارة مزارع الحمام التجاري، مع التركيز على **إنتاج الحمام اللاحم والزغاليل تجاريًا (Commercial Meat Pigeon / Squab Production)**، وبمنهج يبدأ بفهم المجال والعمليات قبل أي تصميم تقني.

## أهداف الدراسة

- فهم مجال إنتاج الزغاليل التجاري بصورة موثقة.
- توثيق دورة الإنتاج والعمليات والقرارات التشغيلية.
- الفصل بين الحقائق البيولوجية والممارسات التشغيلية المتغيرة وقرارات المشروع.
- فهم كيانات المجال قبل أي كيانات برمجية.
- استخراج قواعد العمل من التحليل لاحقًا.
- الوصول إلى نموذج بيانات وتصميم نظام وMVP مبنيين على الواقع التشغيلي.

## النطاق

### داخل النطاق

إنتاج الحمام اللاحم والزغاليل تجاريًا، مع دراسة المسارات البديلة عندما تكون ضرورية لمنع بناء نموذج مجال مغلق.

### غير مسموح قبل مراحله

- Database Design / ERD.
- Software Models / Entities.
- Migrations / Software Enums.
- APIs / UI / Filament.
- Software Architecture.
- MVP Implementation.
- Coding.

## منهجية الدراسة

**البحث → فهم المجال → التحليل التشغيلي → تحليل الأعمال → قواعد العمل → نمذجة البيانات → تصميم النظام → تعريف MVP → المعمارية التقنية → المراجعة النهائية.**

المبدأ الحاكم: **التحليل يولّد التصميم، وليس العكس.**

---

## سياسة اللغة والتوثيق

**اللغة الأساسية لجميع ملفات الدراسة هي العربية.**

1. تكتب الشروحات والتحليلات والتقارير بالعربية.
2. يستخدم المصطلح الإنجليزي بين قوسين عند الحاجة.
3. تبقى أسماء الملفات والمسارات والـIDs والـURLs وأسماء المصادر والعناوين الأصلية كما هي.
4. البحث من أي لغة يُفهم ويُحلل ثم يوثق بالعربية.
5. يمكن إبقاء Status Vocabulary الموحدة مثل `Pending`, `In Progress`, `Completed`, `Approved`.

---

# مراحل الدراسة

| المرحلة | الاسم | الحالة | الاعتماديات | ملاحظات |
|---|---|---|---|---|
| Phase 0 | تهيئة الدراسة | Completed | لا يوجد | مكتملة. |
| Phase 1 | بحث المجال | **Approved** | Phase 0 | معتمدة. |
| Phase 2 | هيكل المزرعة وإدارة الحمام | **Approved** | Phase 1 | اعتمدها المستخدم نهائيًا في 2026-08-18. |
| Phase 3 | تحليل الإنتاج | **In Progress** | Phases 1–2 | Phase 3A Approved؛ Phase 3B مكتملة بانتظار المراجعة. |
| Phase 4 | الصحة والتغذية | Pending | Phases 1–3 | الصحة والعلاجات والنفوق والتغذية والرفاهية. |
| Phase 5 | العمليات والمالية | Pending | Phases 1–4 | المخزون والمشتريات والمبيعات والاقتصاد والماليات. |
| Phase 6 | تحليل النظام | Pending | Phases 1–5 | KPIs والتقارير والتنبيهات والأدوار والقواعد. |
| Phase 7 | التصميم التقني | Pending | Phase 6 | نموذج البيانات والعلاقات والمعمارية والتدقيق. |
| Phase 8 | تعريف MVP | Pending | Phases 6–7 | نطاق MVP والتطوير والتوسع المستقبلي. |
| Phase 9 | المراجعة والتجميع النهائي | Pending | Phases 1–8 | `FINAL-STUDY.md`. |

## تقدم Phase 1

| المرحلة الفرعية / المهمة | الحالة |
|---|---|
| Phase 1A | Completed |
| Phase 1B | Completed |
| Phase 1C | Completed |
| Arabic Language Normalization | Completed |
| Open Questions Resolution Round 1 | Completed |
| Phase 1 Final Alignment & Approval Readiness | Completed |
| اعتماد Phase 1 النهائي | **Approved — 2026-08-18** |

## تقدم Phase 2

| المرحلة الفرعية | الاسم | الحالة | الملف الأساسي |
|---|---|---|---|
| Phase 2A | تحليل الهيكل التشغيلي لمزرعة الحمام | **Approved** | `02-farm-structure/farm-structure.md` |
| Phase 2B | إدارة الطائر والسلالات | **Approved** | `02-farm-structure/pigeon-management.md`, `breed-management.md` |
| Phase 2C | إدارة الأزواج والنسب | **Approved** | `02-farm-structure/pair-management.md`, `pedigree-management.md` |
| Phase 2D | تجميع ومراجعة Phase 2 | **Approved** | `02-farm-structure/PHASE-2-BASELINE.md` |

## تقدم Phase 3

| المرحلة الفرعية | الاسم | الحالة | الملف الأساسي |
|---|---|---|---|
| Phase 3A | دورة التربية وإدارة البيض | **Approved** | `03-production/breeding-cycle.md`, `egg-management.md` |
| Phase 3B | الحضانة والفقس | **Completed — Awaiting Review** | `03-production/hatching.md` |
| Phase 3C | إدارة الزغاليل | Pending | `03-production/squab-management.md` |
| Phase 3D | الأداء وتجميع Phase 3 | Pending | `03-production/performance-management.md` + baseline لاحقًا |

---

# سجل القرارات (Decision Log)

| رقم القرار | التاريخ | المرحلة | القرار | الحالة |
|---|---|---|---|---|
| DEC-001 | 2026-08-17 | Phase 0 | النطاق الأساسي هو إنتاج الحمام اللاحم والزغاليل تجاريًا. | Approved |
| DEC-002 | 2026-08-17 | Phase 0 | لا يتم تصميم Software Entities أو Database Tables قبل فهم Domain Entities ومسارات العمل. | Approved |
| DEC-003 | 2026-08-17 | Phase 0 | السياق التقني المستهدف Laravel 12 + PHP 8.2+ + Filament 4 + MySQL دون تنفيذ مبكر. | Approved |
| DEC-004 | 2026-08-17 | Phase 0 → 1 | تعليمات Phase 1A سمحت ببدء Phase 1. | Approved |
| DEC-005 | 2026-08-17 | Phase 1C | Phase 1 Domain Baseline مكتمل بما يكفي للمراجعة. | Approved |
| DEC-006 | 2026-08-17 | Language | العربية لغة التوثيق الأساسية. | Approved |
| DEC-007 | 2026-08-18 | OQ Round 1 | نموذج البداية = الأزواج الفردية داخل الأقفاص/العيون مع المرونة. | Approved |
| DEC-008 | 2026-08-18 | OQ Round 1 | التتبع متعدد المستويات. | Approved |
| DEC-009 | 2026-08-18 | OQ Round 1 | لا تعريف واحد ثابت لـProduction Cycle؛ الأحداث والمراسي هي الأساس. | Approved |
| DEC-010 | 2026-08-18 | OQ Round 1 | تغيير الشريك ينهي العلاقة السابقة ويبدأ علاقة جديدة دون محو التاريخ. | Approved |
| DEC-011 | 2026-08-18 | OQ Round 1 | Pedigree يعتمد على الأب والأم عند معرفتهما دون حد ثابت للأجيال. | Approved |
| DEC-012 | 2026-08-18 | OQ Round 1 | عدد الأعشاش مرن وDouble Nest ليس إلزاميًا. | Approved |
| DEC-013 | 2026-08-18 | OQ Round 1 | فصل هوية الطائر والزوج والموقع عن المعرف الخارجي. | Approved |
| DEC-014 | 2026-08-18 | OQ Round 1 | دعم تحليل الربحية مستقبلًا على مستويات متعددة. | Approved |
| DEC-015 | 2026-08-18 | OQ Round 1 | MVP Online First. | Approved |
| DEC-016 | 2026-08-18 | OQ Round 1 | QR/Barcode/RFID/Sensors تكاملات مستقبلية. | Approved |
| DEC-017 | 2026-08-18 | OQ Round 1 | AI مؤجل حتى تتوفر بيانات موثوقة. | Approved |
| DEC-018 | 2026-08-18 | OQ Round 1 | `Genetic Parentage ≠ Foster / Rearing Parentage`. | Approved |
| DEC-019 | 2026-08-18 | OQ-021 | Parent Loss = Emergency Rearing Workflow متعدد النتائج. | Approved |
| DEC-020 | 2026-08-18 | Phase 1 Approval | اعتماد Phase 1. | Approved |
| DEC-021 | 2026-08-18 | Phase 2A Approval | اعتماد Phase 2A. | Approved |
| DEC-022 | 2026-08-18 | Phase 2B Approval | اعتماد Phase 2B. | Approved |
| DEC-023 | 2026-08-18 | Phase 2C Approval | اعتماد Phase 2C. | Approved |
| DEC-024 | 2026-08-18 | Phase 2D | بداية الزوج لا تختزل في تاريخ عالمي واحد. | Approved |
| DEC-025 | 2026-08-18 | Phase 2D | Same Pair Reunited بعد نهاية فعلية = Operational Episode جديدة. | Approved |
| DEC-026 | 2026-08-18 | Phase 2D | Trial Pair اختياري ويحتاج تحققًا ميدانيًا. | Approved |
| DEC-027 | 2026-08-18 | Phase 2 Final Approval | تعليمات صاحب المشروع اعتمدت Phase 2 نهائيًا وسمحت ببدء Phase 3A فقط. | Approved |
| DEC-028 | 2026-08-18 | Phase 3A | الإنتاج يحلل من خلال Clutch/Egg/events؛ الزوج الواحد قد يحمل أكثر من Clutch متزامنة، و`Egg Identity ≠ Egg Sequence`. | Approved |
| DEC-029 | 2026-08-18 | Phase 3A | `Expected Hatch = Prediction ≠ Actual Hatch`; مرساة الحضانة لا تُفرض عالميًا وتبقى Policy/Definition Choice إلى Phase 3B. | Approved |
| **DEC-030** | **2026-08-18** | **Phase 3A Approval** | **تعليمات صاحب المشروع الحالية تعتمد Phase 3A رسميًا وتسمح ببدء Phase 3B فقط.** | **Approved** |
| **DEC-031** | **2026-08-18** | **Phase 3B** | **`CON-006` تحل كـConfigurable Domain Policy: لا Universal Biological Incubation Anchor، ويولد Expected Hatch من Policy/Anchor معلنة قابلة للمراجعة مع بقاء الأحداث البيولوجية مستقلة.** | **Approved** |
| **DEC-032** | **2026-08-18** | **Phase 3B** | **نتائج الحضانة والفقس تُحفظ على مستوى البيضة أولًا، ومع الفقس الناجح يجب الحفاظ على `Hatched Egg → Specific Squab` مع فصل Genetic Parentage عن Incubation Responsibility.** | **Approved** |

> **قاعدة حوكمة:** `Decision ≠ Assumption ≠ Verified Fact`.

---

# سياسة أدلة البحث

التصنيفات المستخدمة: Verified Fact، Strong/Moderate Evidence، Industry/Producer Practice، Assumption، Project Decision، Open Question / Field Validation.

القواعد:

- لا يتحول الافتراض إلى حقيقة دون دليل.
- لا يتحول قرار المشروع إلى حقيقة عامة عن السوق.
- تسجل اختلافات المصادر بدل إخفائها.
- تحفظ القيم المرجعية مع سياقها.

---

# قواعد المجال إلى النظام

**Domain Entity ≠ Database Table**  
**Domain Event ≠ Software Event**  
**Information Requirement ≠ Database Field**  
**Benchmark ≠ Constant**  
**Domain Status ≠ Software Enum**

المرجع: `09-review/domain-to-system-boundaries.md`.

---

# حالة الأسئلة المفتوحة

### محسومة على مستوى اتجاه المشروع/المجال

`OQ-001`, `OQ-002`, `OQ-003`, `OQ-004`, `OQ-006`, `OQ-007`, `OQ-008`, `OQ-010`, `OQ-011`, `OQ-012`, `OQ-013`, `OQ-014`, `OQ-016`, `OQ-017`, `OQ-018`, `OQ-021`.

### مجابة جزئيًا وتحتاج تحققًا

- `OQ-009` — طرق التسجيل الحالية.
- `OQ-015` — مواصفات سوق الزغاليل.
- `OQ-019` — أثر الصيف محليًا.
- `OQ-020` — انتشار Foster / Artificial Incubation / Early Separation / Hand Feeding.

### مؤجلة

- `OQ-005` — المتطلبات المحلية والتنظيمية والبيطرية.

### Phase 3B

لم تضف Phase 3B OQ جديدة. `CON-006` أصبحت **Resolved as Configurable Domain Policy** ولا تمنع المراحل التالية. Candling/Artificial/Foster/Assisted Hatch practices تبقى Field Validation غير حابسة.

---

# قائمة البحث والتحقق المستقبلي (Future Research Queue)

| ID | الموضوع | المرحلة | الحالة / الغرض |
|---|---|---|---|
| FRQ-001 | إدارة البيض والحضانة والفقس | Phase 3 | **Phase 3A/3B Completed؛ أداء الإنتاج يجمع في 3D.** |
| FRQ-002 | نمو الزغاليل والفطام والتسويق | Phase 3 / 5 | Phase 3C + Market Validation. |
| FRQ-003 | الأمراض والعلاجات والتحصينات والحجر والنفوق | Phase 4 | High Priority. |
| FRQ-004 | التغذية | Phase 4 | High Priority. |
| FRQ-005 | المخزون والمشتريات والموردون | Phase 5 | Queued. |
| FRQ-006 | KPIs والقيم المرجعية | Phase 6 | Queued. |
| FRQ-007 | التمثيل البرمجي للمفاهيم | Phase 7 | Deferred. |
| FRQ-008 | Artificial Incubation / Early Separation / Hand Feeding | Phase 3 / 4 | Field Validation Required. |
| FRQ-009 | Foster / Rearing Workflow | Phase 2 / 3 | Direction approved; local usage needs validation. |
| FRQ-010 | Animal Welfare | Phase 4 → 6 | High Priority. |
| FRQ-011 | الاقتصاد والمالية في السياق المصري | Phase 5 | High Priority. |
| FRQ-012 | Field Interviews / Farm Validation | Parallel | Local Validation. |
| FRQ-013 | Farm Structure Field Validation | Parallel | Non-blocking. |
| FRQ-014 | Bird & Breed Field Validation | Parallel | Non-blocking. |
| FRQ-015 | Pair & Pedigree Field Validation | Parallel | Non-blocking. |
| FRQ-016 | Egg Production Field Validation: Egg 1/2 recording، Clutch completion، egg marking، Double Nest، Candling timing، prediction anchor، Foster Egg Transfer، Artificial Incubation، Pair movement | Phase 3 / Parallel | Added in Phase 3A — Non-blocking. |
| **FRQ-017** | **Incubation & Hatch Field Validation:** Expected Hatch policy/revision، repeated Candling، Fertility/Embryonic Loss classification، post-failure examination، Pip/Hatch observation precision، Late Hatch، Hatchability definitions، Foster/Artificial/Assisted Hatch، Parent Loss | **Phase 3 / Parallel Track** | **Added in Phase 3B — Non-blocking.** |

---

# ملخص Phase 2 المعتمد

المرجع النهائي لمفاهيم Farm/Location/Bird/Breed/Pair/Pedigree/Foster/Data Confidence هو:

`02-farm-structure/PHASE-2-BASELINE.md`

ولا تعيد Phase 3 تعريف هذه المفاهيم.

---

# ملخص نتائج Phase 3A

- لا يوجد `Production Cycle` غامضة؛ كل Metric يحتاج Start/End Event.
- `Operational Pair → Multiple Clutches` مع إمكانية التداخل.
- `Clutch ≠ Nest` و`Clutch Identity ≠ Fixed Egg Count`.
- `Egg Identity ≠ Egg Sequence`.
- Missing Egg 2 لا تبرر اختلاق بيضة ثانية.
- Extra Egg لا يُفسر سببها دون دليل.
- `Genetic Parentage ≠ Incubating Caregiver` عند نقل البيضة.
- Egg Transfer يحفظ الهوية والنسب والتاريخ.
- Planned وEmergency Foster Transfer مساران مختلفان.
- Artificial Incubation مسار ممكن لكنه يحتاج Field Validation مصريًا.
- `Current Egg Condition ≠ Final Egg Outcome`.
- `Clutch Outcome ≠ Failure Cause`.
- `Expected Hatch = Prediction ≠ Actual Hatch`.

---

# ملخص نتائج Phase 3B

- `Incubation ≠ Single Start Date`؛ تم فصل behavior / sustained incubation / responsibility / period / observation.
- `CON-006 = Resolved as Configurable Domain Policy` دون Universal Anchor.
- Expected Hatch يعتمد على Policy/Anchor واضحة ويمكن إجراء Prediction Revision.
- `Egg Exists ≠ Fertility Known ≠ Embryonic Viability ≠ Hatch Success`.
- `Candling Performed ≠ Observation ≠ Interpretation ≠ Confirmed Diagnosis`.
- Multiple Candling observations صحيحة وتحفظ كتاريخ ملاحظات على مستوى المجال.
- `Infertility ≠ Embryonic Death ≠ Dead-in-shell`.
- Early/Late Embryonic Loss مفاهيم مفيدة، لكن حدود الأيام Context-dependent.
- Actual Hatch يمثل حدثًا فعليًا مستقلًا عن Expected Hatch.
- `Expected Date Passed ≠ Failure Confirmed`.
- `Hatch Failure ≠ Failure Cause`، وUnknown Cause حالة صحيحة.
- `Egg Outcome ≠ Clutch Outcome`.
- Fertility/Hatchability تحتاج Numerator/Denominator صريحين.
- Caregiver يمكن أن يتغير خلال حضانة البيضة، مع ثبات Genetic Parentage.
- Artificial/Foster Incubation مسارات ممكنة؛ Assisted Hatch استثنائي ويحتاج Expert/Veterinary Validation.
- `Hatched Egg → Specific Squab` قاعدة continuity إلى Phase 3C.

---

# الافتراضات

- `ASM-001`: Validated.
- `ASM-002`: Validated.
- `ASM-003`: Provisional.
- `ASM-004`: Provisional.
- افتراضات جديدة في Phase 3A: 0.
- **افتراضات جديدة في Phase 3B: 0.**

---

# المخاطر

- `RSK-007`: Active — Materially Reduced.
- `RSK-009`: Active — Materially Reduced after Phase 3B.
- `RSK-017`: Egg Identity Confusion — Active — Materially Reduced.
- `RSK-018`: Clutch Overlap Misattribution — Active — Reduced.
- `RSK-019`: Foster Transfer Parentage Error — Active — Materially Reduced.
- `RSK-020`: Prediction-as-Fact Risk — Active — Materially Reduced.
- `RSK-021`: Fertility/Hatchability Definition Risk — Active.
- `RSK-022`: Egg-to-Squab Link Loss — Active — Reduced by Principle.
- `RSK-023`: Hatch Failure Misclassification — Active.
- `RSK-024`: Caregiver Attribution Error — Active — Reduced by Principle.

---

# قضايا الاتساق المحمولة

- `CON-003`: Project Direction Resolved / Market Practice Requires Field Validation.
- `CON-006`: **Resolved as Configurable Domain Policy.**
- `CON-009`: Context-dependent / Requires Field Validation.
- Blocking Contradictions after Phase 3B: **0**.

---

# Carry Forward

## Phase 3C

- Hatched Egg → Squab Identity continuity.
- Rearing Caregiver after hatch.
- Fostered Squab.
- Parent Loss after hatch.
- Early post-hatch dependency.
- Crop Milk.
- Growth / Weaning / Early Separation.

## Phase 3D

- Fertility/Hatchability metric definitions.
- Egg vs Clutch performance.
- Genetic Pair vs Incubating Caregiver attribution.
- Embryonic mortality/failure reporting.
- Hatch timing/window metrics where useful.
- Failed production classification.
- Phase 3 baseline/consistency.

## Phase 4

Health / Quarantine / Treatment / Mortality / Welfare / Veterinary confirmation.

## Phase 5

Purchase / Sale / Ownership / Financial attribution.

## Phase 6

Pair KPIs / cross-pair performance / Breed performance / alerts / confidence reporting / Configurable incubation prediction rules.

## Phase 7

تحويل المبادئ إلى Data Model/History/Audit دون كسر Egg/Clutch/Caregiver continuity.

## Phase 8

Advanced Pedigree/Inbreeding/Pair recommendation/Genetic analytics.

---

# معايير الخروج العامة Phase 2 → Phase 8

| المرحلة | معايير الخروج العامة |
|---|---|
| Phase 2 | Approved. |
| Phase 3 | تحليل الإنتاج والأحداث والاستثناءات مكتمل؛ CON-006 معرف ومحلول تحليليًا؛ مراجعة المستخدم مطلوبة. |
| Phase 4 | بحث الصحة والتغذية والرفاهية مكتمل؛ مراجعة المستخدم مطلوبة. |
| Phase 5 | العمليات والمالية محللة والسياق المصري المالي موثق؛ مراجعة المستخدم مطلوبة. |
| Phase 6 | KPIs والتقارير والتنبيهات والأدوار وقواعد العمل محللة؛ مراجعة المستخدم مطلوبة. |
| Phase 7 | نموذج البيانات والعلاقات والمعمارية والتدقيق مبنية على التحليل؛ مراجعة المستخدم مطلوبة. |
| Phase 8 | MVP محدد بوضوح؛ مراجعة المستخدم مطلوبة. |

---

# الحالة الحالية

- **Phase 1: Approved.**
- **Phase 2: Approved.**
- **Phase 3: In Progress.**
- **Phase 3A: Approved.**
- **Phase 3B: Completed — Awaiting Review.**
- **Phase 3C: Pending.**

## القرار الموصى به

**Phase 3B is ready for user approval.**

## الخطوة التالية — بعد مراجعة المستخدم فقط

**Phase 3C — Squab Management Domain Analysis**

## شرط التوقف

لا تبدأ Phase 3C أو Squab Growth أو Weaning أو Performance Management أو Phase 4 أو Database Design أو ERD أو Architecture أو MVP أو Coding قبل اعتماد المستخدم.
