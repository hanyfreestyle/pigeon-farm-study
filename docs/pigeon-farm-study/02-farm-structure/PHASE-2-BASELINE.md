# خط الأساس التجميعي للمرحلة الثانية (Phase 2 Domain Baseline)

> **المرحلة:** Phase 2D — مراجعة وتجميع المرحلة الثانية  
> **الحالة:** Completed — Awaiting Review  
> **التاريخ:** 2026-08-18  
> **الغرض:** مرجع تجميعي معتمد لمخرجات Phase 2A وPhase 2B وPhase 2C، دون استبدال الملفات التفصيلية ودون تصميم قاعدة بيانات أو معمارية أو MVP.  
> **مرجع الحدود:** `09-review/domain-to-system-boundaries.md`.

---

## 1. الملخص التنفيذي للمرحلة الثانية

توضح Phase 2 أن مزرعة الحمام يجب فهمها كمجموعة من **مواقع مستقلة الهوية، وطيور مستقلة الهوية، وعلاقات أزواج تاريخية، وتصنيفات سلالية متفاوتة الثقة، وروابط نسب وراثية مستقلة عن الرعاية الفعلية**.

النموذج المتماسك الناتج لا يفترض أن المكان هو الشاغل، ولا أن رقم الحلقة هو الطائر، ولا أن الزوج الحالي يساوي تاريخ الطائر، ولا أن السلالة المسجلة تثبت النقاء، ولا أن الزوج الحاضن هو الأب الوراثي، ولا أن نقص النسب يجعل السجل غير صالح.

المبادئ الحاكمة:

- `Location Identity ≠ Occupant Identity ≠ Operational Purpose`.
- `Bird Identity ≠ External Identifier ≠ Location Identity ≠ Pair Identity`.
- `Bird Status ≠ Bird Role`.
- `Breed ≠ Strain ≠ Breeding Line` تلقائيًا.
- `Operational Pair ≠ Pair Formation Attempt ≠ Pair Bond`.
- `Pair Identity ≠ Pair Code ≠ Location Identity`.
- تغيير أحد الشريكين = علاقة تشغيلية جديدة، مع حفظ العلاقة السابقة.
- `Genetic Parentage ≠ Incubating Caregiver ≠ Rearing Caregiver`.
- `Pedigree ≠ Pair History`.
- `Unknown / Partial Pedigree ≠ Invalid Record`.
- `No Known Relationship ≠ Proven Unrelated`.
- `Unknown ≠ Invalid`, و`Estimated ≠ Verified`, و`Reported ≠ Confirmed`.

Phase 2 أصبحت متماسكة بما يكفي للمراجعة النهائية من المستخدم قبل الانتقال إلى Phase 3.

---

## 2. الهيكل التشغيلي للمزرعة

التسلسل التشغيلي الموصى به مرن:

```text
Owner / Organization
        ↓
Farm
        ↓
Farm Site ?
        ↓
Pigeon House / Barn
        ↓
Section / Zone ?
        ↓
Cage Group / Row / Rack ?
        ↓
Cage / Production Eye
        ↓
Nest(s)
```

علامة `?` تعني أن المستوى اختياري. هذا **Operational Hierarchy** وليس Database Hierarchy.

نموذج البداية التشغيلي للمشروع وفق `DEC-007` هو **الأزواج الفردية داخل الأقفاص / العيون الإنتاجية**، مع إبقاء Loft / Dovecote / Colony / Mixed Systems ممكنة مستقبلًا.

---

## 3. Farm / Site / Pigeon House / Section

- **Farm:** وحدة النشاط التشغيلي والإداري.
- **Farm Site:** موقع فعلي منفصل عند تعدد المواقع؛ قد يندمج عمليًا مع Farm في المزرعة البسيطة.
- **Pigeon House / Barn:** وحدة الإسكان الرئيسية دون افتراض تصميم واحد.
- **Physical Section:** جزء مكاني فعلي.
- **Functional Section:** غرض تشغيل قد يُسند لمكان ويتغير بمرور الوقت.

