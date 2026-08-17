# Open Questions

> الأسئلة هنا لا تعني افتراض إجابات. بعد Phase 1C تم تصنيف كل سؤال حسب المرحلة التي يجب حسمه قبلها.

## Priority Classification

| Classification | Question IDs |
|---|---|
| Must Answer Before Farm Structure | OQ-001, OQ-002, OQ-014, OQ-016 |
| Must Answer Before Data Model | OQ-003, OQ-007, OQ-008, OQ-017, OQ-018, OQ-020, OQ-021 |
| Must Answer Before MVP | OQ-004, OQ-006, OQ-009, OQ-010, OQ-015, OQ-019 |
| Can Defer | OQ-005 |
| Optional | OQ-011, OQ-012, OQ-013 |

---

## Critical

### OQ-001
- **Question:** ما نموذج/نماذج تشغيل المزارع التجارية التي يجب أن يمثلها النظام في الإصدار المستهدف الأول؟
- **Reason:** Phase 1 أثبت وجود loft/dovecote/communal وأنظمة أزواج في أقفاص فردية واختلافها التشغيلي.
- **Related Phase:** Phase 2
- **Priority:** Must Answer Before Farm Structure
- **Status:** Open — Research Informed / Field Validation Required
- **Answer:** البحث يؤكد تعدد النظم؛ لم يُحسم أيها يمثل السوق المستهدف.
- **Impact:** يغيّر حدود المجال ومسارات العمليات التي يجب تحليلها.

### OQ-002
- **Question:** ما المستوى الفعلي المطلوب لتتبع الحمام داخل المزرعة: فرد، زوج، مجموعة/موقع، أم مزيج؟
- **Reason:** الزوج مهم تشغيليًا، لكن الفرد والعش/الموقع والزغلول قد تحتاج تتبعًا مستقلًا.
- **Related Phase:** Phase 2 / Phase 3
- **Priority:** Must Answer Before Farm Structure
- **Status:** Open — Research Informed / Field Validation Required
- **Answer:** لا يوجد مستوى واحد يكفي لكل النظم.
- **Impact:** مرتفع على تحليل Domain Entities والسجلات والأداء.

### OQ-003
- **Question:** كيف تُعرّف المزرعة عمليًا "دورة الإنتاج" وما نقطة بدايتها ونهايتها لأغراض الإدارة والقياس، خصوصًا مع تداخل الدورات؟
- **Reason:** Phase 1 أثبت أن Production Cycle مصطلح مبهم وأن الدورات قد تتداخل.
- **Related Phase:** Phase 3
- **Priority:** Must Answer Before Data Model
- **Status:** Open — Critical
- **Answer:** يجب استخدام anchors واضحة مثل first-egg-to-next-first-egg أو hatch-to-next-lay بدل مصطلح عام غير محدد.
- **Impact:** يؤثر على الأحداث والمؤشرات والتقارير وقواعد العمل.

### OQ-004
- **Question:** ما القرارات التشغيلية اليومية التي يجب أن يساعد النظام صاحب المزرعة أو المدير على اتخاذها؟
- **Reason:** النظام يجب أن يخدم القرار التشغيلي لا مجرد تخزين البيانات.
- **Related Phase:** Phase 6 / Phase 8
- **Priority:** Must Answer Before MVP
- **Status:** Open
- **Answer:** Pending
- **Impact:** يؤثر على KPIs والتنبيهات والمهام ونطاق MVP.

### OQ-005
- **Question:** ما المتطلبات المحلية أو التنظيمية أو البيطرية التي يجب أن تؤخذ في الاعتبار في السوق المستهدف؟
- **Reason:** قد تضيف متطلبات سجلات أو إجراءات خاصة.
- **Related Phase:** Phase 4 / Phase 6
- **Priority:** Can Defer
- **Status:** Open
- **Answer:** Pending
- **Impact:** قد يضيف قيودًا أو تقارير إلزامية.

