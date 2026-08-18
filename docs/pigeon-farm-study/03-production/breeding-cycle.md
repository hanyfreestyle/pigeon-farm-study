# دورة التربية والإنتاج — تحليل المجال (Breeding Cycle Domain Analysis)

> **المرحلة:** Phase 3A — تحليل دورة التربية وإدارة البيض  
> **الحالة:** Completed — Awaiting Review  
> **التاريخ:** 2026-08-18  
> **النطاق:** تحليل بداية وتتابع الأحداث الإنتاجية المتعلقة بالوضع والبطون والأعشاش وتداخل السياقات الإنتاجية، دون تحليل تفصيلي للفقس أو الزغاليل أو تصميم قاعدة بيانات.  
> **مرجع Phase 2 المعتمد:** `02-farm-structure/PHASE-2-BASELINE.md`.

---

## 1. الملخص التنفيذي

النتيجة الأساسية لـPhase 3A هي أن إنتاج الحمام لا يجب تمثيله كدورة خطية مغلقة واحدة. الزوج التشغيلي الواحد قد يكون مرتبطًا بأكثر من **بطن بيض (Clutch)** عبر الزمن، وقد يبدأ بطنًا جديدًا في عش بينما تستمر رعاية زغاليل بطن سابقة في عش آخر.

لذلك يكون التحليل مبنيًا على أحداث ومراسي واضحة، وليس على قيمة واحدة غامضة باسم `Production Cycle`.

المبدأ:

**Operational Pair → Multiple Clutches → Multiple Eggs → Independent Outcomes**

مع إمكان التداخل الزمني بين أكثر من سياق إنتاجي للزوج نفسه.

---

## 2. Production Cycle Terminology

طبقًا لـ`DEC-009` لا يوجد تعريف عالمي واحد لـ **دورة الإنتاج (Production Cycle)**.

أي Metric زمني مستقبلي يجب أن يذكر بوضوح:

- Start Event.
- End Event.
- Context.

أمثلة سليمة:

- `First Egg → Next First Egg`.
- `Clutch Start → Next Clutch Start`.
- `Hatch → Next Lay`.
- `Egg 1 → Egg 2`.
- `Observed Sustained Incubation → Hatch`.

أما عبارة:

`Production Cycle = X days`

دون مرساة، فهي غير كافية تحليليًا.

---

## 3. نموذج الأحداث الإنتاجية

الأحداث الواقعية المهمة في هذه المرحلة قد تشمل:

### أحداث بيولوجية / ملاحظة مباشرة

- Courtship observed.
- Mating observed.
- Nest activity / preparation observed.
- Egg laid.
- Additional egg laid.
- Incubation behavior observed.
- Hatch observed — يحمل للتفصيل في Phase 3B.

### أحداث إدارية

- Clutch considered complete.
- Egg checked / candled.
- Egg transferred.
- Egg removed.
- Expected hatch assigned.
- Egg marked أو identified خارجيًا إن كانت المزرعة تفعل ذلك.

هذه **Domain Events واقعية** وليست Software Events.

---

## 4. First Egg وSecond Egg

البيضة الأولى والثانية حدثان منفصلان.

### البيضة الأولى

قد يكون من المهم معرفة:

- وقت/تاريخ الملاحظة أو الوضع إذا كان معلومًا.
- العش الموجود به البيض.
- الزوج المنتج.
- الأب والأم الوراثيان وفق درجة الثقة المتاحة.
- سياق البطن.

### البيضة الثانية

تسجل كمفهوم مستقل ولا تشتق تلقائيًا من تاريخ البيضة الأولى.

الأدلة الحديثة على حمام التربية أظهرت في بعض السياقات **Clutch = 2 eggs** وفاصل وضع قريبًا من يومين، كما تدعم مراجعات التكاثر وجود بيضتين عادة خلال نحو 48 ساعة [SRC-016, SRC-003]. هذه قيم مرجعية قوية لكنها لا تتحول إلى Constant عالمي.

إذا لم تظهر البيضة الثانية فلا يتم اختلاقها.

---

## 5. تعريف البطن (Clutch)

البطن هو **تجميع إنتاجي لبيض ناتج عن نوبة وضع مرتبطة بسياق تناسلي واحد**.

البطن ليس مساويًا للعش، وليس مساويًا للدورة الكاملة.

يمكن أن يكون لدينا:

- بطن طبيعي ببيضتين.
- Single Egg Clutch.
- أكثر من بيضتين في حالة غير معتادة.
- بطن فقدت منه بيضة.
- بطن أزيلت منها بيضة.
- بطن نُقلت بيضة منها إلى Foster Pair.

لذلك:

**Clutch Identity ≠ Egg Count Constant**.

اكتمال البطن قد يكون حدثًا معروفًا بالملاحظة أو قرارًا تشغيليًا/استنتاجًا بعد مرور السياق المتوقع؛ يجب الحفاظ على مصدر المعرفة ودرجة الثقة عند الحاجة.

---

## 6. Pair → Multiple Clutches

الزوج التشغيلي لا يتغير لمجرد بدء بطن جديدة.

مثال:

```text
Operational Pair P1
  ├─ Clutch A
  ├─ Clutch B
  └─ Clutch C
```

تاريخ كل بطن مستقل، بينما يظل Pair History محفوظًا كما اعتمدته Phase 2.

---

## 7. Overlapping Production

هذه نقطة حاكمة لـ`RSK-007`.

يمكن أن يكون:

```text
Pair P1
├─ Nest 1 → Squabs from Clutch A
└─ Nest 2 → Eggs from Clutch B
```

في الوقت نفسه.

لا يعني ذلك أن Nest 1 دائمًا للعش القديم أو Nest 2 دائمًا للجديد؛ هذه مجرد حالة ممكنة.

القاعدة:

**Previous Production Context does not need to end before a new Clutch begins.**

وبالتالي لا يجوز بناء التحليل على:

`Eggs → Hatch → Squabs → End → New Cycle`

كخط إلزامي.

---

## 8. Double Nest

طبقًا لـ`DEC-012`:

**Double Nest ليس إلزاميًا.**

لكن عندما يوجد أكثر من عش، يجب أن يستطيع المجال وصف كل عش ومحتواه وسياقه الحالي بصورة مستقلة.

قد يكون العش:

- فارغًا.
- يحتوي بيضًا.
- يحتوي زغاليل.
- مستخدمًا لبطن سابقة أو لاحقة.
- خارج الاستخدام مؤقتًا.

ولا يتم ربط Nest Number تلقائيًا بعمر الدورة.

---

## 9. Nest vs Clutch

**Nest = Location / nesting context.**  
**Clutch = Production grouping of eggs.**

العش نفسه يمكن أن يستخدم لعدة بطون عبر الزمن.

كما يمكن لبيض من بطن واحدة أن ينتقل من عش إلى آخر أو إلى Foster Pair أو إلى Artificial Incubation دون تغيير أصل البطن أو النسب الوراثي للبيضة.

---

## 10. علاقة البطن بالنسب والرعاية

تطبق Phase 3A مبدأ Phase 2:

`Genetic Parentage ≠ Incubating Caregiver ≠ Rearing Caregiver`.

البطن ترتبط بالزوج/الأبوين الوراثيين بحسب البيانات المتاحة، لكن البيض قد يُحضن بواسطة طرف آخر.

لا يغير النقل:

- Genetic Father.
- Genetic Mother.
- أصل البطن.

---

## 11. Pair Movement أثناء مرحلة البيض

إذا نُقل الزوج أثناء وجود بيض، لا توجد قاعدة عالمية تقول إن البيض أو العش ينتقلان معه دائمًا.

معلومات المجال المهمة قد تشمل:

- موقع الزوج قبل وبعد النقل.
- مكان البيض قبل وبعد القرار.
- هل نقل العش؟
- هل جهز عش جديد؟
- هل تغير مقدم الحضانة؟
- سبب القرار.
- أثر النقل على استمرار البطن.

هذه تبقى **Information Requirements / Field Validation** وليست Workflow إلزاميًا.

---

## 12. Parent Loss / Pair End أثناء بطن نشطة

طبقًا لـ`DEC-019`، فقد أحد الأبوين أثناء مرحلة البيض قد ينتج عنه:

- استمرار الوالد الباقي.
- Planned/Emergency Foster Transfer حسب السياق.
- Artificial Incubation.
- فشل البطن.

النظام المستقبلي لا يقرر المسار.

كذلك إذا انتهت علاقة الزوج إداريًا أثناء وجود بطن، يجب ألا يؤدي ذلك إلى محو:

- Genetic Parentage.
- Clutch History.
- Egg History.

---