قاعدة:

`Physical Section ≠ Functional Purpose`.

---

## 4. Cage / Production Eye / Nest

القفص / العين الإنتاجية هو موقع إسكان محدد في نموذج الأزواج الفردية، لكنه لا يساوي الشاغل أو الغرض الحالي.

`Cage Identity ≠ Occupant ≠ Operational Purpose`.

العش مستقل مفاهيميًا عن القفص. يمكن أن يوجد عش واحد أو أكثر، ولا يفترض أن الزوج يملك عشًا دائمًا واحدًا. `Double Nest` خيار تشغيلي مثبت كمفهوم لكنه ليس إلزاميًا لكل زوج.

---

## 5. هوية الموقع (Location Identity)

المكان يحتفظ بهويته رغم تغير:

- الشاغل؛
- النشاط؛
- الاستخدام؛
- رقم أو وصف تشغيلي قابل للتغيير.

تغيير غرض القفص من إنتاج إلى إحلال أو عزل لا يجعله مكانًا جديدًا في ذاته.

---

## 6. هوية الطائر (Bird Identity)

الطائر فرد تاريخي مستقل يستمر تعريفه رغم:

- تغيير القفص أو العنبر؛
- تغيير الزوج؛
- فقد أو استبدال الحلقة؛
- تغير الدور أو الحالة؛
- البيع أو التقاعد أو النفوق مع بقاء التاريخ.

`Bird Identity ≠ Ring Number / External Identifier`.

الحلقة وسيلة تعريف وليست الهوية نفسها.

---

## 7. Bird Status مقابل Bird Role

**الحالة (Status / Condition)** تصف وضع الطائر في وقت ما، مثل مفقود أو مريض أو في حجر أو نشط.

**الدور (Role)** يصف وظيفته داخل القطيع، مثل Breeding Bird أو Replacement Bird أو Foster Bird.

`Bird Status ≠ Bird Role`.

ولا تتحول هذه المفاهيم تلقائيًا إلى Enums برمجية.

---

## 8. أصل الطائر وثقة البيانات

يجب الفصل بين:

- `Birth Origin` — مكان/سياق الفقس؛
- `Acquisition Source` — كيف دخل إلى المزرعة الحالية؛
- `Genetic Origin` — الأصل المرتبط بالنسب.

كما أن قيمة المعلومة ومصدرها ودرجة الثقة فيها مفاهيم مستقلة، خصوصًا في:

- العمر؛
- الجنس؛
- السلالة؛
- النسب؛
- الأصل؛
- تاريخ الزوج المشترى.

`Reported / Estimated / Inferred ≠ Verified`.

---

## 9. Breed / Strain / Line

لا يُفترض أن:

`Breed = Strain = Breeding Line`.

اسم التصنيف لا يثبت النقاء الوراثي، كما أن صفات السلالة المرجعية لا تساوي صفات كل فرد منها.

`Breed Trait ≠ Individual Bird Trait`.

يجب قبول حالات Crossbred / Mixed Lineage / Unknown Classification بدل إجبار كل طائر على سلالة نقية واحدة.

---

## 10. الإحلال (Replacement)

الإحلال قرار إدارة قطيع وليس مرحلة عمرية تلقائية.

`Selected Replacement ≠ Breeding Ready ≠ Active Breeder`.

اختيار الإحلال قد يعتمد على العمر والنمو والصحة والسلالة والخط والنسب وأداء الأبوين واحتياجات القطيع، دون Threshold عالمي واحد.

---

## 11. الزوج التشغيلي (Operational Pair)

الزوج التشغيلي هو علاقة تاريخية بين ذكر وأنثى محددين قررت المزرعة إدارتهما كوحدة تربية خلال فترة معينة.

مجرد وضع الطائرين معًا لا يكفي لإثبات زوج مستقر.

`Operational Pair ≠ Pair Formation Attempt ≠ Pair Bond`.

كما أن وجود زوج لا يعني نجاح إنتاجه:

`Pair Existence ≠ Production Success`.

---

