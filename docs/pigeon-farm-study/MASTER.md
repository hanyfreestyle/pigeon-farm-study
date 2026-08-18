# نظام إدارة مزارع الحمام — الملف الرئيسي للدراسة

> المصدر المركزي المعتمد لحالة الدراسة والقرارات وسياسة الأدلة والنطاق والانتقال بين المراحل.

## رؤية المشروع

دراسة وتحليل وتصميم نظام متكامل لإدارة مزارع الحمام التجاري، مع التركيز على **إنتاج الحمام اللاحم والزغاليل تجاريًا (Commercial Meat Pigeon / Squab Production)**، وبمنهج يبدأ بفهم المجال والعمليات قبل أي تصميم تقني.

## أهداف الدراسة

- فهم مجال إنتاج الزغاليل التجاري بصورة موثقة.
- توثيق دورة الإنتاج والعمليات والقرارات التشغيلية.
- الفصل بين الحقائق البيولوجية والممارسات التشغيلية المتغيرة وقرارات المشروع.
- فهم كيانات المجال (Domain Entities) قبل أي كيانات برمجية (Software Entities).
- استخراج قواعد العمل (Business Rules) من التحليل لاحقًا.
- الوصول إلى نموذج بيانات وتصميم نظام وMVP مبنيين على الواقع التشغيلي.

## النطاق

### داخل النطاق

إنتاج الحمام اللاحم والزغاليل تجاريًا، مع دراسة المسارات البديلة عندما تكون ضرورية لمنع بناء نموذج مجال مغلق.

### خارج نطاق Phase 1

- Database Design / ERD.
- Software Entities / Models.
- Migrations.
- Software Enums.
- APIs / UI / Filament.
- Software Architecture.
- MVP Implementation.
- Coding.

## منهجية الدراسة

**البحث → فهم المجال → التحليل التشغيلي → تحليل الأعمال → قواعد العمل → نمذجة البيانات → تصميم النظام → تعريف MVP → المعمارية التقنية → المراجعة النهائية.**

المبدأ الحاكم: **التحليل يولّد التصميم، وليس العكس.**

## سياسة اللغة والتوثيق

**اللغة الأساسية لجميع ملفات الدراسة هي العربية.**

1. تكتب الشروحات والتحليلات والتقارير بالعربية.
2. يستخدم المصطلح الإنجليزي بين قوسين عند الحاجة.
3. يحتفظ بالمصطلحات الفنية الإنجليزية المهمة لضمان الدقة.
4. لا تكتب فقرات كاملة بالإنجليزية إلا لأسماء/عناوين أصلية أو عناصر ثابتة.
5. كل الملفات والمراحل الجديدة تبدأ بالعربية افتراضيًا.
6. البحث من أي لغة يُفهم ويُحلل ثم يُوثق بالعربية.
7. لا تترجم File Paths أو File Names أو IDs أو Codes أو URLs أو أسماء المصادر والمؤلفين والمؤسسات والسلالات المعروفة.
8. يمكن إبقاء Status Vocabulary الموحدة مثل `Pending`, `Completed`, `Approved`.

## مراحل الدراسة

| المرحلة | الاسم | الحالة | الاعتماديات | ملاحظات |
|---|---|---|---|---|
| Phase 0 | تهيئة الدراسة | Completed | لا يوجد | مكتملة. |
| Phase 1 | بحث المجال | **Completed — Awaiting Final User Approval** | Phase 0 | تمت المواءمة النهائية بعد OQ Round 1. |
| Phase 2 | هيكل المزرعة والمجال الأساسي | Pending | اعتماد Phase 1 | لا تبدأ قبل الاعتماد الصريح. |
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
| Phase 1 Final Alignment & Approval Readiness | Completed — Awaiting Final User Approval |

## سجل القرارات (Decision Log)

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
| DEC-014 | 2026-08-18 | OQ Round 1 | دعم تحليل الربحية مستقبلًا على مستوى المزرعة والعنبر/القسم والسلالة والزوج والدورة/الدفعة حسب البيانات. | Approved |
| DEC-015 | 2026-08-18 | OQ Round 1 | MVP يعمل Online أساسًا وتأجيل Offline + Sync. | Approved |
| DEC-016 | 2026-08-18 | OQ Round 1 | QR/Barcode/RFID/Sensors تكاملات مستقبلية وليست Core MVP. | Approved |
| DEC-017 | 2026-08-18 | OQ Round 1 | AI ليس جزءًا أساسيًا من MVP ويؤجل حتى تتوفر بيانات موثوقة. | Approved |
| DEC-018 | 2026-08-18 | OQ Round 1 | `Genetic Parentage ≠ Foster / Rearing Parentage`؛ نقل البيضة/الزغلول لا يغير النسب الوراثي. | Approved |
| DEC-019 | 2026-08-18 | Resolve OQ-021 | فقد أحد الأبوين أثناء وجود بيض/زغاليل هو Emergency Rearing Workflow متعدد النتائج، مع حفظ النسب الوراثي مستقلًا عن مقدم الرعاية. | Approved |

