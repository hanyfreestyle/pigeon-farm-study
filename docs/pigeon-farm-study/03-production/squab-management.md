# إدارة الزغاليل — تحليل المجال (Squab Management Domain Analysis)

> **المرحلة:** Phase 3C — تحليل إدارة الزغاليل  
> **الحالة:** Completed — Awaiting Review  
> **التاريخ:** 2026-08-18  
> **النطاق:** الانتقال من الفقس إلى الزغلول، الهوية، الرعاية، Crop Milk، النمو والوزن، Foster/Hand Feeding، الفصل والفطام، الحركة والنتائج التشغيلية؛ دون KPIs نهائية أو صحة تفصيلية أو تغذية أو ماليات أو تصميم تقني.  
> **المراجع المعتمدة:** `02-farm-structure/PHASE-2-BASELINE.md`، `03-production/breeding-cycle.md`، `03-production/egg-management.md`، `03-production/hatching.md`.

---

## 1. الملخص التنفيذي

Phase 3C تثبت أن الزغلول ليس "ناتجًا عدديًا" فقط، بل هو **نفس الفرد الحيواني** الذي تبدأ هويته عند الفقس ويجب أن يظل مرتبطًا بالبيضة المحددة التي خرج منها وبـClutch والأبوين الوراثيين ومقدمي الحضانة والرعاية.

المبدأ:

**Hatched Egg → Specific Squab → Same Bird Identity through later life stages**

كما تثبت أن:

- `Genetic Parentage ≠ Rearing Caregiver`.
- `Separation ≠ Physiological Weaning`.
- `Weaning Readiness ≠ Market Readiness ≠ Sale Decision`.
- `Single Weight ≠ Growth Trend`.
- `Squab Life Stage ≠ Bird Status ≠ Bird Role`.
- `Squab Outcome ≠ Mortality / Failure Cause`.

---

## 2. Egg → Squab Continuity

طبقًا لـ`DEC-032`:

**Hatched Egg → Specific Squab**.

عند الفقس الناجح يجب أن تبقى الاستمرارية المفاهيمية قادرة على تفسير:

- Egg Identity الأصلية.
- Clutch.
- Genetic Father / Mother.
- Incubating Caregiver history.
- Hatch context.
- Squab / Bird Identity الناتجة.

ولا يجوز اختزال الفقس إلى مجرد:

`1 squab produced`.

---

## 3. تعريف الزغلول (Squab)

الزغلول هو الطائر الصغير بعد الفقس خلال مرحلة اعتماده المبكر والنمو السريع قبل الانتقال إلى مرحلة الطائر اليافع (Young Bird).

يجب عدم فرض عمر رقمي عالمي للفصل بين:

- Newly Hatched Squab.
- Dependent Squab.
- Growing Squab.
- Weaning-stage Bird.
- Young Bird.

لأن الانتقال يعتمد على التطور وطريقة الرعاية والسلالة والإدارة، وليس العمر وحده.

---

## 4. Squab Identity vs Bird Identity

Phase 2B عرّفت **Bird Identity** كهوية الفرد المستمرة عبر الزمن.

Phase 3C لا تنشئ هوية منفصلة تنافسها.

النتيجة:

**Squab هو Bird في Life Stage مبكرة، وليس فردًا جديدًا منفصلًا عن Bird Identity.**

أي أن:

- الهوية تبدأ مع الفرد بعد الفقس.
- Life Stage قد تتغير من Squab إلى Young Bird ثم لاحقًا أدوار أخرى.
- تغير المرحلة لا ينشئ فردًا جديدًا.

هذا يمنع Duplicate Identity مستقبلًا.

---

## 5. Genetic Parents vs Rearing Caregiver

الأب والأم الوراثيان لا يتغيران بعد الفقس حتى لو:

- نُقل الزغلول.
- رعاه Foster Pair.
- مات أحد الأبوين.
- استكمل أحد الأبوين الرعاية منفردًا.
- استخدمت Hand Feeding.

القاعدة:

**Genetic Parentage ≠ Rearing Caregiver**.

وقد يكون مقدم التربية:

- Genetic Pair.
- Foster Pair.
- One surviving parent.
- Hand-feeding caregiver.
- Dedicated care system.
- Mixed / changed caregivers عبر الزمن.

---