## 12. تكوين الزوج (Pair Formation)

يمكن أن يكون التكوين طبيعيًا أو متحكمًا فيه. مؤشرات القبول قد تشمل انخفاض العدوان، المغازلة المتبادلة، القرب، التزاوج، استخدام العش والتنسيق في الرعاية.

لا توجد مدة عالمية ثابتة لتكوين الزوج، ولا يصبح كل زوج موضوع معًا زوجًا مقبولًا تلقائيًا.

### محاذاة بداية الزوج

لا تعتمد Phase 2 تاريخًا واحدًا عالميًا لبداية الزوج. يجب الاحتفاظ بالمفاهيم/الأحداث الواقعية منفصلة تحليليًا:

- Birds placed together.
- Pair acceptance.
- Management activation.
- First mating observed.
- First egg.

هذه أحداث مختلفة، وأي مرساة تحليلية مستقبلية يجب أن تُسمى بوضوح بدل اختزالها في `Pair Start Date` غامض.

---

## 13. تاريخ الأزواج (Pair History)

لكل طائر تاريخ علاقات يمكن أن يشمل أكثر من شريك.

تغيير الشريك لا يعدل العلاقة السابقة. مثلًا:

```text
Male A + Female B = Pair Episode 1
Pair Episode 1 ends
Male A + Female C = Pair Episode 2
```

يُحفظ تاريخ كل علاقة ونتائجها بصورة مستقلة.

`Poor Pair Performance ≠ Poor Male + Poor Female`، ولذلك يلزم لاحقًا تقييم الفرد عبر شركاء متعددين.

### نفس الزوج بعد الانفصال ثم العودة

إذا **انتهت** العلاقة بين Male A وFemale B فعليًا ثم أُعيدا معًا بعد فترة، فهذه **علاقة/حلقة تشغيلية جديدة بين نفس الفردين**، وليست إعادة فتح للعلاقة التاريخية القديمة.

أما إذا كان الفصل مؤقتًا ولم تُعتبر العلاقة منتهية إداريًا، فيمكن أن يستمر نفس الزوج التشغيلي.

هذا التفريق يحافظ على Pair History ويمنع دمج فترتين إنتاجيتين منفصلتين.

---

## 14. الزوج مقابل الموقع

`Pair Identity ≠ Location Identity`.

نقل الزوج من قفص أو قسم أو عنبر إلى آخر لا ينشئ زوجًا جديدًا، طالما لم تتغير العلاقة نفسها.

يجب حمل أثر النقل أثناء إنتاج نشط إلى Phase 3.

---

## 15. الزوج مقابل العش

`Pair ≠ Nest`.

قد يستخدم الزوج عشًا واحدًا أو عدة أعشاش، وقد يتم استبدال العش أو هجره أو إعادة تخصيصه. لا يُفترض أن للزوج ملكية دائمة لعش واحد.

---

## 16. Foster / Rearing Roles

يجب توحيد المفاهيم التالية:

- **Foster Stock:** طيور/أزواج متاحة للرعاية البديلة، مخصصة أو مؤقتة.
- **Foster Bird:** طائر دوره الحالي دعم الرعاية البديلة؛ ليس Breed.
- **Foster Pair:** زوج يؤدي دور الحضانة أو التربية البديلة؛ ليس Genetic Parent تلقائيًا.
- **Planned Foster Transfer:** نقل مخطط ضمن استراتيجية إنتاج.
- **Emergency Foster Transfer:** نقل بسبب طارئ مثل فقد أحد الأبوين.
- **Incubating Caregiver:** من قام بالحضانة الفعلية، وقد يكون زوجًا بديلًا أو حضانة صناعية.
- **Rearing Caregiver:** من قام بتربية الزغلول فعليًا، وقد يكون الأبوين الوراثيين أو Foster Pair أو والدًا واحدًا أو رعاية يدوية/مختلطة.

قواعد:

**Foster Role ليس Breed.**  
**Foster Role ليس Location.**  
**Foster Pair ليس Genetic Parent لمجرد الرعاية.**