> **قاعدة حوكمة:** `Decision ≠ Assumption ≠ Verified Fact`.

## سياسة أدلة البحث

التصنيفات المستخدمة:

- حقيقة موثقة (Verified Fact).
- دليل قوي (Strong Evidence).
- دليل متوسط (Moderate Evidence).
- ممارسة صناعية (Industry Practice).
- ممارسة خبير/مربي (Expert / Producer Practice).
- افتراض (Assumption).
- قرار مشروع/تصميم (Project / Design Decision).
- سؤال مفتوح / يحتاج تحققًا ميدانيًا (Open Question / Requires Field Validation).

القواعد:

- لا يتحول الافتراض إلى حقيقة دون دليل.
- لا يتحول قرار المشروع إلى حقيقة عامة عن السوق.
- تسجل اختلافات المصادر بدل إخفائها.
- تحفظ القيم المرجعية مع سياق السلالة والإسكان والإدارة والمناخ والسوق وتعريف القياس.

## قواعد العمل للمراحل القادمة

1. قراءة `MASTER.md`.
2. قراءة ملفات المراحل السابقة ذات الصلة.
3. مراجعة `09-review/open-questions.md` و`assumptions.md` و`risks.md` و`consistency-review.md`.
4. عدم تكرار بحث معتمد دون سبب.
5. عدم تغيير قرار Approved دون قرار جديد موثق.
6. تحديث `STUDY-LOG.md` بعد كل مهمة رئيسية.
7. الرجوع إلى `09-review/domain-to-system-boundaries.md` عند الانتقال من المجال إلى النظام.

## قاعدة المجال أولًا

**Domain Entity ≠ Database Table**  
**Domain Event ≠ Software Event**  
**Information Requirement ≠ Database Field**  
**Benchmark ≠ Constant**  
**Domain Status ≠ Software Enum**

المرجع الكامل: `09-review/domain-to-system-boundaries.md`.

## حالة الأسئلة بعد Open Questions Resolution Round 1

### محسومة على مستوى اتجاه المشروع/المجال

`OQ-001`, `OQ-002`, `OQ-003`, `OQ-004`, `OQ-006`, `OQ-007`, `OQ-008`, `OQ-010`, `OQ-011`, `OQ-012`, `OQ-013`, `OQ-014`, `OQ-016`, `OQ-017`, `OQ-018`, `OQ-021`.

### مجابة جزئيًا وتحتاج تحققًا

- `OQ-009` — طرق التسجيل الحالية.
- `OQ-015` — مواصفات سوق الزغاليل.
- `OQ-019` — حجم أثر الصيف محليًا.
- `OQ-020` — انتشار Foster / Artificial Incubation / Early Separation / Hand Feeding.

### مؤجلة

- `OQ-005` — المتطلبات المحلية والتنظيمية والبيطرية.

**لم تعد OQ-001/OQ-002/OQ-014/OQ-016/OQ-021 Blocking Questions لبدء Phase 2 بعد الاعتماد النهائي.**

## قائمة البحث والتحقق المستقبلي (Future Research Queue)

| ID | الموضوع | المرحلة | الحالة / الغرض |
|---|---|---|---|
| FRQ-001 | إدارة البيض بالتفصيل | Phase 3 | Partially Researched — تفصيل المسارات لاحقًا. |
| FRQ-002 | نمو الزغاليل والفطام والتسويق | Phase 3 / 5 | يحتاج Market Validation. |
| FRQ-003 | الأمراض والعلاجات والتحصينات والحجر والنفوق | Phase 4 | High Priority — بحث صحي منظم. |
| FRQ-004 | التغذية: Feed Types / Programs / Consumption / Cost Inputs | Phase 4 | High Priority — مدخل تشغيلي ومالي. |
| FRQ-005 | المخزون والمشتريات والموردون | Phase 5 | Queued. |
| FRQ-006 | تعريف KPIs والقيم المرجعية | Phase 6 | Queued. |
| FRQ-007 | التمثيل البرمجي للطائر/الزوج/العش/البطن/التداخل | Phase 7 | Deferred until system analysis complete. |
| FRQ-008 | Artificial Incubation / Early Separation / Hand Feeding | Phase 3 / 4 | Field Validation Required. |
| FRQ-009 | Foster / Rearing Pair وفصل النسب عن مقدم الرعاية | Phase 2 / 3 | Domain direction approved; local usage needs validation. |
| FRQ-010 | **الرفاهية الحيوانية (Animal Welfare):** كثافة الإسكان، التعامل، الفصل، الرعاية اليدوية، الظروف البيئية | Phase 4 → Phase 6 عند الحاجة | New Queue Item — لا بحث في هذه المهمة. |
| FRQ-011 | **الاقتصاد والمالية في السياق المصري:** بنية التكلفة، العلف، العمالة، الأدوية، الطاقة، الإهلاك، تكلفة الزغلول، أسعار وقنوات البيع، العملاء، الهوامش والتدفقات | Phase 5 | High Priority before/during Phase 5. |
| FRQ-012 | **Field Interviews / Farm Validation** مع أصحاب ومديري المزارع والمربين والتجار والمتخصصين والأطباء البيطريين | Parallel Validation Track | لا تنفذ الآن؛ تستخدم للتحقق المحلي. |

