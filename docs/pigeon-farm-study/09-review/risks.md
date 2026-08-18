# سجل المخاطر

| رقم الخطر | الوصف | الاحتمالية | التأثير | إجراءات التخفيف | المرحلة المرتبطة | آخر مراجعة | الحالة |
|---|---|---|---|---|---|---|---|
| RSK-001 | القفز مبكرًا إلى تصميم الجداول أو الكيانات البرمجية قبل فهم المجال. | Medium | High | تطبيق Domain-First والرجوع إلى `domain-to-system-boundaries.md`. | Phases 1–7 | Phase 3A التزمت بتحليل الأحداث والمعلومات دون تصميم تقني. | Active — Reduced |
| RSK-002 | اعتبار ممارسة مزرعة واحدة قاعدة عامة. | High | High | تصنيف الممارسة والسياق والدليل والتحقق الميداني. | Phases 1–6 | Candling/Artificial Incubation/Foster Transfer بقيت Field Validation حيث يلزم. | Active |
| RSK-003 | الاعتماد على مصادر ضعيفة أو تجارية منفردة لإثبات معلومة مهمة. | Low-Medium | High | إعطاء الأولوية للمصادر المحكمة والرسمية وتسجيل القيود. | Phases 1–6 | Phase 3A استخدمت أدلة محكمة ومصادر Phase 1/2 المعتمدة. | Controlled — Monitor |
| RSK-004 | توسع النطاق نحو الهواية/السباق/الزينة أو موضوعات مراحل لاحقة. | Medium | Medium | استخدام Future Research Queue وحدود المراحل. | جميع المراحل | لم تتوسع Phase 3A إلى الصحة/الماليات/الزغاليل التفصيلية. | Active — Controlled |
| RSK-005 | تضارب المصطلحات أو استخدام المصطلح نفسه بمعان مختلفة. | Medium | High | قاموس مصطلحات موحد + مصطلحات ملتبسة. | Phases 1–6 | Phase 3A فصلت Egg Identity/Sequence وNest/Clutch وPrediction/Observation. | Active — Reduced |
| RSK-006 | بناء MVP كأداة تسجيل فقط قبل فهم القرارات التشغيلية. | Medium | High | تأجيل MVP حتى اكتمال تحليل المجال والنظام. | Phases 6–8 | لم يبدأ تصميم MVP. | Active |
| RSK-007 | تمثيل دورة الإنتاج كدورة غير متداخلة. | Medium | Very High | استخدام Clutch/Egg/events ومراسي زمنية صريحة ودعم أكثر من سياق متزامن للزوج. | Phases 1B–7 | Phase 3A حللت Pair→Multiple Clutches وOverlapping Clutches صراحة. | **Active — Materially Reduced** |
| RSK-008 | نقل ممارسات مكثفة/أجنبية إلى مصر باعتبارها الوضع القياسي. | High | High | الفصل بين Project Direction وMarket Fact والتحقق محليًا. | Phases 1–6 | Artificial Incubation/Candling/Foster usage لم تعتبر Market Facts مصرية. | Active |
| RSK-009 | استخدام قيمة مرجعية واحدة للعمر/الوزن/الدورة/الخصوبة دون سياق. | High | High | حفظ السياق وعدم تحويل Benchmark إلى Constant. | Phases 1–7 | Phase 3A أكدت أن Clutch size/Egg interval/Incubation duration تحتاج سياق وAnchor. | **Active — Reduced** |
| RSK-010 | تفسير انخفاض الصيف كتوقف تناسلي إلزامي. | Low-Medium | High | معاملة الحرارة والبيئة كعوامل مؤثرة والتحقق محليًا. | Phases 1 / 4 / 6 | لا تغيير. | Active — Reduced |
| RSK-011 | اعتبار رقم القفص/العش أو الحلقة أو Pair Code هوية دائمة للطائر أو الزوج. | Medium | High | فصل Bird/Pair/Location Identity عن External Identifier. | Phases 1B–2 / 7 | Phase 3A حافظت على استقلال Egg/Nest/Pair identities. | Active — Reduced |
| RSK-012 | فرض تسلسل مكاني جامد على جميع المزارع رغم أن بعض المستويات اختيارية. | Medium | High | اعتماد Hierarchy مرنة والتحقق الميداني. | Phase 2 / 7 | لا تغيير جوهري في Phase 3A. | Active — Reduced; verify in Phase 7 design |
| RSK-013 | تحويل بيانات غير مؤكدة عن العمر أو الجنس أو السلالة أو النسب إلى حقائق مؤكدة. | High | High | فصل القيمة عن المصدر ودرجة الثقة ودعم Unknown/Estimated/Reported. | Phase 2B–7 | Phase 3A طبقت Provenance على Lay date/Parentage/Clutch association. | Active — Reduced; address in Phase 6/7 |
| RSK-014 | مساواة Breed وStrain وLine أو إجبار كل طائر على سلالة نقية واحدة. | Medium-High | High | حفظ نوع التصنيف ومصدره/ثقته ودعم Crossbred/Mixed Lineage. | Phase 2B–7 | لا تغيير. | Active — Reduced; address in Phase 6/7 |
| RSK-015 | إعادة كتابة تاريخ الزوج عند تغيير الشريك أو إعادة استخدام Pair Code. | Medium | Very High | العلاقات التاريخية المستقلة وعدم إعادة كتابة الماضي. | Phase 2C–7 | Phase 3A حافظت على Pair History عند وجود Clutch نشطة. | Active — Materially Reduced; enforce in Phase 6/7 |
| RSK-016 | اعتبار عدم ظهور قرابة في Pedigree ناقص دليلًا على عدم وجود Inbreeding. | Medium-High | High | حفظ Pedigree Confidence/Completeness وعدم تفسير مؤشرات دون بيانات كافية. | Phase 2C / 6–8 | لا تغيير جوهري في Phase 3A. | Active; address in Phase 6/8 |
| **RSK-017** | **الخلط بين ترتيب البيضة داخل البطن (`Egg 1/Egg 2`) وهوية البيضة نفسها، بما يسبب فقد التاريخ عند النقل أو التصحيح.** | Medium | High | الفصل بين Egg Identity وEgg Sequence وحفظ Provenance عند عدم اليقين. | Phase 3A–7 | اكتشف ووثق في Phase 3A. | **Active** |
| **RSK-018** | **نسبة البيض أو النتائج إلى البطن/السياق الإنتاجي الخطأ عند تداخل أكثر من Clutch للزوج نفسه.** | Medium-High | Very High | استقلال Clutch context وربط كل بيضة بسياقها بدل Cycle خطية واحدة. | Phase 3A–7 | اكتشف ووثق في Phase 3A. | **Active** |
| **RSK-019** | **تغيير النسب الوراثي خطأً عند نقل البيضة إلى Foster Pair أو Artificial Incubation.** | Medium | Very High | تثبيت `Genetic Parentage ≠ Incubating Caregiver` وحفظ Transfer history. | Phase 3A–7 | اكتشف ووثق في Phase 3A؛ DEC-018 أساس التخفيف. | **Active — Reduced by Principle** |
| **RSK-020** | **تحويل Expected Hatch إلى حقيقة أو اعتبار تجاوز الموعد المتوقع فشلًا مؤكدًا.** | High | High | فصل Prediction عن Actual Observation وفرض Anchor/Policy واضحة لاحقًا. | Phase 3A–6 | اكتشف ووثق في Phase 3A. | **Active** |

## خلاصة مراجعة المخاطر بعد Phase 3A

خفضت Phase 3A بصورة جوهرية `RSK-007` عبر التخلي عن الدورة الخطية لصالح Clutch/Egg/events، وخفضت `RSK-009` عبر تثبيت أن كل Benchmark يحتاج سياقًا ومرساة قياس. ظهرت أربعة مخاطر إنتاجية جديدة تتعلق بهوية البيضة، ونسبة البطن المتداخلة، وفصل النسب عن مقدم الحضانة، وتحويل التوقع إلى حقيقة.

### Carry-forward

- `RSK-017` → Phase 3B/3D ثم Phase 7.
- `RSK-018` → Phase 3D/6/7.
- `RSK-019` → Phase 3B/3C/7.
- `RSK-020` → Phase 3B/6.

لا يوجد خطر جديد يحجب استمرار Phase 3 بعد مراجعة المستخدم.