---

## 17. النسب الوراثي (Genetic Parentage)

الأب والأم الوراثيان يصفان الأصل الجيني للطائر، ولا يتغيران بسبب نقل البيضة أو الزغلول.

`Genetic Parents ≠ Incubating Caregiver ≠ Rearing Caregiver`.

قد تتطابق الأطراف في المسار الطبيعي، وقد تختلف في التحضين البديل أو الحضانة الصناعية أو الرعاية اليدوية.

---

## 18. Pedigree

Pedigree هو شبكة العلاقات الوراثية التاريخية عبر الأب والأم عند معرفتهما، وليس سجل الأزواج التي دخلها الطائر.

`Pedigree ≠ Pair History`.

عمق النسب غير محدود بعدد ثابت من الأجيال وفق `DEC-011`، لكن الواقع قد يحتوي على صفر أو جيل واحد أو عدة أجيال فقط.

---

## 19. Partial Pedigree

الحالات الصحيحة تشمل:

- أب معروف وأم مجهولة؛
- أم معروفة وأب مجهول؛
- كلاهما مجهول؛
- Parents reported / claimed؛
- نسب مستورد أو ناقص الأجيال.

`Unknown / Partial Pedigree ≠ Invalid Record`.

النظام المستقبلي لا يجب أن يجبر المستخدم على اختراع أب أو أم لاستكمال شجرة شكلية.

---

## 20. الوعي بزواج الأقارب (Inbreeding Awareness)

يجب أن يستطيع المجال مستقبلًا التمييز بين علاقات قريبة معروفة مثل Parent × Offspring أو Full/half siblings وبين حالة عدم توفر نسب كافٍ.

القاعدة الأساسية:

`No Known Relationship ≠ Proven Unrelated`.

معامل زواج الأقارب (Inbreeding Coefficient) مناسب كميزة تحليلية مستقبلية إذا توفر Pedigree كافٍ وموثوق، لكنه لا يحمل معنى قويًا دون معرفة عمق واكتمال النسب.

لا تنفذ Phase 2 أي Formula أو Algorithm.

---

## 21. مفاهيم الحركة

تشمل الحركة:

- Bird Movement.
- Pair Movement.
- Location Change.
- Temporary Location.
- Quarantine Transfer.
- Treatment Transfer.

المبادئ المشتركة:

- حركة الطائر لا تغير هويته.
- حركة الزوج لا تغير هوية العلاقة.
- الموقع الحالي لا يلغي التاريخ المكاني.
- النقل قد يؤثر في تفسير الأداء أو الإنتاج، ولذلك تحمل الأحداث المرتبطة بدورة نشطة إلى Phase 3.

---

## 22. الاستثناءات المهمة

يجب أن يظل النموذج صالحًا لحالات مثل:

- Purchased / Imported Adult.
- Sold then Returned Bird.
- Retired then Reactivated Bird.
- Missing then Found Bird.
- Bird without Ring / Ring replaced.
- Unknown Age / Sex / Breed / Origin.
- Purchased Established Pair.
- Pair with unknown start date.
- Same pair reunited after a true termination.
- Temporary pair separation.
- Wrong sex discovered.
- One partner missing.
- Foster-only use.
- Pair without production.
- Repeated failed clutches.
- Partial / corrected Pedigree.

### Trial Pair

`Trial Pair` يظل **Optional Domain Concept / Requires Field Validation**. لا توجد حاجة لفرضه كمفهوم إلزامي على كل مزرعة في Phase 2. يمكن وصف الواقع بدقة من خلال `Pair Formation Attempt` ما لم يثبت الاستخدام المحلي المستقل لمصطلح Trial Pair أو حاجة تشغيلية منفصلة.

---

## 23. التحقق الميداني المطلوب

### Farm Structure Validation — أولوية متوسطة

- المصطلحات المحلية لـ Pigeon House / Battery / Production Eye.
- ترقيم المواقع والأقفاص والأعشاش.
- وجود Section / Cage Group فعليًا.
- Double Nest usage.
- Foster Stock location.