### OQ-014
- **Question:** هل نظام العشّين Double Nest مطبق فعليًا وبأي صورة في المزارع التجارية المصرية المستهدفة، أم يختلف حسب loft/cage/dovecote؟
- **Reason:** أهميته مدعومة بقوة، لكن انتشار التطبيق المحلي الحالي غير محسوم.
- **Related Phase:** Phase 2 / Phase 3
- **Priority:** Must Answer Before Farm Structure
- **Status:** Open — Field Validation Required
- **Answer:** Pending
- **Impact:** مرتفع على فهم nest workflow والتداخل بين الدورات.

### OQ-015
- **Question:** ما مواصفة السوق الحالية للزغلول في المزارع المصرية المستهدفة: عمر البيع، الوزن الحي/المذبوح، وهل تختلف حسب العميل أو المنطقة؟
- **Reason:** 3–4 أسابيع نطاق بحثي شائع لكنه ليس مواصفة سوق مصرية موحدة.
- **Related Phase:** Phase 3 / Phase 5 / Phase 8
- **Priority:** Must Answer Before MVP
- **Status:** Open — Field Validation Required
- **Answer:** Pending
- **Impact:** يؤثر على Market Readiness والأداء والمبيعات.

## Important

### OQ-006
- **Question:** ما أحجام المزارع المستهدفة مبدئيًا من حيث نطاق التشغيل؟
- **Reason:** الحجم يؤثر على مستوى الأتمتة والصلاحيات وسهولة الإدخال وحجم البيانات.
- **Related Phase:** Phase 6 / Phase 8
- **Priority:** Must Answer Before MVP
- **Status:** Open
- **Answer:** Pending
- **Impact:** يؤثر على الأولويات وتجربة الاستخدام.

### OQ-007
- **Question:** ما الطرق الفعلية لإدارة الزوج المنتج وإعادة تكوينه عند وفاة أحد الأفراد أو ضعف الأداء أو قرار الاستبعاد؟
- **Reason:** لا توجد قاعدة تجارية موحدة لإعادة pairing أو كسر الزوج.
- **Related Phase:** Phase 2 / Phase 3
- **Priority:** Must Answer Before Data Model
- **Status:** Open — Field Validation Required
- **Answer:** Pending
- **Impact:** يؤثر على التاريخ والنسب والأداء.

### OQ-008
- **Question:** ما مستوى الدقة المطلوب لتتبع النسب Pedigree في المزارع التجارية المستهدفة؟
- **Reason:** قد يكون أساسيًا في بعض المزارع وثانويًا في أخرى.
- **Related Phase:** Phase 2
- **Priority:** Must Answer Before Data Model
- **Status:** Open
- **Answer:** Pending
- **Impact:** يؤثر على Pedigree Management والبيانات التاريخية.

### OQ-009
- **Question:** ما العمليات التي تتم حاليًا ورقيًا أو باستخدام Excel أو تطبيقات منفصلة في المزارع الواقعية؟
- **Reason:** لم نجد أدلة مصرية كافية عن أدوات التسجيل الحالية.
- **Related Phase:** Phase 6 / Phase 8
- **Priority:** Must Answer Before MVP
- **Status:** Open — Field Validation Required
- **Answer:** Pending
- **Impact:** يؤثر على أولويات MVP ومسارات الاستخدام.

### OQ-010
- **Question:** ما نطاق الربط المطلوب بين بيانات الإنتاج والتكاليف والمبيعات لقياس الربحية؟
- **Reason:** مستوى قياس الربحية لم يُحسم بعد.
- **Related Phase:** Phase 5 / Phase 6 / Phase 8
- **Priority:** Must Answer Before MVP
- **Status:** Open
- **Answer:** Pending
- **Impact:** يؤثر على Financial Analysis وKPIs.

### OQ-016
- **Question:** ما طريقة التعريف السائدة في المزارع المستهدفة: حلقات فردية، ألوان، رقم زوج، رقم قفص، رقم عش، أم مزيج؟
- **Reason:** يجب فصل individual identification عن pair/location identification.
- **Related Phase:** Phase 2
- **Priority:** Must Answer Before Farm Structure
- **Status:** Open — Field Validation Required
- **Answer:** Pending
- **Impact:** يؤثر على موثوقية التتبع والنسب والسجلات.

