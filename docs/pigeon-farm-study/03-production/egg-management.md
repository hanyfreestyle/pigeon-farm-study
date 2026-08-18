# إدارة البيض — تحليل المجال (Egg Management Domain Analysis)

> **المرحلة:** Phase 3A — تحليل دورة التربية وإدارة البيض  
> **الحالة:** Completed — Awaiting Review  
> **التاريخ:** 2026-08-18  
> **النطاق:** هوية البيضة وتسلسلها وعلاقتها بالبطن والعش والنسب والحضانة والنقل والنتائج الأولية، دون تحليل تفصيلي للفقس أو الزغاليل أو تصميم تقني.

---

## 1. المبدأ الأساسي

كل بيضة يجب أن تكون **قابلة للتمييز مفاهيميًا على مستوى المجال** حتى لو لم تحمل رقمًا ظاهرًا للمربي.

يجب أن نستطيع تفسير:

- أي بيضة نتحدث عنها؟
- من أي بطن؟
- من أي أبوين وراثيين؟
- في أي عش توجد الآن؟
- هل نُقلت؟
- من يحضنها الآن؟
- ما حالتها الحالية؟
- ما نتيجتها النهائية لاحقًا؟

**Egg Identity ≠ Egg Sequence.**

---

## 2. Egg Identity vs Egg Sequence

`Egg 1` و`Egg 2` يصفان ترتيب الوضع داخل البطن، وليس هوية دائمة للبيضة نفسها.

قد تكون لدينا بيضة معروفة الهوية لكن ترتيبها غير مؤكد، خصوصًا عند:

- التسجيل المتأخر.
- Loft / Colony.
- نقل البيض.
- وجود بيض إضافي.

لذلك:

**Lay Order / Sequence ≠ Egg Identity**.

---

## 3. Egg Information Requirements

قد يحتاج المجال إلى معرفة:

- البيضة المقصودة.
- Lay date/time إذا كان معلومًا.
- Sequence داخل البطن إذا كان معلومًا.
- Clutch association.
- Nest / physical location الحالي.
- Genetic Father / Mother.
- Incubating Caregiver.
- Current condition.
- Transfer history.
- Observation / confidence source.
- Final outcome لاحقًا.

هذه ليست Database Fields نهائية.

---

## 4. Missing Second Egg

إذا وُجدت Egg 1 ولم تظهر Egg 2:

لا يتم اختلاق بيضة ثانية.

يمكن وصف الواقع مثل:

- Single Egg Clutch.
- Expected second egg not observed.
- Clutch completeness uncertain.
- Unknown outcome.

ولا يتم تشخيص سبب طبي في Phase 3A.

---

## 5. Extra Egg

وجود أكثر من بيضتين يجب أن يكون ممكن الوصف دون افتراض السبب.

الأسباب المحتملة قد تشمل:

- Variation.
- Egg from another bird.
- Foster / transfer situation.
- Colony attribution confusion.

لكن لا يتم اختيار سبب دون دليل.

---

## 6. Egg Parentage

تطبق قاعدة Phase 2:

`Genetic Parentage ≠ Incubating Caregiver`.

البيضة لها أب وأم وراثيان إذا أمكن معرفتهما بدرجة ثقة كافية.

نقل البيضة لا يغير:

- Genetic Father.
- Genetic Mother.

حتى لو تغير:

- Nest.
- Location.
- Foster Pair.
- Incubating Caregiver.

---

## 7. Unknown Egg Parentage

في Loft/Colony قد يوجد بيض معروف العش أو الموقع لكن Parentage غير مؤكدة.

يجب السماح بـ:

- Known parentage.
- Partially known parentage.
- Reported parentage.
- Inferred parentage.
- Unknown parentage.

مع تطبيق `Data Confidence / Provenance` من Phase 2.

**Unknown Parentage ≠ Invalid Egg Record.**

---

## 8. Egg Attribution Confidence

قد تحتاج الثقة إلى التطبيق على:

- Genetic Parents.
- Clutch association.
- Lay order.
- Lay date.
- Egg source.

مثال:

بيضة شوهدت صباحًا داخل Nest بعد عدم وجودها مساء اليوم السابق؛ تاريخ الوضع قد يكون **Estimated/Observed window** وليس Timestamp مؤكدًا.

---

## 9. Egg Location

يجب الفصل بين:

`Genetic Origin`

و:

`Current Physical Location`

و:

`Incubating Caregiver`.

قد تنتقل البيضة:

`Nest A → Nest B`

أو:

`Genetic Pair → Foster Pair`

أو:

`Nest → Artificial Incubator`

دون تغيير النسب.

---

## 10. Egg Movement

الحركة مهمة تاريخيًا عندما تغير مكان البيضة أو مقدم الحضانة أو تفسير النتيجة.