### Bird Management Validation — أولوية عالية

- طرق الحلقات والترقيم وتوقيت تركيبها.
- فقد/استبدال الحلقة.
- طرق تحديد الجنس محليًا.
- تسجيل عمر الطائر البالغ المشترى.
- طرق حفظ مصدر الطائر وحركته.
- معايير الإحلال والتقاعد.

### Breed Validation — أولوية عالية

- الاستخدام المحلي لـ Breed / Strain / Line.
- معنى Baladi / Local Egyptian.
- White Mirthys / Myrthes وZagel في الممارسة.
- Crossbreeding وMixed Lineage.
- مصادر الثقة في تصنيف السلالة.

### Pair Management Validation — أولوية عالية

- كيف ومتى يعلن المربي الزوج رسميًا.
- Pair Formation ومدة القبول/الرفض.
- Re-pairing وفترات الانتظار إن وجدت.
- Purchased Established Pairs.
- Pair Coding.
- Same-pair reunion في الممارسة.
- مدى استخدام Trial Pair كمفهوم مستقل.

### Pedigree Validation — أولوية عالية

- مدى حفظ Pedigree فعليًا.
- مستوى الأجيال المعتاد.
- شهادات أو سجلات النسب.
- تصحيح النسب الخاطئ.
- وعي المربين بالقرابة وInbreeding.
- Linebreeding / Outcrossing / Crossbreeding strategies.

### Foster Workflow Validation — أولوية عالية عند المزارع التي تستخدمه

- Planned Foster use.
- Emergency Foster use.
- هل يوجد Foster Stock مخصص أم دور مؤقت.
- من يسجل Incubating / Rearing Caregiver.
- Artificial Incubation / Hand Feeding.

هذه البنود **غير حابسة لPhase 3** ما لم يظهر منها لاحقًا تعارض جديد يؤثر مباشرة في تحليل الإنتاج.

---

## 24. ما يُحمل إلى Phase 3 — Production

يجب أن تبدأ Phase 3 وهي تحمل صراحة:

- Pair → Multiple Clutches.
- Overlapping Production Cycles.
- Egg Identity.
- Egg 1 / Egg 2.
- Nest 1 / Nest 2.
- `CON-006` — Incubation Start Anchor.
- Genetic Parents.
- Incubating Caregiver.
- Rearing Caregiver.
- Foster Transfer.
- Planned vs Emergency Foster Transfer.
- Parent Loss.
- Egg → Hatch → Squab continuity.
- Pair Movement during active production.
- Production attribution: Bird vs Pair vs Clutch.
- Failed production scenarios.
- Pair Performance concepts دون KPI formulas.

---

## 25. استنتاجات Phase 2

1. **المزرعة بنية مرنة وليست Hierarchy إلزامية كاملة.**
2. **المكان والشاغل والغرض مفاهيم مستقلة.**
3. **الطائر فرد تاريخي مستقل عن الحلقة والموقع والزوج الحالي.**
4. **الحالة والدور ليسا التصنيف نفسه.**
5. **المعلومة قد تكون مجهولة أو مقدرة أو مبلغًا عنها دون أن يصبح السجل غير صالح.**
6. **السلالة والخط والتصنيف تحتاج مصدرًا وثقة ولا تثبت أداء الفرد.**
7. **الزوج علاقة تاريخية مستقلة؛ تغيير الشريك لا يعيد كتابة الماضي.**
8. **لا يوجد تاريخ واحد عالمي لبداية الزوج؛ الأحداث المختلفة تحفظ مفاهيميًا بصورة مستقلة.**
9. **عودة نفس الطائرين بعد انتهاء العلاقة تمثل Episode تشغيلية جديدة؛ الفصل المؤقت لا يفعل ذلك.**
10. **Pair Code وسيلة تعريف وليس هوية العلاقة.**
11. **Pedigree علاقة وراثية، وPair History علاقة تشغيلية.**
12. **Genetic Parentage مستقل عن Incubating/Rearing Caregiver.**
13. **النسب الناقص لا يثبت عدم القرابة.**
14. **Trial Pair مفهوم اختياري لا يفرض على كل المزارع.**
15. **لا يوجد تعارض Domain حابس يمنع الانتقال إلى Phase 3 بعد اعتماد المستخدم.**

