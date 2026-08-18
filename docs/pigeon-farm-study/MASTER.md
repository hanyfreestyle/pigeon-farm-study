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
| Phase 3 | تحليل الإنتاج | **In Progress** | Phases 1–2 | Phase 3A و3B Approved؛ Phase 3C مكتملة بانتظار المراجعة. |
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
| Phase 3B | الحضانة والفقس | **Approved** | `03-production/hatching.md` |
| Phase 3C | إدارة الزغاليل | **Completed — Awaiting Review** | `03-production/squab-management.md` |
| Phase 3D | الأداء وتجميع Phase 3 | Pending | `03-production/performance-management.md` + baseline لاحقًا |

---

# سجل القرارات (Decision Log)

| رقم القرار | التاريخ | المرحلة | القرار | الحالة |
|---|---|---|---|---|
| DEC-001 | 2026-08-17 | Phase 0 | النطاق الأساسي هو إنتاج الحمام اللاحم والزغاليل تجاريًا. | Approved |
| DEC-002 | 2026-08-17 | Phase 0 | لا يتم تصميم Software Entities أو Database Tables قبل فهم المجال. | Approved |
| DEC-003 | 2026-08-17 | Phase 0 | السياق التقني المستهدف Laravel 12 + PHP 8.2+ + Filament 4 + MySQL دون تنفيذ مبكر. | Approved |
| DEC-004 | 2026-08-17 | Phase 0 → 1 | تعليمات Phase 1A سمحت ببدء Phase 1. | Approved |
| DEC-005 | 2026-08-17 | Phase 1C | Phase 1 Domain Baseline جاهز للمراجعة. | Approved |
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
| DEC-027 | 2026-08-18 | Phase 2 Final Approval | اعتماد Phase 2 وبدء Phase 3A فقط. | Approved |
| DEC-028 | 2026-08-18 | Phase 3A | الإنتاج يحلل من خلال Clutch/Egg/events؛ `Egg Identity ≠ Egg Sequence`. | Approved |
| DEC-029 | 2026-08-18 | Phase 3A | `Expected Hatch = Prediction ≠ Actual Hatch`. | Approved |
| DEC-030 | 2026-08-18 | Phase 3A Approval | اعتماد Phase 3A وبدء Phase 3B فقط. | Approved |
| DEC-031 | 2026-08-18 | Phase 3B | `CON-006` = Configurable Domain Policy؛ لا Universal Incubation Anchor. | Approved |
| DEC-032 | 2026-08-18 | Phase 3B | `Hatched Egg → Specific Squab` مع فصل Genetic Parentage عن Incubation Responsibility. | Approved |
| **DEC-033** | **2026-08-18** | **Phase 3B Approval** | **تعليمات صاحب المشروع الحالية تعتمد Phase 3B رسميًا وتسمح ببدء Phase 3C فقط.** | **Approved** |
| **DEC-034** | **2026-08-18** | **Phase 3C** | **Squab هو نفس Bird Identity في Life Stage مبكرة؛ `Hatched Egg → Specific Squab → Same Bird Identity` ولا تنشأ هوية جديدة عند الانتقال إلى Young Bird.** | **Approved** |
| **DEC-035** | **2026-08-18** | **Phase 3C** | **`Management Separation ≠ Physiological Weaning ≠ Weaning Readiness ≠ Market Readiness ≠ Sale Decision`؛ ولا يعتمد عمر/وزن عالمي للفطام أو السوق.** | **Approved** |

> **قاعدة حوكمة:** `Decision ≠ Assumption ≠ Verified Fact`.

---

# سياسة أدلة البحث

التصنيفات المستخدمة: Verified Fact، Strong/Moderate Evidence، Industry/Producer Practice، Assumption، Project Decision، Open Question / Field Validation.

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

### Phase 3C

لم تضف Phase 3C OQ جديدة. `CON-007` أصبحت **Conceptually Resolved / Market Validation Required**. Early Separation/Weaning/Foster/Hand Feeding/Market specifications تبقى Field Validation غير حابسة.

---

# قائمة البحث والتحقق المستقبلي (Future Research Queue)

| ID | الموضوع | المرحلة | الحالة / الغرض |
|---|---|---|---|
| FRQ-001 | إدارة البيض والحضانة والفقس | Phase 3 | Phase 3A/3B Completed؛ الأداء يجمع في 3D. |
| FRQ-002 | نمو الزغاليل والفطام والتسويق | Phase 3 / 5 | **Phase 3C Completed؛ Market Validation يحمل إلى Phase 5.** |
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
| FRQ-016 | Egg Production Field Validation | Phase 3 / Parallel | Non-blocking. |
| FRQ-017 | Incubation & Hatch Field Validation | Phase 3 / Parallel | Non-blocking. |
| **FRQ-018** | **Squab Management Field Validation:** Squab/Young Bird terminology، identification timing، weighing practice، Growth baselines، Parent/Foster/Hand rearing، Early Separation، Weaning meaning/readiness، Market Age/Weight، movement، mortality stage، replacement timing، attribution | **Phase 3 / Parallel Track** | **Added in Phase 3C — Non-blocking.** |

---

# ملخص Phase 2 المعتمد

المرجع النهائي لمفاهيم Farm/Location/Bird/Breed/Pair/Pedigree/Foster/Data Confidence هو:

`02-farm-structure/PHASE-2-BASELINE.md`