## 13. Production Attribution — مستوى مفاهيمي

لا يجوز افتراض أن كل مؤشرات الإنتاج تنسب إلى نفس الطرف بالطريقة نفسها.

مثلًا:

- Egg laying يرتبط مباشرة بالأنثى ضمن سياق الزوج.
- Clutch context يرتبط بالزوج التشغيلي/الأبوين الوراثيين.
- Fertility نتيجة تشاركية ولا تنسب بصورة مبسطة لطائر واحد دون تحليل.
- Incubation performance قد يرتبط بمقدم الحضانة الفعلي.
- Hatch outcome يرتبط بالبيضة والسياق والحضانة وعوامل أخرى.

تُرحّل صيغ Attribution وKPIs إلى Phase 6.

---

## 14. Conceptual Diagram

```text
Operational Pair P1
│
├── Clutch A
│   ├── Egg A1
│   └── Egg A2
│
└── Clutch B                    [قد يبدأ قبل نهاية سياق A]
    ├── Egg B1
    └── Egg B2
          │
          └── Foster Transfer
                 ↓
          Different Incubating Caregiver

Genetic Parents remain unchanged.
```

هذا رسم Domain Conceptual وليس Database Relations.

---

## 15. Benchmarks

القيم المستخدمة في الدراسة لا تتحول إلى Constants.

| Metric | Reference | Context |
|---|---|---|
| Clutch size | غالبًا 2 eggs | قوي في الأدلة، لكن لا يفرض عددًا ثابتًا لكل بطن |
| Egg 1 → Egg 2 | نحو 2 أيام في دراسات متعددة | يختلف ويجب تسجيل الحدث الفعلي |
| Natural incubation | نحو 17–20 يومًا | يحتاج Anchor صريح عند الحساب |
| Candling | من أيام مبكرة إلى أيام لاحقة حسب البروتوكول | ليس إجراءً أو يومًا إلزاميًا عالميًا |

كل Benchmark مستقبلي يجب أن يحمل Population/Breed/Housing/Geography/Source/Context.

---

## 16. السياق المصري

تدعم الأدلة المصرية الموجودة مسبقًا:

- وجود Individual Pair Cages في مزرعة تجارية مصرية [SRC-002].
- وجود نظم إسكان أخرى في مصر، لذلك لا تتحول أقفاص الأزواج إلى Market Fact شامل [SRC-007].
- وجود Double Nest/routine alternating nesting في بعض الأدلة المصرية البحثية، لكن الانتشار الفعلي التجاري ما زال Field Validation [SRC-005].

لا يوجد في Phase 3A ما يبرر تعميم ممارسة Candling أو Foster Egg Transfer أو Artificial Incubation على كل المزارع المصرية.

---

## 17. المخاطر

### RSK-007 — Overlapping Production Risk

**الحالة بعد Phase 3A:** Active — Materially Reduced.

تم خفضه لأن Clutch أصبحت وحدة سياق مستقلة ويمكن وجود أكثر من سياق متزامن للزوج نفسه.

يبقى الخطر قائمًا حتى تتحول هذه المبادئ لاحقًا إلى قواعد النظام الصحيحة في Phase 6/7.

### RSK-009 — Benchmark as Constant Risk

**الحالة بعد Phase 3A:** Active — Reduced.

تم تثبيت أن Clutch size، Egg Interval، Incubation Duration وغيرها قيم سياقية وليست Constants.

---

## 18. Carry Forward

### إلى Phase 3B

- Fertility confirmation.
- Candling interpretation.
- Incubation Anchor.
- Expected Hatch vs Actual Hatch.
- Embryonic development/outcomes.
- Hatch process and failures.

### إلى Phase 3C

- Egg → Hatch → Squab continuity.
- Rearing caregiver.
- Fostered squab.
- Parent loss after hatch.
- Growth / Weaning.

### إلى Phase 3D

- Production performance consolidation.
- Pair vs individual attribution.
- Failed cycle classification.
- Phase 3 consistency and baseline.

---

## 19. الاستنتاج

Phase 3A تثبت أن البنية التحليلية السليمة للإنتاج تبدأ من **الأحداث الفعلية، البطن، والبيضة الفردية** مع دعم التداخل والحركة وتعدد مقدمي الرعاية، وليس من Cycle واحدة ذات عدد أيام ثابت.

لا يوجد تعارض حابس مع `PHASE-2-BASELINE.md`.