## 6. Rearing Caregiver History

يمكن أن يتغير مقدم الرعاية للزغلول نفسه.

مثال:

`Genetic Pair → Foster Pair → Hand Feeding`.

لذلك يحتاج المجال إلى **Rearing Caregiver History** وليس `Current Caregiver` فقط.

المعلومات الدومينية المهمة عند التغيير:

- caregiver before.
- caregiver after.
- date/time context.
- reason.
- location.
- squab age/stage.
- observed outcome later.

هذه Information Requirements وليست Database Fields.

---

## 7. دور الأبوين بعد الفقس

الأدلة تدعم أن الذكر والأنثى يشاركان في رعاية الزغاليل وإطعامها، ولا يصح افتراض أن جنسًا واحدًا يقوم بالرعاية كاملة في المسار الطبيعي [SRC-003, SRC-004, SRC-005].

أوجه الرعاية تشمل:

- feeding / regurgitation.
- crop milk delivery في المرحلة المبكرة.
- warming / brooding.
- nest attendance.
- protection.

وقد يتغير توزيع الرعاية مع العمر والسياق.

---

## 8. Crop Milk

**Crop Milk / Pigeon Milk** مكوّن بيولوجي أساسي في الرعاية المبكرة للزغاليل، وينتجه كلا الجنسين.

الأدلة تؤكد أن الزغاليل Altricial وتعتمد بدرجة كبيرة على Crop Milk في الأيام الأولى، وأن جودة/كمية Crop Milk ترتبط بالنمو والبقاء [SRC-003, SRC-021].

تظهر المراجعات الحديثة أن الاعتماد يكون قويًا جدًا في الأسبوع الأول، ثم تنتقل تغذية الزغلول تدريجيًا إلى مواد أكثر اعتمادًا على الغذاء الذي يتناوله الأبوان وتنقله الرعاية الأبوية.

لا يتم في Phase 3C تحليل:

- Feed formulation.
- Nutrient requirements.
- Crop milk replacer composition.

فهذه موضوعات Phase 4.

---

## 9. Early Dependency

الزغلول في الأيام الأولى شديد الاعتماد بسبب:

- ضعف القدرة على التغذية المستقلة.
- الاعتماد على الرعاية الحرارية والحماية.
- الاعتماد الغذائي على الأبوين/Crop Milk.
- سرعة النمو والحساسية لفقد الرعاية.

القاعدة:

**Biological Dependency ≠ Management Separation**.

يمكن أن يفصل المربي الزغلول إداريًا قبل أن يصبح مستقلاً فسيولوجيًا، لكن هذا يتطلب مسار رعاية بديلًا ولا يعني أن الطائر أصبح Weaned بيولوجيًا.

---

## 10. Early Post-Hatch Observations

من منظور إدارة الإنتاج، قد تكون الملاحظات المبكرة المهمة:

- survival / alive observation.
- evidence of feeding.
- parental attendance.
- body condition.
- sibling size difference.
- nest condition.
- unusual weakness.
- caregiver availability.

لا يتم تشخيص الأمراض في هذه المرحلة؛ الحالات الصحية تحمل إلى Phase 4.

---

## 11. Siblings and Hatch Asynchrony

Clutch من بيضتين قد تنتج:

- 0 Squabs.
- 1 Squab.
- 2 Squabs.
- حالات استثنائية أخرى بحسب Clutch غير النمطية.

إذا فقست البيضتان في أوقات مختلفة، فقد يختلف الزغلولان في:

- العمر الفعلي.
- الحجم.
- النمو.
- القوة التنافسية.

لذلك:

**Same Clutch ≠ Exactly Same Age**.

ولا يجوز اشتقاق عمر الزغلولين من Clutch فقط إذا كان Actual Hatch لكل بيضة معروفًا بصورة أدق.

---

## 12. Age and Hatch Date

يجب الفصل بين:

- Exact Hatch Date/Time when observed.
- Approximate Hatch Date.
- Age derived from known hatch.
- Estimated Age.

العمر المشتق من Actual Hatch ليس Manual Fact مستقلًا، بل نتيجة يمكن حسابها لاحقًا.

وعند ضعف الملاحظة يجب حفظ مستوى الثقة بدل اختلاق دقة غير موجودة.

---

## 13. Squab Growth