### OQ-017
- **Question:** ما المعايير الفعلية التي يستخدمها المربي لاختيار طيور الإحلال وإدخالها قطيع الإنتاج؟
- **Reason:** Sexual maturity لا تساوي تلقائيًا Operational Breeding Readiness.
- **Related Phase:** Phase 2 / Phase 3
- **Priority:** Must Answer Before Data Model
- **Status:** Open — Field Validation Required
- **Answer:** Pending
- **Impact:** يؤثر على population flow وتاريخ الطائر.

### OQ-018
- **Question:** ما الحد أو النمط الذي يجعل الزوج "ضعيف الإنتاج"، وهل يتم تقييم الذكر والأنثى منفصلين قبل كسر الزوج؟
- **Reason:** لا يوجد threshold عالمي صالح لكل السلالات والنظم.
- **Related Phase:** Phase 2 / Phase 3 / Phase 6
- **Priority:** Must Answer Before Data Model
- **Status:** Open — Field Validation Required
- **Answer:** Pending
- **Impact:** مرتفع على re-pairing/culling/performance history.

### OQ-019
- **Question:** ما حجم انخفاض الإنتاج صيفًا في المزارع المصرية المستهدفة وما الإجراءات المستخدمة للتخفيف منه حسب نوع المسكن؟
- **Reason:** Heat stress مؤثر مثبت، لكن لا توجد نسبة موحدة لكل مصر.
- **Related Phase:** Phase 4 / Phase 6 / Phase 8
- **Priority:** Must Answer Before MVP
- **Status:** Open — Field Validation Required
- **Answer:** Pending
- **Impact:** يؤثر على تفسير الموسمية والـ benchmarks والتنبيهات.

### OQ-020
- **Question:** هل artificial incubation أو early separation/hand feeding مستخدم تجاريًا في السوق المصري المستهدف؟
- **Reason:** هذه التقنيات تخلق lifecycle مختلفة جذريًا.
- **Related Phase:** Phase 3
- **Priority:** Must Answer Before Data Model
- **Status:** Open — Field Validation Required
- **Answer:** Pending
- **Impact:** قد يضيف مسارات Domain مختلفة.

### OQ-021
- **Question:** ماذا يفعل المربي عمليًا عند وفاة أحد الأبوين مع وجود زغاليل معتمدة عليهما؟
- **Reason:** عدة استجابات ممكنة: الوالد الآخر، fostering، hand feeding، transfer.
- **Related Phase:** Phase 2 / Phase 3 / Phase 4
- **Priority:** Must Answer Before Data Model
- **Status:** Open — Field Validation Required
- **Answer:** Pending
- **Impact:** يؤثر على parent–squab relationship ومسارات الطوارئ.

## Optional

### OQ-011
- **Question:** هل توجد حاجة مستقبلية للعمل Offline أو في بيئات اتصال ضعيف؟
- **Reason:** قد يؤثر لاحقًا على المعمارية وتجربة الاستخدام.
- **Related Phase:** Phase 7 / Phase 8
- **Priority:** Optional
- **Status:** Open
- **Answer:** Pending
- **Impact:** منخفض على Domain Analysis.

### OQ-012
- **Question:** هل توجد حاجة مستقبلية لربط أجهزة أو حساسات أو QR/Barcode/RFID؟
- **Reason:** احتمال توسع في جمع البيانات والتتبع.
- **Related Phase:** Phase 7 / Phase 8
- **Priority:** Optional
- **Status:** Open
- **Answer:** Pending
- **Impact:** مستقبلي.

### OQ-013
- **Question:** ما حالات استخدام الذكاء الاصطناعي التي تستحق الدراسة مستقبلًا بعد توفر بيانات موثوقة؟
- **Reason:** منع إدخال AI قبل فهم البيانات والقرارات.
- **Related Phase:** Phase 8
- **Priority:** Optional
- **Status:** Open
- **Answer:** Pending
- **Impact:** مستقبلي.

## Phase 1C Review Conclusion

- No duplicate questions were added.
- Every current question now has a decision horizon.
- Questions required before Phase 2 are clearly separated from those that can wait until later analysis.