أمثلة:

- Foster Transfer.
- Transfer to artificial incubator.
- Transfer between nests.
- Return after temporary move.
- Intentional removal.

قد يكون من المهم معرفة:

- From.
- To.
- Date/time.
- Reason.
- Stage.
- Decision maker.
- Caregiver before/after.

---

## 11. Planned Foster Transfer

وفق `OQ-020` و`DEC-018`:

يمكن أن يتم نقل بيضة مخططًا من زوج وراثي إلى Foster Pair.

معلومات المجال المهمة:

- Genetic Pair.
- Source nest.
- Destination pair/nest.
- Transfer date.
- Egg stage.
- Reason.
- Incubating caregiver after transfer.

**Planned Foster Transfer لا يغير Genetic Parentage.**

---

## 12. Emergency Foster Transfer

وفق `DEC-019` قد يحدث النقل بسبب:

- Parent loss.
- Incubation failure.
- Emergency management decision.

الفرق عن Planned Transfer هو **سبب وسياق القرار**، وليس النسب.

---

## 13. Artificial Incubation

الحضانة الصناعية مسار Domain ممكن:

`Egg → Artificial Incubation`.

في هذه الحالة:

- Genetic Parents تبقى معروفة/محتملة كما هي.
- لا يوجد Foster Pair حاضن بالضرورة.
- Current Incubation Method تختلف عن الطبيعية.

انتشارها في مزارع الحمام اللاحم المصرية:

**Requires Field Validation.**

---

## 14. Egg Condition vs Final Outcome

يجب الفصل بين:

### Current Condition

مثل:

- Intact.
- Under incubation.
- Transferred.
- Removed temporarily.
- Development observed.

### Final Outcome

مثل:

- Hatched.
- Infertile.
- Embryonic death.
- Dead-in-shell.
- Broken.
- Missing.
- Removed/discarded.
- Abandoned.

لا تتحول هذه القوائم إلى Enum في هذه المرحلة.

---

## 15. Removed / Lost / Transferred / Discarded

هذه ليست نتيجة واحدة.

- **Removed:** أُخرجت عمدًا من مكانها.
- **Transferred:** نقلت إلى موقع/مقدم رعاية آخر مع استمرار سياقها.
- **Lost/Missing:** مكانها أو مصيرها غير معلوم.
- **Discarded:** قرار بالتخلص منها/عدم استمرارها.

الحفاظ على الفرق مهم لتفسير الأداء لاحقًا.

---

## 16. Fertility

وجود البيضة لا يعني أن Fertility معروفة.

المراحل المعرفية قد تكون:

- Fertility unknown.
- Fertility suspected/inferred.
- Fertile/developing observed.
- Infertile/clear assessed.

لكن كيفية التأكيد وتوقيت التقييم يحملان إلى Phase 3B.

لا يتم حساب Fertility KPI هنا.

---

## 17. Candling

`Candling` إجراء مراقبة غير هدّام نسبيًا يستخدم لرؤية مؤشرات التطور داخل البيضة.

الأدلة المستخدمة في الدراسة تظهر اختلافًا في توقيت الفحص:

- دراسة استخدمت Candling في اليوم 5 من الحضانة لتحديد البيض المخصب [SRC-006/مرتبط بأدلة التغذية السابقة].
- دراسات أخرى استخدمته في Day 7 أو أكثر [SRC-018 ومصادر Phase 3A].
- أبحاث حديثة طورت كشفًا آليًا مبكرًا في الأيام 1–4، لكنها لا تجعل هذه التقنية ممارسة مزرعية معيارية [SRC-018].

النتيجة:

**Candling Timing ≠ Universal Constant.**

ولا يفترض أن كل المزارع تستخدم Candling.

---

## 18. CON-006 — Incubation Anchor Analysis

`CON-006` لا يغلق بتخمين.

يجب التمييز بين:

1. Egg 1 laid.
2. Egg 2 laid.
3. First observed incubation behavior.
4. Observed sustained incubation.
5. Management-selected prediction anchor.

الأدلة البيولوجية توضح أن توقيت بدء الحضانة يؤثر في تزامن الفقس، وأن بعض الأزواج قد تبدأ الحضانة قبل اكتمال وضع البيض؛ لذلك لا توجد مرساة واحدة يمكن فرضها عالميًا.

### Status after Phase 3A

**Analyzed — Definition/Policy Choice Still Open for Phase 3B.**

ليس هناك تعارض؛ هناك أكثر من Anchor صحيحة حسب المقصود.

---

## 19. Expected Hatch Date

**Expected Hatch Date = Prediction.**

وليست Biological Fact.

يمكن أن تعتمد مستقبليًا على Policy واضحة مثل:

- Egg 1.
- Egg 2.
- Observed sustained incubation.
- Manual expected date.

لكن Phase 3A لا تعتمد واحدة كقاعدة عالمية.

---

## 20. Actual Hatch

**Actual Hatch = Observation / Biological Event.**

ويجب أن يبقى مستقلًا عن Expected Hatch.

الفرق:

`Prediction ≠ Observation`.

يُحلل الفقس تفصيليًا في Phase 3B.

---

## 21. Incubation Duration Metrics

لا تستخدم عبارة `Incubation Duration` دون تحديد Start Anchor.

يمكن أن توجد Metrics مختلفة:

- Egg 1 → Hatch.
- Egg 2 → Hatch.
- Sustained incubation → Hatch.

كل واحدة تقيس معنى مختلفًا.

---

## 22. Failed Clutch

`Failed Clutch` وصف نتيجة عامة، وليس سببًا واحدًا.

قد ينتج الفشل عن:

- infertility.
- embryonic loss.
- broken eggs.
- abandonment.
- missing eggs.
- parent loss.
- management decision.

لذلك:

**Clutch Outcome ≠ Failure Cause.**

---

## 23. Abandoned Clutch

إذا توقف الزوج عن الحضانة، يمكن وصف البطن بأنها مهجورة/متروكة تشغيليًا إذا كان ذلك معلومًا.

لكن Phase 3A لا تشخص السبب؛ قد يكون:

- سلوكًا.
- disturbance.
- health issue.
- parent loss.
- management action.

السبب يحتاج دليلًا مستقلًا.

---

## 24. Parent Loss During Egg Stage

طبقًا لـ`DEC-019` المسارات الممكنة:

- surviving parent continues incubation.
- Emergency Foster Transfer.
- Artificial Incubation.
- clutch failure.

النظام المستقبلي يعرض ويسجل القرار، ولا يتخذه تلقائيًا.

---

## 25. Pair End During Active Clutch

انتهاء Operational Pair لا يمحو:

- Genetic Parentage.
- Clutch association.
- Egg history.
- transfer/caregiving history.

هذه قاعدة حفظ تاريخ تمتد من Phase 2.

---

## 26. Egg → Hatch Continuity

البيضة قد تؤدي إلى زغلول عند الفقس:

`Egg → Hatched Squab`.

لكن إدارة الزغلول لا تبدأ في Phase 3A.

يجب حمل استمرارية الهوية/المصدر إلى Phase 3B/3C.

---

## 27. Production Attribution

Attribution تختلف حسب Metric:

- Lay event يرتبط بالأنثى/الزوج.
- Genetic parentage بالأب والأم.
- Incubation performance بمقدم الحضانة الفعلي.
- Hatch outcome بالبيضة مع سياق الحضانة.

لا يتم إنشاء Formula أو KPI في Phase 3A.

---

## 28. Observation vs Inference

### Observation

- Egg observed.
- Hatch observed.
- Mating observed.
- Egg broken observed.

### Inference / Reported

- Fertility inferred.
- Lay date estimated.
- Parentage reported.
- Egg source inferred.

يجب تطبيق Data Confidence / Provenance حيث يكون الفرق مؤثرًا.

---

## 29. New Material Risks Identified

### Egg Identity Confusion

خلط Egg 1/Egg 2 كترتيب بهوية البيضة نفسها.

### Clutch Overlap Misattribution

نسبة بيض بطن جديدة إلى سياق سابق بسبب التداخل.

### Foster Transfer Parentage Error

تغيير Parentage خطأً عند نقل البيضة.

### Prediction-as-Fact Risk

تحويل Expected Hatch إلى حقيقة أو اعتبار فوات التوقع Hatch Failure تلقائيًا.

تم تسجيلها في `risks.md`.

---

## 30. Field Validation Required

- هل يسجل المربي Egg 1 وEgg 2 منفصلين؟
- كيف يميز البيض داخل البطن؟
- هل يسجل Clutch مستقلًا؟
- متى يعتبر البطن مكتملًا؟
- كيفية التعامل مع Single Egg Clutch.
- Extra Egg scenarios.
- Double Nest usage.
- Candling usage and timing.
- من أي Anchor يحسب المربي موعد الفقس؟
- Foster Egg Transfer.
- Artificial Incubation.
- Egg marking/numbering.
- Pair movement أثناء وجود البيض.

---

## 31. الاستنتاج

البيضة ليست مجرد Count داخل الزوج؛ هي وحدة إنتاج واقعية لها هوية وسياق ونسب وموقع ومقدم حضانة وتاريخ حركة ونتيجة محتملة. هذا الفهم يمنع فقد المعلومات عند التداخل أو النقل أو فشل بعض البيض داخل البطن نفسها.