النمو في Phase 3C يُفهم كمجموعة ملاحظات عبر الزمن تشمل:

- age.
- body weight.
- body condition.
- physical development.
- feather development where useful.
- survival.
- rearing method/context.

ولا يتم تعريف KPI نهائي هنا.

القاعدة:

**Single Measurement ≠ Growth Performance**.

---

## 14. Weight Observations

وزن الزغلول **Measured Observation** يمكن تكراره عبر الزمن.

يجب الفصل بين:

- Single Weight.
- Repeated Weight Observations.
- Growth Trend.

سياق الوزن قد يشمل:

- age / hatch anchor.
- exact vs estimated age.
- date/time.
- breed / strain.
- rearing method.
- measurement method عندما يكون مؤثرًا.

ولا يتم اعتماد وزن عالمي لعمر محدد.

---

## 15. Growth Benchmark Policy

طبقًا لـ`RSK-009`:

**Growth Benchmark ≠ Constant**.

أي Benchmark للعمر/الوزن يجب أن يحتفظ بسياقه:

- source.
- breed / strain.
- housing.
- rearing method.
- geography.
- age anchor.
- measurement method.
- confidence.

يمكن أن يكون `Slow Growth` أو `Below Expected Growth` مفهومًا تحليليًا، لكن Thresholds تحمل إلى Phase 3D / Phase 6.

---

## 16. Rearing Methods

تم الفصل بين مسارات الرعاية التالية:

- Parent-reared.
- Foster-reared.
- Hand-fed.
- Mixed-reared.
- Dedicated / artificial care where applicable.

هذه ليست متساوية افتراضيًا في:

- labor.
- biological dependency.
- growth.
- mortality risk.
- welfare implications.

ولا يتم اعتماد أحدها كـBest Practice عالمية.

---

## 17. Fostered Squab

إذا نُقل الزغلول إلى Foster Pair:

- Genetic Father/Mother يبقيان كما هما.
- Rearing Caregiver يتغير.
- Location قد تتغير.
- Transfer history يجب أن يبقى مفهومًا.

القاعدة:

**Foster Rearing changes care, not parentage.**

---

## 18. Planned Squab Transfer

يمكن أن يكون نقل الزغاليل مخططًا في بعض نظم التربية لأسباب مثل:

- إدارة حمل الرعاية.
- استخدام Foster Stock.
- حماية ناتج ذي قيمة وراثية عالية.
- استراتيجية تشغيلية خاصة.

لكن مدى انتشار هذا الاستخدام في مزارع اللحم المصرية يحتاج **Field Validation**.

ولا يفترض أنه Workflow أساسي لكل مزرعة.

---

## 19. Emergency Squab Transfer

طبقًا لـ`DEC-019`، النقل الطارئ يختلف عن النقل المخطط.

قد يحدث بسبب:

- parent death.
- abandonment.
- insufficient care.
- emergency condition.

المبدأ:

**Planned Transfer ≠ Emergency Transfer**.

والقرار النهائي للمسار يبقى للمربي/مدير المزرعة.

---

## 20. Parent Loss After Hatch

عند فقد أحد الأبوين بعد الفقس، المسارات الممكنة قد تشمل:

- surviving parent continues.
- Foster Pair.
- Hand Feeding.
- Dedicated Care.
- loss / production failure.

الدراسة المصرية الخاصة بفقد أحد الأبوين أو كليهما تدعم أن الرعاية بواسطة أب/أم واحد أو foster/hand-rearing مسارات واقعية ذات نتائج نمو ورفاهية مختلفة [SRC-005].

النظام المستقبلي لا يقرر تلقائيًا أي مسار هو الصحيح.

---

## 21. One-parent Rearing

يمكن أن يستمر أحد الأبوين في رعاية الزغاليل بعد فقد الشريك في بعض الحالات [SRC-005].

لكن:

**Possible ≠ Guaranteed Successful**.

يجب وصفها كمسار ممكن مع متابعة النتيجة، لا كقاعدة نجاح ثابتة.

---

## 22. Hand Feeding

Hand Feeding مسار رعاية حقيقي في الحمام، وقد يستخدم في:

- emergency rearing.
- planned early separation.
- high-value / ornamental contexts.
- research/intensive systems.

لكن Phase 3C لا تقدم بروتوكول تغذية أو تركيبة غذائية.