---

## المبادئ الدومينية المعتمدة

### Location

`Location Identity ≠ Occupant Identity`  
`Location Identity ≠ Operational Purpose`

### Bird

`Bird Identity ≠ Ring Number / External Identifier`  
`Bird Identity ≠ Location Identity`  
`Bird Identity ≠ Pair Identity`  
`Bird Status ≠ Bird Role`

### Breed

`Breed ≠ Strain ≠ Line`  
`Breed Trait ≠ Individual Bird Trait`

### Pair

`Operational Pair ≠ Pair Formation Attempt`  
`Pair Identity ≠ Location Identity`  
`Pair Code ≠ Pair Identity`  
`Partner Change = New Operational Relationship`

### Parentage

`Genetic Parentage ≠ Incubating Caregiver ≠ Rearing Caregiver`

### Pedigree

`Pedigree ≠ Pair History`  
`Unknown Pedigree ≠ Invalid Record`  
`No Known Relationship ≠ Proven Unrelated`

### Data

`Unknown ≠ Invalid`  
`Estimated ≠ Verified`  
`Reported ≠ Confirmed`

---

## Bird Lifecycle Alignment

المرجع الوصفي:

`Egg → Hatch → Squab → Young Bird → Replacement Candidate → Breeding Ready → Active Breeder`

ليس Mandatory Linear Workflow؛ يمكن للطائر الدخول بالغًا بالشراء/الاستيراد أو المرور بمسارات بيع/عودة أو تقاعد/إعادة تفعيل أو فقد/عودة.

---

## Pair Lifecycle Alignment

المرجع الوصفي:

`Candidate Combination → Pair Formation Attempt → Acceptance → Operational Pair → End → Re-pairing`

هذا Reference Domain Lifecycle وليس Mandatory State Machine.

---

## التعامل مع البيانات المجهولة أو الجزئية

يجب قبول:

- Unknown Age.
- Unknown Sex.
- Unknown Breed.
- Unknown Father.
- Unknown Mother.
- Unknown Pair Start.
- Unknown Previous Pair History.
- Unknown Origin.

المبدأ:

**النظام المستقبلي لا يجب أن يجبر المستخدم على اختراع بيانات لمجرد استكمال نموذج.**

---

## مبادئ الحفاظ على التاريخ

- تغيير الموقع لا يمحو Location History.
- تغيير الحلقة لا ينشئ Bird جديدًا.
- تغيير الشريك لا يعيد كتابة Pair History.
- بيع الطائر لا يمحو إنتاجه السابق.
- النفوق لا يمحو السجل التاريخي.
- تصحيح النسب يجب أن يكون قابلًا للتتبع من حيث القيمة القديمة والسبب والمصدر.
- تغيير الغرض من القفص لا يغير Location Identity.
- انتهاء الزوج ثم عودة نفس الفردين ينشئ Episode تشغيلية جديدة بدل إعادة فتح الماضي.

---

## ما يُحمل إلى Phase 4

- Quarantine.
- Sick / Treatment.
- Mortality / Cause of Death.
- Body Condition.
- Health effects on production.
- Animal Welfare.
- Recommended Capacity من منظور الرفاهية والصحة.

## ما يُحمل إلى Phase 5

- Purchase / Acquisition.
- Supplier / Seller.
- Sale / Buyer.
- Price / Value.
- Bird Ownership / Custody عند الحاجة.
- Financial attribution للطائر/الزوج/الناتج.

## ما يُحمل إلى Phase 6

- Pair KPIs.
- Individual vs Pair Performance.
- Cross-pair historical comparison.
- Breed / Line performance.
- Inbreeding / Kinship warnings.
- Data Confidence reporting.
- Low-performance alerts.

## ما يُحمل إلى Phase 8

