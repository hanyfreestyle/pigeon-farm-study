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
| Phase 2 | هيكل المزرعة وإدارة الحمام | **In Progress** | Phase 1 | Phase 2A و2B Approved، وPhase 2C مكتملة بانتظار المراجعة. |
| Phase 3 | تحليل الإنتاج | Pending | Phases 1–2 | البيض والفقس والزغاليل والأداء والدورات. |
| Phase 4 | الصحة والتغذية | Pending | Phases 1–3 | الصحة والعلاجات والنفوق والتغذية والرفاهية. |
| Phase 5 | العمليات والمالية | Pending | Phases 1–4 | المخزون والمشتريات والمبيعات والاقتصاد والماليات. |
| Phase 6 | تحليل النظام | Pending | Phases 1–5 | KPIs والتقارير والتنبيهات والأدوار والقواعد. |
| Phase 7 | التصميم التقني | Pending | Phase 6 | نموذج البيانات والعلاقات والمعمارية والتدقيق. |
| Phase 8 | تعريف MVP | Pending | Phases 6–7 | نطاق MVP والتطوير والتوسع المستقبلي. |
| Phase 9 | المراجعة والتجميع النهائي | Pending | Phases 1–8 | `FINAL-STUDY.md`. |

## تقدم Phase 1

| المرحلة الفرعية / المهمة | الحالة |
|---|---|
| Phase 1A — بحث مجال تربية الحمام التجاري | Completed |
| Phase 1B — دورة إنتاج الحمام بالتفصيل | Completed |
| Phase 1C — تجميع المجال ومراجعة التحقق | Completed |
| Arabic Language Normalization | Completed |
| Open Questions Resolution Round 1 | Completed |
| Phase 1 Final Alignment & Approval Readiness | Completed |
| اعتماد Phase 1 النهائي | **Approved — 2026-08-18** |

## تقدم Phase 2

| المرحلة الفرعية | الاسم | الحالة | الملف الأساسي |
|---|---|---|---|
| Phase 2A | تحليل الهيكل التشغيلي لمزرعة الحمام | **Approved** | `02-farm-structure/farm-structure.md` |
| Phase 2B | إدارة الطائر والسلالات | **Approved** | `02-farm-structure/pigeon-management.md`, `breed-management.md` |
| Phase 2C | إدارة الأزواج والنسب | **Completed — Awaiting Review** | `02-farm-structure/pair-management.md`, `pedigree-management.md` |
| Phase 2D | تجميع ومراجعة Phase 2 | Pending | يحدد عند بدء المرحلة. |

---

# سجل القرارات (Decision Log)