التطبيق المصري التجاري الواسع يحتاج تحققًا ميدانيًا.

---

## 23. Early Separation — Evidence and Boundary

الدراسة المصرية الحديثة على مزرعة تجارية بطريق القاهرة–الإسكندرية اختبرت White Mirthys مع الفصل عند:

- hatch (`W0`).
- 7 days (`W7`).
- 28 days (`W28`).

وأظهرت أن الفصل عند الفقس:

- سرّع العودة التناسلية للأبوين ورفع الناتج العددي في فترة الدراسة.
- لكنه خفض وزن/نمو الزغاليل ورفع النفوق مقارنة بـW7 وW28.

بينما لم تظهر فروق جوهرية مماثلة بين W7 وW28 في بعض نتائج النمو والنفوق في هذه التجربة [SRC-002].

هذه **نتيجة Research Context-specific** لسلالة ونظام وإدارة محددة، وليست Best Practice مصرية عامة.

---

## 24. Separation ≠ Physiological Weaning ≠ Market Age

هذه قاعدة إلزامية:

**Early Separation ≠ Physiological Weaning ≠ Market Age**.

إزالة الزغلول من الأبوين حدث إداري.

الاستقلال عن الرعاية/التغذية الأبوية تطور بيولوجي/وظيفي.

والسوق قرار تجاري منفصل.

---

## 25. Weaning Definition

مصطلح **Weaning / الفطام** قد يستخدم بمعان مختلفة، ولذلك يجب تحديد المقصود.

دومينيًا من الأفضل الفصل بين:

- reduced dependence on crop milk / parental feeding.
- ability to self-feed adequately.
- physical separation from parents.
- management declaration of weaned status.

لا يُختزل الفطام في العمر وحده.

---

## 26. Weaning Readiness

المؤشرات المحتملة قد تشمل:

- self-feeding observed.
- water intake.
- body development.
- feathering.
- behavior.
- age.
- weight.

لكن لا يوجد Threshold عالمي معتمد في Phase 3C.

ويجب الفصل بين:

`Observed self-feeding`

و:

`Management decision: Weaning complete`.

---

## 27. Market Readiness

الجاهزية للتسويق مفهوم تجاري لا يساوي الفطام.

تم تثبيت:

**Weaning Readiness ≠ Market Readiness ≠ Sale Decision**.

قد تعتمد Market Readiness على:

- buyer specification.
- live/dressed sale.
- weight.
- age.
- breed.
- condition.
- farm strategy.

التفاصيل المصرية تحمل إلى Phase 5 وMarket Validation.

---

## 28. Market Age / Market Weight

النطاقات مثل 21–28 يومًا وأوزان معينة مفيدة كـBenchmarks في بعض الدراسات/النظم، لكنها ليست Constants.

لا يعتمد Phase 3C:

- Universal Market Age.
- Universal Market Weight.

وتبقى `OQ-015` مرتبطة بالتحقق من السوق المصري.

---

## 29. Squab Status vs Life Stage

`Squab` وصف **Life Stage**.

أما حالات مثل:

- healthy.
- weak.
- under treatment.
- missing.

فهي Status/Condition.

وأوصاف مثل:

- foster-reared.
- replacement candidate later.

هي Role/History/Management context بحسب الحالة.

القاعدة:

**Life Stage ≠ Status ≠ Role**.

---

## 30. Squab Location and Movement

هوية الزغلول لا تعتمد على موقعه.

قد يوجد في:

- genetic nest.
- foster nest/cage.
- dedicated care area.
- treatment area.
- separation/growing area.

الحركة تصبح تاريخيًا مهمة عندما تؤثر على:

- caregiver.
- rearing method.
- health context.
- separation.
- sale preparation.
- interpretation of growth/performance.

`Location Identity ≠ Squab/Bird Identity`.

---

## 31. Squab Mortality

Death حدث نهائي للزغلول، لكن Phase 3C لا تبدأ Mortality Module.

يمكن التمييز وصفيًا بين:

- pre-weaning death.
- post-weaning death.
- unknown stage.

عندما يكون تعريف Weaning واضحًا في السياق.

لكن:

**Mortality Outcome ≠ Mortality Cause**.

ولا ينسب السبب تلقائيًا إلى:

