# سجل المخاطر

| رقم الخطر | الوصف | الاحتمالية | التأثير | إجراءات التخفيف | المرحلة المرتبطة | آخر مراجعة | الحالة |
|---|---|---|---|---|---|---|---|
| RSK-001 | القفز مبكرًا إلى تصميم الجداول أو الكيانات البرمجية قبل فهم المجال. | Medium | High | تطبيق Domain-First والرجوع إلى `domain-to-system-boundaries.md`. | Phases 1–7 | Phase 3B التزمت بتحليل المجال دون تصميم تقني. | Active — Reduced |
| RSK-002 | اعتبار ممارسة مزرعة واحدة قاعدة عامة. | High | High | تصنيف الممارسة والسياق والدليل والتحقق الميداني. | Phases 1–6 | Candling/Artificial Incubation/Assisted Hatch/Foster بقيت Field Validation حيث يلزم. | Active |
| RSK-003 | الاعتماد على مصادر ضعيفة أو تجارية منفردة لإثبات معلومة مهمة. | Low-Medium | High | إعطاء الأولوية للمصادر المحكمة والرسمية وتسجيل القيود. | Phases 1–6 | Phase 3B استخدمت مصادر محكمة/بيطرية محدودة النطاق فقط. | Controlled — Monitor |
| RSK-004 | توسع النطاق نحو الهواية/السباق/الزينة أو موضوعات مراحل لاحقة. | Medium | Medium | استخدام Future Research Queue وحدود المراحل. | جميع المراحل | Phase 3B لم تتوسع إلى نمو الزغاليل أو الصحة أو الماليات. | Active — Controlled |
| RSK-005 | تضارب المصطلحات أو استخدام المصطلح نفسه بمعان مختلفة. | Medium | High | قاموس مصطلحات موحد + مصطلحات ملتبسة. | Phases 1–6 | Phase 3B فصلت Incubation behavior/responsibility، Candling observation/interpretation، Fertility/Hatchability، Hatch Failure/Cause. | Active — Reduced |
| RSK-006 | بناء MVP كأداة تسجيل فقط قبل فهم القرارات التشغيلية. | Medium | High | تأجيل MVP حتى اكتمال تحليل المجال والنظام. | Phases 6–8 | لم يبدأ تصميم MVP. | Active |
| RSK-007 | تمثيل دورة الإنتاج كدورة غير متداخلة. | Medium | Very High | استخدام Clutch/Egg/events ومراسي زمنية صريحة ودعم أكثر من سياق متزامن للزوج. | Phases 1B–7 | Phase 3B حافظت على Egg-level analysis داخل Clutches المتداخلة. | **Active — Materially Reduced** |
| RSK-008 | نقل ممارسات مكثفة/أجنبية إلى مصر باعتبارها الوضع القياسي. | High | High | الفصل بين Project Direction وMarket Fact والتحقق محليًا. | Phases 1–6 | Artificial Incubation/Candling/Assisted Hatch لم تعتبر Market Facts مصرية. | Active |
| RSK-009 | استخدام قيمة مرجعية واحدة للعمر/الوزن/الدورة/الخصوبة دون سياق. | High | High | حفظ السياق وعدم تحويل Benchmark إلى Constant. | Phases 1–7 | Phase 3B أكدت أن Incubation duration وCandling day وHatch timing وFertility/Hatchability تحتاج تعريف وسياق. | **Active — Materially Reduced** |
| RSK-010 | تفسير انخفاض الصيف كتوقف تناسلي إلزامي. | Low-Medium | High | معاملة الحرارة والبيئة كعوامل مؤثرة والتحقق محليًا. | Phases 1 / 4 / 6 | لا تغيير. | Active — Reduced |
| RSK-011 | اعتبار رقم القفص/العش أو الحلقة أو Pair Code هوية دائمة للطائر أو الزوج. | Medium | High | فصل Bird/Pair/Location Identity عن External Identifier. | Phases 1B–2 / 7 | Phase 3B حافظت على Egg identity مستقلة عن الموقع والحاضن. | Active — Reduced |
| RSK-012 | فرض تسلسل مكاني جامد على جميع المزارع رغم أن بعض المستويات اختيارية. | Medium | High | اعتماد Hierarchy مرنة والتحقق الميداني. | Phase 2 / 7 | لا تغيير جوهري. | Active — Reduced; verify in Phase 7 design |
| RSK-013 | تحويل بيانات غير مؤكدة عن العمر أو الجنس أو السلالة أو النسب إلى حقائق مؤكدة. | High | High | فصل القيمة عن المصدر ودرجة الثقة ودعم Unknown/Estimated/Reported. | Phase 2B–7 | Phase 3B وسعت Provenance إلى Fertility/Failure/Hatch-time observations. | Active — Reduced; address in Phase 6/7 |
| RSK-014 | مساواة Breed وStrain وLine أو إجبار كل طائر على سلالة نقية واحدة. | Medium-High | High | حفظ نوع التصنيف ومصدره/ثقته ودعم Crossbred/Mixed Lineage. | Phase 2B–7 | لا تغيير. | Active — Reduced; address in Phase 6/7 |
| RSK-015 | إعادة كتابة تاريخ الزوج عند تغيير الشريك أو إعادة استخدام Pair Code. | Medium | Very High | العلاقات التاريخية المستقلة وعدم إعادة كتابة الماضي. | Phase 2C–7 | لا تغيير جوهري في Phase 3B. | Active — Materially Reduced; enforce in Phase 6/7 |
| RSK-016 | اعتبار عدم ظهور قرابة في Pedigree ناقص دليلًا على عدم وجود Inbreeding. | Medium-High | High | حفظ Pedigree Confidence/Completeness وعدم تفسير مؤشرات دون بيانات كافية. | Phase 2C / 6–8 | لا تغيير. | Active; address in Phase 6/8 |
| RSK-017 | الخلط بين ترتيب البيضة داخل البطن (`Egg 1/Egg 2`) وهوية البيضة نفسها، بما يسبب فقد التاريخ عند النقل أو التصحيح. | Medium | High | الفصل بين Egg Identity وEgg Sequence وحفظ Provenance عند عدم اليقين. | Phase 3A–7 | Phase 3B نسبت Candling/Hatch/Failure لكل Egg محددة. | **Active — Materially Reduced** |
| RSK-018 | نسبة البيض أو النتائج إلى البطن/السياق الإنتاجي الخطأ عند تداخل أكثر من Clutch للزوج نفسه. | Medium-High | Very High | استقلال Clutch context وربط كل بيضة بسياقها بدل Cycle خطية واحدة. | Phase 3A–7 | Phase 3B ثبتت `Egg Outcome ≠ Clutch Outcome`. | **Active — Reduced** |
| RSK-019 | تغيير النسب الوراثي خطأً عند نقل البيضة إلى Foster Pair أو Artificial Incubation. | Medium | Very High | تثبيت `Genetic Parentage ≠ Incubating Caregiver` وحفظ Transfer/Caregiver history. | Phase 3A–7 | Phase 3B دعمت تغير مقدم الحضانة على مستوى Egg مع ثبات Genetic Parentage. | **Active — Materially Reduced** |
| RSK-020 | تحويل Expected Hatch إلى حقيقة أو اعتبار تجاوز الموعد المتوقع فشلًا مؤكدًا. | High | High | فصل Prediction عن Actual Observation واعتماد Configurable Domain Policy مع إمكانية Prediction Revision. | Phase 3A–6 | Phase 3B حسمت CON-006 كسياسة قابلة للتحديد، وثبتت Late Hatch ≠ Failure. | **Active — Materially Reduced** |
| **RSK-021** | **استخدام Fertility أو Hatchability دون تعريف واضح للبسط والمقام، بما يجعل المقارنات مضللة.** | High | High | كل Metric مستقبلية يجب أن تحدد Numerator/Denominator/Inclusion Rules/Observation Method. | Phase 3B–6 | اكتشف ووثق في Phase 3B. | **Active** |
| **RSK-022** | **فقد الربط بين البيضة التي فقست والزغلول الناتج، مما يقطع التاريخ الوراثي والإنتاجي والرعائي.** | Medium | Very High | تثبيت `Hatched Egg → Specific Squab` كاستمرارية Domain وحفظ Egg/Parentage/Caregiver context. | Phase 3B–7 | اكتشف ووثق في Phase 3B. | **Active — Reduced by Principle** |
| **RSK-023** | **تصنيف Hatch Failure أو سبب النفوق الجنيني بثقة زائفة دون دليل كافٍ أو خلط Infertility مع Embryonic Death/Dead-in-shell.** | High | High | فصل Outcome عن Cause وتطبيق Data Confidence/Provenance ودعم Unknown Cause. | Phase 3B–6 | اكتشف ووثق في Phase 3B. | **Active** |
| **RSK-024** | **نسب نجاح/فشل الحضانة إلى Genetic Pair رغم تغير مقدم الحضانة، أو فقد تاريخ انتقال المسؤولية بين Genetic/Foster/Artificial caregivers.** | Medium-High | Very High | حفظ Caregiver History لكل Egg وفصل Genetic production عن Incubation responsibility وHatch result. | Phase 3B–7 | اكتشف ووثق في Phase 3B. | **Active — Reduced by Principle** |

## خلاصة مراجعة المخاطر بعد Phase 3B

خفضت Phase 3B `RSK-017 → RSK-020` بصورة ملموسة عبر تحليل البيضة كوحدة النتائج والملاحظات، واعتماد `CON-006` كـConfigurable Domain Policy، وفصل Genetic Parentage عن Caregiver History، وفصل Prediction عن Observation. كما ظهرت أربعة مخاطر جديدة تتعلق بتعريف Metrics، واستمرارية Egg→Squab، وتصنيف الفشل، ونسب الحضانة للطرف الصحيح.

### Carry-forward

- `RSK-017` → Phase 3D/7.
- `RSK-018` → Phase 3D/6/7.
- `RSK-019` → Phase 3C/7.
- `RSK-020` → Phase 3D/6.
- `RSK-021` → Phase 3D/6.
- `RSK-022` → Phase 3C/7.
- `RSK-023` → Phase 3D/4/6.
- `RSK-024` → Phase 3D/6/7.

لا يوجد خطر جديد يحجب الانتقال إلى Phase 3C بعد مراجعة المستخدم.