| رقم القرار | التاريخ | المرحلة | القرار | الحالة |
|---|---|---|---|---|
| DEC-001 | 2026-08-17 | Phase 0 | النطاق الأساسي هو إنتاج الحمام اللاحم والزغاليل تجاريًا. | Approved |
| DEC-002 | 2026-08-17 | Phase 0 | لا يتم تصميم Software Entities أو Database Tables قبل فهم Domain Entities ومسارات العمل. | Approved |
| DEC-003 | 2026-08-17 | Phase 0 | السياق التقني المستهدف Laravel 12 + PHP 8.2+ + Filament 4 + MySQL دون تنفيذ مبكر. | Approved |
| DEC-004 | 2026-08-17 | Phase 0 → 1 | تعليمات Phase 1A سمحت بإكمال Phase 0 وبدء Phase 1. | Approved |
| DEC-005 | 2026-08-17 | Phase 1C | خط أساس Phase 1 مكتمل بما يكفي للمراجعة مع إبقاء عدم اليقين المحلي كتحقق ميداني. | Approved |
| DEC-006 | 2026-08-17 | Language Normalization | العربية لغة التوثيق الأساسية للدراسة. | Approved |
| DEC-007 | 2026-08-18 | OQ Round 1 | يبدأ التركيز التشغيلي على الأزواج الفردية داخل الأقفاص/العيون مع قابلية دعم Loft/Dovecote/Colony مستقبلًا. | Approved |
| DEC-008 | 2026-08-18 | OQ Round 1 | التتبع متعدد المستويات: طائر، زوج، زغلول عند الحاجة، بيضة، عش، قفص/عين، موقع. | Approved |
| DEC-009 | 2026-08-18 | OQ Round 1 | لا تعريف واحد ثابت لدورة الإنتاج؛ تحفظ الأحداث والتواريخ وتُحسب الفترات حسب مرساة القياس. | Approved |
| DEC-010 | 2026-08-18 | OQ Round 1 | انتهاء علاقة الزوج لا يمحو التاريخ؛ عند تغيير الشريك تنتهي العلاقة السابقة وتبدأ علاقة جديدة. | Approved |
| DEC-011 | 2026-08-18 | OQ Round 1 | Pedigree يعتمد على الأب والأم عند معرفتهما دون حد ثابت للأجيال. | Approved |
| DEC-012 | 2026-08-18 | OQ Round 1 | عدد الأعشاش مرن وDouble Nest ليس إلزاميًا. | Approved |
| DEC-013 | 2026-08-18 | OQ Round 1 | فصل هوية الطائر والزوج والموقع عن وسيلة التعريف الخارجية. | Approved |
| DEC-014 | 2026-08-18 | OQ Round 1 | دعم تحليل الربحية مستقبلًا على مستويات متعددة حسب توفر البيانات. | Approved |
| DEC-015 | 2026-08-18 | OQ Round 1 | MVP يعمل Online أساسًا وتأجيل Offline + Sync. | Approved |
| DEC-016 | 2026-08-18 | OQ Round 1 | QR/Barcode/RFID/Sensors تكاملات مستقبلية وليست Core MVP. | Approved |
| DEC-017 | 2026-08-18 | OQ Round 1 | AI ليس جزءًا أساسيًا من MVP ويؤجل حتى تتوفر بيانات موثوقة. | Approved |
| DEC-018 | 2026-08-18 | OQ Round 1 | `Genetic Parentage ≠ Foster / Rearing Parentage`. | Approved |
| DEC-019 | 2026-08-18 | Resolve OQ-021 | فقد أحد الأبوين أثناء وجود بيض/زغاليل هو Emergency Rearing Workflow متعدد النتائج. | Approved |
| DEC-020 | 2026-08-18 | Phase 1 Final Approval | تعليمات صاحب المشروع اعتمدت Phase 1 رسميًا وسمحت ببدء Phase 2A. | Approved |
| DEC-021 | 2026-08-18 | Phase 2A Approval | تعليمات صاحب المشروع اعتمدت Phase 2A رسميًا وسمحت ببدء Phase 2B فقط. | Approved |
| **DEC-022** | **2026-08-18** | **Phase 2B Approval** | **تعليمات صاحب المشروع الحالية تعتمد Phase 2B رسميًا وتسمح ببدء Phase 2C فقط.** | **Approved** |

> **قاعدة حوكمة:** `Decision ≠ Assumption ≠ Verified Fact`.

---

# سياسة أدلة البحث

التصنيفات المستخدمة:

- حقيقة موثقة (Verified Fact).
- دليل قوي (Strong Evidence).
- دليل متوسط (Moderate Evidence).
- ممارسة صناعية (Industry Practice).
- ممارسة خبير/مربي (Expert / Producer Practice).
- افتراض (Assumption).
- قرار مشروع (Project Decision).
- سؤال مفتوح / يحتاج تحققًا ميدانيًا.

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
- `OQ-019` — حجم أثر الصيف محليًا.
- `OQ-020` — انتشار Foster / Artificial Incubation / Early Separation / Hand Feeding.

### مؤجلة

- `OQ-005` — المتطلبات المحلية والتنظيمية والبيطرية.

### Phase 2A / 2B / 2C

لم تضف Phase 2A أو Phase 2B أو Phase 2C أرقام OQ جديدة. نقاط مثل Pair Start، Trial Pair، Same Pair Reunited، مستوى حفظ Pedigree وInbreeding awareness موثقة كـ **Field Validation / Phase 2D Alignment Items غير حابسة**.

---

# قائمة البحث والتحقق المستقبلي (Future Research Queue)