- Genetic Pair.
- Foster Pair.
- feed.
- disease.

التشخيص يحمل إلى Phase 4.

---

## 32. Missing Squab

في Loft / Colony قد يكون Missing event ذا معنى أكبر من نظام القفص المغلق.

القاعدة:

**Missing ≠ Dead**.

ويجب الحفاظ على Outcome غير المؤكد بدل اختلاق Death.

---

## 33. Squab Sale / Retention / Culling

من منظور المجال يمكن أن ينتهي سياق الزغلول بعدة نتائج:

- sold as squab.
- retained / continues growing.
- transferred.
- selected later for replacement pathway.
- culled.
- died.
- missing / unknown.

لا يتم تصميم Sales Module هنا.

إذا بيع الزغلول، يجب ألا يُمحى تاريخه كنتاج Pair/Clutch/Egg.

---

## 34. Replacement Pathway

الزغلول المحتفظ به لا يجب إجباره على الانتقال مباشرة إلى Breeding Stock.

المسار المحتمل:

**Squab → Young Bird → Replacement Candidate → Selected Replacement → Breeding Stock**

بحسب قرارات Phase 2B.

هذا المسار اختياري وليس Mandatory لكل زغلول محتفظ به.

---

## 35. Squab Production Outcome

Final Squab Production Outcome قد يصف نهاية سياق إنتاج الزغلول مثل:

- survived beyond squab stage.
- sold as squab.
- retained.
- transferred.
- culled.
- died.
- missing / unknown.

هذه مفاهيم Domain وليست Enum نهائية.

---

## 36. Pair Production Attribution

لا ينسب كل شيء للزوج بالطريقة نفسها.

طبقات مختلفة:

- Egg Production.
- Fertility.
- Hatch.
- Squab Survival.
- Growth.
- Market Output.

إذا أنتجت Genetic Pair البيضة وربى Foster Pair الزغلول، يجب الفصل بين:

- genetic production.
- incubation result.
- rearing result.
- final market output.

تعريف Metrics يحمل إلى Phase 3D / Phase 6.

---

## 37. Performance by Rearing Method

من المفيد مستقبلًا مقارنة:

- parent-reared.
- foster-reared.
- hand-fed.
- early-separated.
- mixed-reared.

لكن Phase 3C لا تحسب KPIs ولا تضع Thresholds.

---

## 38. Squab Cohort

قد يكون **Squab Cohort** مفهومًا تحليليًا مفيدًا لتجميع طيور تشترك في:

- hatch period.
- barn/location.
- breed/strain.
- rearing method.
- production study/batch context.

لكن الحمام التجاري ذو الإنتاج المتداخل لا يفرض Batch Model طبيعيًا مثل Broiler Flock.

لذلك:

**Cohort = Optional Analytical Grouping, not mandatory production hierarchy.**

---

## 39. RSK-007 Recheck — Overlap

Phase 3C لا تعيد النموذج إلى دورة خطية.

يمكن للزوج في الوقت نفسه:

- رعاية Squabs من Clutch A.
- حضانة أو وضع Eggs من Clutch B.

وبالتالي:

**Squab Stage does not close Pair production context.**

حالة `RSK-007` تبقى مخفضة جوهريًا مع استمرار حملها إلى Phase 7.

---

## 40. RSK-022 Recheck — Egg-to-Squab Link

Phase 3C أكدت أن Squab هو استمرار نفس الفرد الحيواني بعد الفقس، مع الحفاظ على الربط:

`Egg Identity → Squab/Bird Identity`.

لذلك أصبحت `RSK-022`:

**Active — Materially Reduced**.

ويجب لاحقًا ضمان ذلك في Phase 7 Data Model.

---

## 41. المصري والسياق الميداني

لدينا دليل مصري مباشر مهم في نقطتين:

1. دراسة Commercial Farm على طريق القاهرة–الإسكندرية قارنت الفصل عند hatch/7/28 يومًا في White Mirthys وأظهرت trade-off واضحًا بين زيادة سرعة عودة الأبوين للإنتاج وبين نمو/نفوق الزغاليل عند الفصل في يوم الفقس [SRC-002].
2. دراسة مصرية عن فقد أحد الأبوين أو كليهما وثقت One-parent rearing وFoster/Hand-rearing كمسارات عملية ذات آثار مختلفة على النمو والرفاهية [SRC-005].