يُقيّم لاحقًا هل يدخل MVP أم Future Scope:

- Advanced Pedigree Visualization.
- Inbreeding Coefficient.
- Pair Recommendation / Pairing Warnings.
- Genetic Analytics.
- Advanced Breed Analytics.
- Trial Pair كميزة مستقلة.

---

## مصفوفة ثقة المجال للمرحلة الثانية

| الموضوع | النتيجة | مستوى الثقة | يحتاج تحققًا ميدانيًا؟ | تأثيره على Phase 3 |
|---|---|---|---|---|
| Farm / Site | الفصل مفيد عند تعدد المواقع والمستوى اختياري | متوسط-قوي | نعم للانتشار الفعلي | منخفض |
| Pigeon House / Section | مستويات تشغيلية مرنة وليست إلزامية | قوي مفاهيميًا | نعم للمصطلحات والتقسيم المحلي | منخفض |
| Cage / Nest | القفص موقع والعش مستقل وعدد الأعشاش مرن | قوي | نعم للممارسة المحلية | مرتفع |
| Location Identity | مستقل عن الشاغل والغرض | قوي | لا لحسم المبدأ | متوسط |
| Bird Identity | مستقل عن الحلقة والموقع والزوج | قوي | نعم لوسائل التعريف الفعلية | مرتفع |
| Bird Status / Role | مفهومان مختلفان | قوي | نعم للمصطلحات المحلية | متوسط |
| Breed Classification | Breed/Strain/Line لا تتطابق تلقائيًا | متوسط-قوي | نعم — مرتفع | متوسط |
| Operational Pair | علاقة تاريخية مستقلة عن الموقع والكود | قوي | نعم لبداية/إعلان الزوج | مرتفع جدًا |
| Pair Start | لا يوجد تاريخ عالمي واحد؛ توجد أحداث متعددة | قوي كمبدأ | نعم للممارسة التشغيلية | مرتفع |
| Same Pair Reunited | Episode جديدة بعد نهاية فعلية؛ ليس بعد فصل مؤقت | قوي كاتساق تاريخي | نعم لتطبيق المربين | متوسط-مرتفع |
| Foster Workflow | الرعاية البديلة مستقلة عن النسب الوراثي | قوي | نعم للانتشار والتفاصيل | مرتفع جدًا |
| Pedigree | علاقة وراثية مفتوحة العمق مع قبول النقص | قوي مفاهيميًا | نعم لمدى التوثيق | مرتفع |
| Pedigree Confidence | القيمة ومصدر الثقة منفصلان | قوي مفاهيميًا | نعم للطرق المحلية | متوسط |
| Inbreeding | تحليل مستقبلي ممكن لكنه حساس لاكتمال النسب | متوسط-قوي | نعم | منخفض في Phase 3 / مرتفع لاحقًا |
| Trial Pair | مفهوم اختياري يمكن استيعابه عبر Pair Formation Attempt | متوسط | نعم | منخفض |

---

## معايير خروج Phase 2

- ✅ Phase 2A Approved.
- ✅ Phase 2B Approved.
- ✅ Phase 2C Approved عند بدء Phase 2D.
- ✅ `PHASE-2-BASELINE.md` تم إنشاؤه.
- ✅ Cross-file consistency تمت مراجعته.
- ✅ Domain principles تم تجميعها.
- ✅ Terminology TERM-040 → TERM-091 تمت مراجعتها.
- ✅ Risks RSK-012 → RSK-016 تمت مراجعتها.
- ✅ Field Validation تم تجميعه حسب المجال والأولوية.
- ✅ Carry Forward إلى Phase 3 مكتمل.
- ✅ لا توجد Blocking Contradictions غير مسجلة.
- ✅ يمكن مراجعة Phase 2 من ملف تجميعي واحد مع الرجوع للملفات التفصيلية عند الحاجة.

## النتيجة

**Phase 2 is ready for user approval.**

Phase 2 لا تصبح `Approved` إلا بعد مراجعة واعتماد المستخدم الصريح.