| ID | الموضوع | المرحلة | الحالة / الغرض |
|---|---|---|---|
| FRQ-001 | إدارة البيض بالتفصيل | Phase 3 | Partially Researched. |
| FRQ-002 | نمو الزغاليل والفطام والتسويق | Phase 3 / 5 | Market Validation. |
| FRQ-003 | الأمراض والعلاجات والتحصينات والحجر والنفوق | Phase 4 | High Priority. |
| FRQ-004 | التغذية: Feed Types / Programs / Consumption / Cost Inputs | Phase 4 | High Priority. |
| FRQ-005 | المخزون والمشتريات والموردون | Phase 5 | Queued. |
| FRQ-006 | تعريف KPIs والقيم المرجعية | Phase 6 | Queued. |
| FRQ-007 | التمثيل البرمجي للمفاهيم والعلاقات | Phase 7 | Deferred. |
| FRQ-008 | Artificial Incubation / Early Separation / Hand Feeding | Phase 3 / 4 | Field Validation Required. |
| FRQ-009 | Foster / Rearing Pair وفصل النسب عن مقدم الرعاية | Phase 2 / 3 | Domain direction approved; local usage needs validation. |
| FRQ-010 | الرفاهية الحيوانية (Animal Welfare) | Phase 4 → 6 | High Priority when relevant. |
| FRQ-011 | الاقتصاد والمالية في السياق المصري | Phase 5 | High Priority before/during Phase 5. |
| FRQ-012 | Field Interviews / Farm Validation | Parallel Track | تحقق محلي موازٍ. |
| FRQ-013 | Farm Structure Field Validation: المصطلحات المحلية، Battery، العين الإنتاجية، ترقيم المواقع، الأقسام، Double Nest، Foster Stock، الحجر | Phase 2 / Parallel Track | Non-blocking validation. |
| FRQ-014 | Bird & Breed Field Validation: الحلقات والترقيم، تحديد الجنس، العمر/النسب عند الشراء، Breed/Strain/Line المحلية، Crossbreeding، معايير الإحلال، Retirement والملكية | Phase 2 / Parallel Track | Non-blocking validation. |
| **FRQ-015** | **Pair & Pedigree Field Validation:** إعلان الزوج رسميًا، Pair Start، طرق/مدة التكوين، Re-pairing، Trial Pair، Purchased Established Pair، Pair Coding، مستوى Pedigree، Foster Pair practices، Inbreeding awareness وBreeding Strategy | **Phase 2 / Parallel Track** | **Added in Phase 2C — Non-blocking validation.** |

---

# ملخص نتائج Phase 2A

التسلسل التشغيلي الموصى به مرن:

`Owner/Organization → Farm → Farm Site? → Pigeon House/Barn → Section? → Cage Group/Row/Rack? → Cage/Production Eye → Nest(s)`

المبادئ الأساسية:

- `Location Identity ≠ Occupant Identity`.
- `Location Identity ≠ Operational Purpose`.
- تغيير موقع الزوج لا يغير تاريخ الزوج.
- عدد الأعشاش مرن.
- Foster Stock قد يكون مخصصًا أو مؤقتًا.
- لفظ Battery يحتاج تحققًا محليًا.
- `Physical Capacity ≠ Recommended Capacity ≠ Current Occupancy`.

---

# ملخص نتائج Phase 2B

- `Bird Identity ≠ External Identifier ≠ Pair Identity ≠ Location Identity`.
- فقد أو استبدال الحلقة لا يغير هوية الطائر.
- `Known Hatch Date ≠ Estimated Age`.
- `Birth Origin ≠ Acquisition Source ≠ Genetic Origin`.
- `Bird Status ≠ Bird Role`.
- Unknown/Partial Data حالات مجال صحيحة.
- Data Confidence / Provenance مهمة للعمر والجنس والسلالة والنسب والمصدر.
- `Culling ≠ Sale ≠ Retirement ≠ Death`، وMissing لا يساوي Death.
- `Breed ≠ Strain ≠ Line` تلقائيًا.
- Crossbred / Mixed Lineage حالة مشروعة.
- `Breed Trait ≠ Individual Bird Trait`.
- `Genetic Parentage ≠ Foster / Rearing Parentage` مستمرة كقاعدة حاكمة.

---

# ملخص نتائج Phase 2C