لكن لا يجوز تعميم:

- W0/W7/W28.
- hand feeding.
- foster practice.
- 21–28 day market/weaning window.

كمعايير سوق مصرية عامة دون Field Validation.

---

## 42. Benchmark Summary

Benchmarks المفيدة لكنها السياقية تشمل:

- rapid early growth.
- strong dependence on crop milk in first week.
- traditional weaning/market region around 21–28 days in several references.
- study-specific body weights by breed/rearing system.

أي Benchmark يجب أن يحمل Context ولا يتحول إلى Constant.

---

## 43. Biological vs Management Events

### Biological / observed

- Hatch completed.
- Feeding observed.
- Growth.
- Self-feeding observed.
- Development.
- Death.

### Management

- Weigh.
- Transfer.
- Foster assignment.
- Hand feeding decision.
- Early separation.
- Declare weaned.
- Select for replacement.
- Mark market-ready.

`Biological Event ≠ Management Decision`.

---

## 44. Data Confidence / Provenance

يطبق على:

- hatch date/time.
- age.
- weight measurement.
- caregiver history.
- separation date.
- weaning assessment.
- market-readiness assessment.
- mortality/failure cause.

ولا يتم تحويل Estimated/Reported/Observed إلى Verified دون دليل.

---

## 45. Field Validation Required

يحتاج تحققًا ميدانيًا مصريًا خصوصًا:

1. متى يبدأ المربي اعتبار الطائر Squab مقابل Young Bird؟
2. متى وكيف يتم تعريف/تمييز الزغلول فرديًا؟
3. توقيت وترتيب وزن الزغاليل في المزارع التجارية.
4. استخدام Growth Baselines.
5. Parent-rearing vs Foster-rearing prevalence.
6. Planned Squab Transfer.
7. Emergency Foster Transfer.
8. One-parent rearing decisions.
9. Hand Feeding prevalence.
10. Early Separation timing.
11. معنى Weaning المستخدم محليًا.
12. مؤشرات Weaning Readiness.
13. Market Age / Market Weight.
14. Live vs dressed sale specifications.
15. Squab movement / dedicated growing areas.
16. Mortality stage classification.
17. Replacement selection timing from young stock.
18. Foster attribution in farm records.

---

## 46. Carry Forward to Phase 3D

- Fertility / Hatchability metric definitions.
- Squab Survival metrics.
- Growth trend / weight gain metrics.
- Egg → Hatch → Squab → Market output funnel.
- Pair vs Individual vs Caregiver attribution.
- Foster-rearing performance.
- Early separation performance.
- Mortality outcome reporting.
- Cohort comparison where useful.
- Failed production classification.
- Phase 3 consolidated baseline.

---

## 47. Carry Forward to Phase 4

- Crop Milk / Feed relationship.
- Hand-feeding formulation and safety.
- Health causes of slow growth.
- Squab mortality diagnosis.
- Treatment.
- Welfare implications of early separation/hand feeding.
- Environmental care requirements.

---

## 48. Carry Forward to Phase 5

- Market Age/Weight validation.
- Buyer specifications.
- Live vs dressed sale.
- Squab sale.
- Price/value.
- retained vs sold economic decision.

---

## 49. Phase 3C Exit Assessment

تحققت المعايير التالية:

- Egg→Squab continuity preserved.
- Squab Identity analyzed.
- Squab vs Bird Identity clarified.
- Genetic vs Rearing caregiver separated.
- Caregiver history analyzed.
- Crop Milk analyzed.
- Early dependency analyzed.
- Growth and Weight observations analyzed.
- Growth benchmarks contextualized.
- Fostered squabs analyzed.
- Planned/Emergency transfers analyzed.
- Parent loss after hatch analyzed.
- One-parent rearing analyzed.
- Hand Feeding classified.
- Early Separation analyzed.
- Weaning defined without age constant.
- Separation vs Weaning separated.
- Market readiness separated from Weaning.
- Squab movement analyzed.
- Mortality concept carried forward.
- Replacement pathway analyzed.
- Foster attribution analyzed.
- RSK-007 and RSK-022 reviewed.
- Field Validation identified.
- No blocking contradiction with Phase 2 / 3A / 3B.

**Phase 3C is ready for user approval.**