### عناصر Field Validation الأساسية

- طرق التسجيل الحالية في المزارع المصرية.
- مواصفات سوق الزغاليل.
- Double Nest usage.
- Foster System usage.
- Artificial Incubation.
- Early Separation.
- Hand Feeding.
- Summer Performance.
- Identification Practices.

## مراجعة SRC-016

تمت مراجعة التوثيق الحالي فقط دون بحث جديد. المسجل:

- **العنوان:** Age-related dynamics of reproductive performance and egg quality in breeding pigeons
- **URL:** https://www.sciencedirect.com/science/article/pii/S0032579126006498
- **الناشر/المجلة:** Poultry Science
- **سنة النشر:** 2026
- **تاريخ الوصول:** 2026-08-17 (ضمن المصادر الجديدة لـ Phase 1B)

لم يظهر خطأ توثيقي داخلي واضح، لذلك لم يتم تعديل المصدر.

## معايير الخروج العامة للمراحل Phase 2 → Phase 8

> تُفصّل المعايير لكل Sub-phase في تعليمات المرحلة نفسها. الآتي مستوى حوكمة عام فقط.

| المرحلة | معايير الخروج العامة |
|---|---|
| Phase 2 | الملفات المطلوبة مكتملة؛ أسئلة الهيكل/إدارة الحمام راجعت؛ الافتراضات والمخاطر والاتساق محدثة؛ لا Blocking Question غير مسجل؛ مراجعة المستخدم مطلوبة. |
| Phase 3 | تحليل مسارات الإنتاج والأحداث والاستثناءات مكتمل؛ CON-006 وما يرتبط به معرف تحليليًا؛ الأسئلة والمخاطر محدثة؛ مراجعة المستخدم مطلوبة. |
| Phase 4 | بحث الصحة والتغذية والرفاهية المطلوب مكتمل؛ البروتوكولات/الممارسات مصنفة حسب الدليل والسياق؛ المخاطر والأسئلة محدثة؛ مراجعة المستخدم مطلوبة. |
| Phase 5 | العمليات والمخزون والمبيعات والاقتصاد/المالية موثقة؛ السياق المصري المالي مدروس؛ الافتراضات والأسئلة والمخاطر محدثة؛ مراجعة المستخدم مطلوبة. |
| Phase 6 | Business Rules وKPIs والتقارير والتنبيهات والأدوار وأحداث المجال التحليلية مكتملة ومتسقة مع المراحل السابقة؛ مراجعة المستخدم مطلوبة. |
| Phase 7 | نموذج البيانات والعلاقات والمعمارية والتدقيق ناتجة عن التحليل وليست افتراضات مبكرة؛ مراجعة اتساق مكتملة؛ مراجعة المستخدم مطلوبة. |
| Phase 8 | نطاق MVP ومراحل التطوير والميزات المؤجلة محددة؛ كل ميزة مرتبطة بحاجة موثقة؛ مراجعة المستخدم مطلوبة. |

## حالة الافتراضات

- `ASM-001`: Validated.
- `ASM-002`: Validated.
- `ASM-003`: Provisional.
- `ASM-004`: Provisional.

**لم تتم إضافة ASM لقرارات DEC-007 → DEC-019.**

## موضع الدراسة الحالي

- **Phase 1:** `Completed — Awaiting Final User Approval`.
- **Open Questions Resolution Round 1:** Completed على مستوى اتجاهات المجال/المشروع.
- **Field Validation:** ما زال مفتوحًا حيث تم تحديده.
- **Phase 2:** `Pending`.
- **الإجراء التالي الموصى به:** اعتماد المستخدم النهائي لـ Phase 1 ثم إصدار تعليمات مستقلة لبدء Phase 2.

## شرط التوقف

لا تبدأ Phase 2 أو Farm Structure Analysis أو Pigeon Management Analysis أو Research جديد أو Database Design أو Architecture أو MVP أو Coding قبل تعليمات المستخدم.