- `Operational Pair ≠ Pair Formation Attempt ≠ Pair Bond`.
- Pair Formation ليست مجرد جمع الطائرين في مكان واحد.
- لا يوجد تاريخ واحد عالمي لبداية الزوج؛ يجب الفصل بين الجمع والقبول وأول تزاوج والتفعيل الإداري وأول بيضة.
- `Pair Identity ≠ Pair Code ≠ Location Identity`.
- `Pair Existence ≠ Production Success`.
- تغيير الشريك ينهي العلاقة السابقة ويبدأ علاقة جديدة وفق `DEC-010`.
- `Pair Role ≠ Pair Status/Condition`.
- Foster Role قد يكون مخططًا أو طارئًا.
- `Genetic Parents ≠ Incubating Caregiver ≠ Rearing Caregiver`.
- `Pedigree ≠ Pair History`.
- Unknown/Partial Pedigree حالة صحيحة.
- Pedigree يحتاج Confidence / Provenance ويمكن تصحيحه مع الحفاظ على تاريخ التصحيح.
- `No Known Relationship ≠ Proven Unrelated` عند نقص Pedigree.
- Inbreeding Coefficient ميزة تحليلية مستقبلية محتملة، مشروطة بعمق واكتمال النسب.
- `Poor Pair Performance ≠ Poor Male + Poor Female`؛ تقييم الفرد عبر عدة شركاء يحمل إلى Phase 6.

---

# الافتراضات

- `ASM-001`: Validated.
- `ASM-002`: Validated.
- `ASM-003`: Provisional.
- `ASM-004`: Provisional.
- افتراضات جديدة في Phase 2A: 0.
- افتراضات جديدة في Phase 2B: 0.
- **افتراضات جديدة في Phase 2C: 0.**

---

# المخاطر

تم تحديث `09-review/risks.md`، وتضم المخاطر المضافة في Phase 2:

- `RSK-012` — فرض Hierarchy مكانية جامدة.
- `RSK-013` — تحويل بيانات غير مؤكدة إلى حقائق.
- `RSK-014` — الخلط بين Breed/Strain/Line أو فرض Pure Breed.
- `RSK-015` — إعادة كتابة Pair History عند تغيير الشريك/الكود.
- `RSK-016` — الثقة الزائفة في عدم القرابة عند Pedigree ناقص أو تفسير Inbreeding دون اكتمال كافٍ.

---

# قضايا الاتساق المحمولة

- `CON-003`: Project Direction Resolved / Market Practice Requires Field Validation.
- `CON-006`: Still Open — Definition Needed → Carry Forward إلى Phase 3.
- `CON-009`: Context-dependent / Requires Field Validation.
- Phase 2C أضافت قواعد اتساق: `Pedigree ≠ Pair History`، و`Pair Code ≠ Pair Identity`، و`No Known Relationship ≠ Proven Unrelated`.

---

# معايير الخروج العامة Phase 2 → Phase 8

| المرحلة | معايير الخروج العامة |
|---|---|
| Phase 2 | الملفات المطلوبة مكتملة؛ أسئلة الهيكل/إدارة الحمام راجعت؛ الافتراضات والمخاطر والاتساق محدثة؛ لا Blocking Question غير مسجل؛ مراجعة المستخدم مطلوبة. |
| Phase 3 | تحليل الإنتاج والأحداث والاستثناءات مكتمل؛ CON-006 معرف تحليليًا؛ مراجعة المستخدم مطلوبة. |
| Phase 4 | بحث الصحة والتغذية والرفاهية المطلوب مكتمل؛ الممارسات مصنفة حسب الدليل والسياق؛ مراجعة المستخدم مطلوبة. |
| Phase 5 | العمليات والمخزون والمشتريات والمبيعات والاقتصاد والماليات محللة؛ السياق المصري المالي موثق؛ مراجعة المستخدم مطلوبة. |
| Phase 6 | KPIs والتقارير والتنبيهات والأدوار وقواعد العمل وأحداث المجال محللة؛ الاتساق مراجع؛ مراجعة المستخدم مطلوبة. |
| Phase 7 | نموذج البيانات والعلاقات والمعمارية وسجل التدقيق مبنية على التحليل السابق؛ مراجعة المستخدم مطلوبة. |
| Phase 8 | MVP محدد بوضوح مع ما داخل/خارج النطاق ومراحل التطوير؛ مراجعة المستخدم مطلوبة. |

---

# الحالة الحالية

- **Phase 1: Approved.**
- **Phase 2: In Progress.**
- **Phase 2A: Approved.**
- **Phase 2B: Approved.**
- **Phase 2C: Completed — Awaiting Review.**
- **Phase 2D: Pending.**

## الخطوة التالية — بعد مراجعة المستخدم فقط

**Phase 2D — Phase 2 Consolidation & Review**

## شرط التوقف

لا تبدأ Phase 2D أو Production Analysis أو Database Design أو ERD أو Architecture أو MVP أو Coding قبل تعليمات المستخدم.
