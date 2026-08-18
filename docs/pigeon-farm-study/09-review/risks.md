# سجل المخاطر

| رقم الخطر | الوصف | الاحتمالية | التأثير | إجراءات التخفيف | المرحلة المرتبطة | آخر مراجعة | الحالة |
|---|---|---|---|---|---|---|---|
| RSK-001 | القفز مبكرًا إلى تصميم الجداول أو الكيانات البرمجية قبل فهم المجال. | Medium | High | تطبيق Domain-First والرجوع إلى `domain-to-system-boundaries.md`. | Phases 1–7 | Phase 3C التزمت بتحليل المجال دون تصميم تقني. | Active — Reduced |
| RSK-002 | اعتبار ممارسة مزرعة واحدة قاعدة عامة. | High | High | تصنيف الممارسة والسياق والدليل والتحقق الميداني. | Phases 1–6 | Early Separation/Foster/Hand Feeding بقيت Field Validation حيث يلزم. | Active |
| RSK-003 | الاعتماد على مصادر ضعيفة أو تجارية منفردة لإثبات معلومة مهمة. | Low-Medium | High | إعطاء الأولوية للمصادر المحكمة والرسمية وتسجيل القيود. | Phases 1–6 | Phase 3C أعادت استخدام مصادر محكمة ومصرية مع تحقق محدود. | Controlled — Monitor |
| RSK-004 | توسع النطاق نحو الهواية/السباق/الزينة أو موضوعات مراحل لاحقة. | Medium | Medium | استخدام Future Research Queue وحدود المراحل. | جميع المراحل | Phase 3C لم تتوسع إلى Feed/Health/Finance/Sales. | Active — Controlled |
| RSK-005 | تضارب المصطلحات أو استخدام المصطلح نفسه بمعان مختلفة. | Medium | High | قاموس مصطلحات موحد + مصطلحات ملتبسة. | Phases 1–6 | Phase 3C فصلت Squab/Bird Identity وSeparation/Weaning/Market Readiness. | Active — Reduced |
| RSK-006 | بناء MVP كأداة تسجيل فقط قبل فهم القرارات التشغيلية. | Medium | High | تأجيل MVP حتى اكتمال تحليل المجال والنظام. | Phases 6–8 | لم يبدأ تصميم MVP. | Active |
| RSK-007 | تمثيل دورة الإنتاج كدورة غير متداخلة. | Medium | Very High | استخدام Clutch/Egg/Squab/events ودعم أكثر من سياق متزامن للزوج. | Phases 1B–7 | Phase 3C ثبتت أن Squab stage لا تغلق إنتاج الزوج أمام Clutch تالية. | **Active — Materially Reduced** |
| RSK-008 | نقل ممارسات مكثفة/أجنبية إلى مصر باعتبارها الوضع القياسي. | High | High | الفصل بين Project Direction وMarket Fact والتحقق محليًا. | Phases 1–6 | نتائج Early Separation المصرية بقيت Study-specific وليست Standard. | Active |
| RSK-009 | استخدام قيمة مرجعية واحدة للعمر/الوزن/الدورة/الخصوبة دون سياق. | High | High | حفظ السياق وعدم تحويل Benchmark إلى Constant. | Phases 1–7 | Phase 3C طبقت ذلك على Growth/Weight/Weaning/Market Age. | **Active — Materially Reduced** |
| RSK-010 | تفسير انخفاض الصيف كتوقف تناسلي إلزامي. | Low-Medium | High | معاملة الحرارة والبيئة كعوامل مؤثرة والتحقق محليًا. | Phases 1 / 4 / 6 | لا تغيير. | Active — Reduced |
| RSK-011 | اعتبار رقم القفص/العش أو الحلقة أو Pair Code هوية دائمة للطائر أو الزوج. | Medium | High | فصل Bird/Pair/Location Identity عن External Identifier. | Phases 1B–2 / 7 | Phase 3C حافظت على Squab/Bird Identity مستقلة عن الموقع. | Active — Reduced |
| RSK-012 | فرض تسلسل مكاني جامد على جميع المزارع رغم أن بعض المستويات اختيارية. | Medium | High | اعتماد Hierarchy مرنة والتحقق الميداني. | Phase 2 / 7 | لا تغيير جوهري. | Active — Reduced; verify in Phase 7 design |
| RSK-013 | تحويل بيانات غير مؤكدة عن العمر أو الجنس أو السلالة أو النسب إلى حقائق مؤكدة. | High | High | فصل القيمة عن المصدر ودرجة الثقة ودعم Unknown/Estimated/Reported. | Phase 2B–7 | Phase 3C وسعت Provenance إلى Hatch Age/Weaning/Market Readiness. | Active — Reduced; address in Phase 6/7 |
| RSK-014 | مساواة Breed وStrain وLine أو إجبار كل طائر على سلالة نقية واحدة. | Medium-High | High | حفظ نوع التصنيف ومصدره/ثقته ودعم Crossbred/Mixed Lineage. | Phase 2B–7 | لا تغيير. | Active — Reduced; address in Phase 6/7 |
| RSK-015 | إعادة كتابة تاريخ الزوج عند تغيير الشريك أو إعادة استخدام Pair Code. | Medium | Very High | العلاقات التاريخية المستقلة وعدم إعادة كتابة الماضي. | Phase 2C–7 | لا تغيير جوهري في Phase 3C. | Active — Materially Reduced; enforce in Phase 6/7 |
| RSK-016 | اعتبار عدم ظهور قرابة في Pedigree ناقص دليلًا على عدم وجود Inbreeding. | Medium-High | High | حفظ Pedigree Confidence/Completeness وعدم تفسير مؤشرات دون بيانات كافية. | Phase 2C / 6–8 | لا تغيير. | Active; address in Phase 6/8 |
| RSK-017 | الخلط بين ترتيب البيضة داخل البطن (`Egg 1/Egg 2`) وهوية البيضة نفسها. | Medium | High | الفصل بين Egg Identity وEgg Sequence. | Phase 3A–7 | Phase 3C حافظت على الربط بالبيضة المحددة بعد الفقس. | **Active — Materially Reduced** |
| RSK-018 | نسبة البيض أو النتائج إلى البطن/السياق الإنتاجي الخطأ عند تداخل أكثر من Clutch للزوج نفسه. | Medium-High | Very High | استقلال Clutch context وربط كل فرد بسياقه. | Phase 3A–7 | Phase 3C حافظت على Squab→Clutch continuity. | **Active — Reduced** |
| RSK-019 | تغيير النسب الوراثي خطأً عند نقل البيضة أو الزغلول إلى Foster Pair. | Medium | Very High | تثبيت `Genetic Parentage ≠ Incubating/Rearing Caregiver` وحفظ التاريخ. | Phase 3A–7 | Phase 3C وسعت المبدأ إلى Fostered Squab/Caregiver History. | **Active — Materially Reduced** |
| RSK-020 | تحويل Expected Hatch إلى حقيقة أو اعتبار تجاوز الموعد المتوقع فشلًا مؤكدًا. | High | High | فصل Prediction عن Actual Observation. | Phase 3A–6 | لا تغيير جوهري في 3C. | **Active — Materially Reduced** |
| RSK-021 | استخدام Fertility أو Hatchability دون تعريف واضح للبسط والمقام. | High | High | كل Metric مستقبلية تحدد Numerator/Denominator/Inclusion Rules. | Phase 3B–6 | Carry Forward إلى 3D/6. | **Active** |
| RSK-022 | فقد الربط بين البيضة التي فقست والزغلول الناتج، مما يقطع التاريخ الوراثي والإنتاجي والرعائي. | Medium | Very High | تثبيت `Hatched Egg → Specific Squab → Same Bird Identity`. | Phase 3B–7 | Phase 3C أكدت Squab/Bird continuity. | **Active — Materially Reduced** |
| RSK-023 | تصنيف Hatch Failure أو سبب النفوق الجنيني بثقة زائفة. | High | High | فصل Outcome عن Cause وتطبيق Data Confidence. | Phase 3B–6 | Carry Forward إلى Phase 4/3D. | **Active** |
| RSK-024 | نسب نجاح/فشل الحضانة إلى Genetic Pair رغم تغير مقدم الحضانة. | Medium-High | Very High | حفظ Caregiver History وفصل Genetic/Incubation/Rearing attribution. | Phase 3B–7 | Phase 3C وسعت attribution إلى rearing stage. | **Active — Reduced** |
| **RSK-025** | **فقد هوية الزغلول أو إنشاء هوية ثانية عند الانتقال من Squab إلى Young Bird، بما يقطع Egg→Bird history.** | Medium | Very High | تثبيت أن Squab هو نفس Bird Identity في Life Stage مبكرة، وأن تغير المرحلة لا ينشئ فردًا جديدًا. | Phase 3C–7 | اكتشف ووثق في Phase 3C. | **Active — Reduced by Principle** |
| **RSK-026** | **الخلط بين الفصل الإداري والفطام الفسيولوجي والجاهزية للبيع، بما يسبب حالات تشغيلية ومقارنات مضللة.** | High | High | الفصل بين `Separation ≠ Physiological Weaning ≠ Market Readiness ≠ Sale Decision`. | Phase 3C–6 | اكتشف ووثق في Phase 3C. | **Active — Materially Reduced** |
| **RSK-027** | **تحويل عمر/وزن تسويق أو نمو من دراسة/سلالة/طريقة رعاية محددة إلى Constant عام.** | High | High | كل Growth/Market Benchmark يحمل Source/Breed/Rearing/Age Anchor/Context؛ Market validation في Phase 5. | Phase 3C–6 | اكتشف ووثق في Phase 3C. | **Active** |
| **RSK-028** | **نسب نمو/بقاء/Market Output بالكامل إلى Genetic Pair رغم Foster/Hand/Mixed rearing أو تغير مقدم الرعاية.** | Medium-High | Very High | فصل Genetic Production عن Hatch/Rearing/Market attribution وتعريف Metric قبل النسبة. | Phase 3C–7 | اكتشف ووثق في Phase 3C. | **Active — Reduced by Principle** |
| **RSK-029** | **استخدام وزن منفرد أو مقارنة عمر غير متكافئ للحكم على Slow Growth، أو تجاهل Hatch Asynchrony بين الأشقاء.** | High | High | استخدام repeated observations وعمر/هتش Anchor واضح وسياق Breed/Rearing؛ Thresholds إلى Phase 3D/6. | Phase 3C–6 | اكتشف ووثق في Phase 3C. | **Active** |

## خلاصة مراجعة المخاطر بعد Phase 3C

خفضت Phase 3C `RSK-022` بصورة ملموسة عبر تثبيت أن الزغلول هو نفس Bird Identity الناتجة عن البيضة المحددة. كما أبقت `RSK-007` منخفضًا عبر دعم تداخل رعاية الزغاليل مع Clutch لاحقة، ووسعت مبادئ Attribution من الحضانة إلى الرعاية بعد الفقس. ظهرت خمسة مخاطر جديدة تتعلق باستمرارية الهوية، والخلط بين Separation/Weaning/Market، وإساءة استخدام Growth Benchmarks، وإسناد الرعاية، وتفسير الوزن/النمو.

### Carry-forward

- `RSK-007` → Phase 3D/7.
- `RSK-009` → Phase 3D/5/6.
- `RSK-022` → Phase 7.
- `RSK-025` → Phase 7.
- `RSK-026` → Phase 3D/5/6/7.
- `RSK-027` → Phase 3D/5/6.
- `RSK-028` → Phase 3D/6/7.
- `RSK-029` → Phase 3D/6.

لا يوجد خطر جديد يحجب Phase 3D بعد مراجعة المستخدم.