ولا تعيد Phase 3 تعريف هذه المفاهيم.

---

# ملخص نتائج Phase 3A

- كل Metric يحتاج Start/End Event صريحين.
- `Operational Pair → Multiple Clutches` مع التداخل.
- `Clutch ≠ Nest` و`Egg Identity ≠ Egg Sequence`.
- Egg Transfer يحفظ الهوية والنسب.
- `Expected Hatch = Prediction ≠ Actual Hatch`.

# ملخص نتائج Phase 3B

- `Incubation ≠ Single Start Date`.
- `CON-006 = Resolved as Configurable Domain Policy`.
- `Egg Exists ≠ Fertility Known ≠ Embryonic Viability ≠ Hatch Success`.
- `Infertility ≠ Embryonic Death ≠ Dead-in-shell`.
- `Hatch Failure ≠ Failure Cause`.
- `Egg Outcome ≠ Clutch Outcome`.
- `Hatched Egg → Specific Squab`.

# ملخص نتائج Phase 3C

- Squab هو نفس Bird Identity في Life Stage مبكرة.
- `Hatched Egg → Specific Squab → Same Bird Identity`.
- `Genetic Parentage ≠ Rearing Caregiver` مع Rearing Caregiver History.
- Crop Milk والرعاية الأبوية مركزية في الاعتماد المبكر، ويشارك كلا الأبوين في المسار الطبيعي.
- `Same Clutch ≠ Exactly Same Age` عند Hatch Asynchrony.
- `Single Weight ≠ Growth Trend`.
- Growth/Weight benchmarks تحتاج Breed/Rearing/Age Anchor/Context.
- `Planned Squab Transfer ≠ Emergency Squab Transfer`.
- One-parent/Foster/Hand Feeding مسارات ممكنة وليست نجاحًا مضمونًا أو Standard عامًا.
- الدليل المصري W0/W7/W28 أظهر trade-off عند Early Separation؛ لا Best Practice عامة.
- `Separation ≠ Physiological Weaning ≠ Market Readiness ≠ Sale Decision`.
- `Mortality Outcome ≠ Mortality Cause` و`Missing ≠ Dead`.
- `Squab → Young Bird → Replacement Candidate` مسار ممكن مع ثبات Bird Identity.
- `Genetic Production ≠ Hatch Result ≠ Rearing Result ≠ Market Output Attribution`.
- Squab Cohort تجميع تحليلي اختياري وليس Batch hierarchy إلزاميًا.

---

# الافتراضات

- `ASM-001`: Validated.
- `ASM-002`: Validated.
- `ASM-003`: Provisional.
- `ASM-004`: Provisional.
- **افتراضات جديدة في Phase 3C: 0.**

---

# المخاطر

- `RSK-007`: Active — Materially Reduced.
- `RSK-009`: Active — Materially Reduced.
- `RSK-022`: Egg-to-Squab Link Loss — Active — Materially Reduced.
- `RSK-025`: Squab/Bird Identity Loss — Active — Reduced by Principle.
- `RSK-026`: Weaning/Separation/Market Confusion — Active — Materially Reduced.
- `RSK-027`: Growth/Market Benchmark as Constant — Active.
- `RSK-028`: Rearing Attribution Error — Active — Reduced by Principle.
- `RSK-029`: Growth Trend Misinterpretation — Active.

---

# قضايا الاتساق المحمولة

- `CON-003`: Project Direction Resolved / Market Practice Requires Field Validation.
- `CON-006`: Resolved as Configurable Domain Policy.
- `CON-007`: **Conceptually Resolved / Market Validation Required.**
- `CON-009`: Context-dependent / Requires Field Validation.
- Blocking Contradictions after Phase 3C: **0**.

---

# Carry Forward

## Phase 3D

- Fertility/Hatchability definitions.
- Egg→Hatch→Squab→Market output funnel.
- Squab survival/growth/weight metrics.
- Pair vs Individual vs Incubating/Rearing Caregiver attribution.
- Early separation / Foster performance comparison.
- Mortality outcome reporting.
- Failed production classification.
- Phase 3 consolidated baseline.

## Phase 4

Health / Treatment / Mortality causes / Crop Milk & nutrition / Hand Feeding safety / Welfare / environmental care.

## Phase 5

Market Age/Weight validation / Buyer specs / live vs dressed / sale / price / retained-vs-sold economics.

## Phase 6

KPIs / thresholds / alerts / confidence reporting / metric definitions.

## Phase 7

Data Model/History/Audit مع حماية Egg→Squab→Bird وCaregiver continuity.

---

# معايير الخروج العامة Phase 2 → Phase 8

| المرحلة | معايير الخروج العامة |
|---|---|
| Phase 2 | Approved. |
| Phase 3 | تحليل الإنتاج والأحداث والاستثناءات مكتمل؛ مراجعة المستخدم مطلوبة. |
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
- **Phase 3B: Approved.**
- **Phase 3C: Completed — Awaiting Review.**
- **Phase 3D: Pending.**

## القرار الموصى به

**Phase 3C is ready for user approval.**

## الخطوة التالية — بعد مراجعة المستخدم فقط

**Phase 3D — Production Performance Domain Analysis**

## شرط التوقف

لا تبدأ Phase 3D أو Performance Management أو Phase 3 Consolidation أو Phase 4 أو Database Design أو ERD أو Architecture أو MVP أو Coding قبل اعتماد المستخدم.
