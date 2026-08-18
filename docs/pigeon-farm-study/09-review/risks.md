# سجل المخاطر

| رقم الخطر | الوصف | الاحتمالية | التأثير | إجراءات التخفيف | المرحلة المرتبطة | آخر مراجعة | الحالة |
|---|---|---|---|---|---|---|---|
| RSK-001 | القفز مبكرًا إلى تصميم الجداول أو الكيانات البرمجية قبل فهم المجال. | Medium | High | تطبيق Domain-First والرجوع إلى `domain-to-system-boundaries.md`. | Phases 1–7 | Phase 2D التزمت بالتجميع دون تصميم تقني. | Active — Reduced |
| RSK-002 | اعتبار ممارسة مزرعة واحدة قاعدة عامة. | High | High | تصنيف الممارسة والسياق والدليل والتحقق الميداني. | Phases 1–6 | Phase 2D جمعت Field Validation دون تحويله إلى Facts. | Active |
| RSK-003 | الاعتماد على مصادر ضعيفة أو تجارية منفردة لإثبات معلومة مهمة. | Low-Medium | High | إعطاء الأولوية للمصادر المحكمة والرسمية وتسجيل القيود. | Phases 1–6 | لا بحث جديد في Phase 2D؛ تم الاعتماد على الأدلة السابقة فقط. | Controlled — Monitor |
| RSK-004 | توسع النطاق نحو الهواية/السباق/الزينة أو موضوعات مراحل لاحقة. | Medium | Medium | استخدام Future Research Queue وحدود المراحل. | جميع المراحل | Phase 2D استخدمت Fancy/Foster فقط لاختبار اتساق المجال. | Active — Controlled |
| RSK-005 | تضارب المصطلحات أو استخدام المصطلح نفسه بمعان مختلفة. | Medium | High | قاموس مصطلحات موحد + مصطلحات ملتبسة. | Phases 1–6 | تمت مراجعة TERM-040 → TERM-091 دون تكرار حابس. | Active — Reduced |
| RSK-006 | بناء MVP كأداة تسجيل فقط قبل فهم القرارات التشغيلية. | Medium | High | تأجيل MVP حتى اكتمال تحليل المجال والنظام. | Phases 6–8 | لم يبدأ تصميم MVP. | Active |
| RSK-007 | تمثيل دورة الإنتاج كدورة غير متداخلة. | Medium | Very High | استخدام الأحداث الفعلية ومراسي قياس صريحة في Phase 3. | Phases 1B–7 | Phase 2 Baseline تحمل Pair→Multiple Clutches وOverlapping Cycles صراحة إلى Phase 3. | Active — Reduced |
| RSK-008 | نقل ممارسات مكثفة/أجنبية إلى مصر باعتبارها الوضع القياسي. | High | High | الفصل بين Project Direction وMarket Fact والتحقق محليًا. | Phases 1–6 | Field Validation المصرية بقيت منفصلة عن اتجاه المشروع. | Active |
| RSK-009 | استخدام قيمة مرجعية واحدة للعمر/الوزن/الدورة/الخصوبة دون سياق. | High | High | حفظ السياق وعدم تحويل Benchmark إلى Constant. | Phases 1–7 | Phase 2D لم تضف Thresholds أو مدد عالمية. | Active — Reduced |
| RSK-010 | تفسير انخفاض الصيف كتوقف تناسلي إلزامي. | Low-Medium | High | معاملة الحرارة والبيئة كعوامل مؤثرة والتحقق محليًا. | Phases 1 / 4 / 6 | لا تغيير. | Active — Reduced |
| RSK-011 | اعتبار رقم القفص/العش أو الحلقة أو Pair Code هوية دائمة للطائر أو الزوج. | Medium | High | فصل Bird/Pair/Location Identity عن External Identifier. | Phases 1B–2 / 7 | Phase 2 Baseline ثبتت `Bird Identity ≠ Ring` و`Pair Code ≠ Pair Identity`. | Active — Reduced |
| RSK-012 | فرض تسلسل مكاني جامد على جميع المزارع رغم أن بعض المستويات اختيارية. | Medium | High | اعتماد Hierarchy مرنة والتحقق الميداني. | Phase 2 / 7 | Phase 2D ثبتت أن Farm Site وSection وCage Group مستويات اختيارية. | Active — Reduced; verify in Phase 7 design |
| RSK-013 | تحويل بيانات غير مؤكدة عن العمر أو الجنس أو السلالة أو النسب إلى حقائق مؤكدة، خاصة عند شراء طيور بالغة. | High | High | فصل القيمة عن مصدرها ودرجة الثقة، والسماح بـ Unknown/Estimated/Reported. | Phase 2B–7 | Phase 2D اعتمدت Data Confidence / Provenance وUnknown Data Strategy في baseline. | Active — Reduced; address in Phase 6/7 |
| RSK-014 | مساواة Breed وStrain وLine أو إجبار كل طائر على سلالة نقية واحدة. | Medium-High | High | حفظ نوع التصنيف ومصدره/ثقته ودعم Crossbred/Mixed Lineage. | Phase 2B–7 | Phase 2D ثبتت `Breed ≠ Strain ≠ Line` وراجعت المصطلحات. | Active — Reduced; address in Phase 6/7 |
| RSK-015 | إعادة كتابة تاريخ الزوج عند تغيير أحد الشريكين أو إعادة استخدام نفس Pair Code، بما يؤدي إلى نسب إنتاج قديم إلى علاقة جديدة. | Medium | Very High | اعتبار كل علاقة شريكين خلال فترة تاريخية مستقلة، وإنهاء العلاقة القديمة قبل Re-pairing، وعدم مساواة Pair Code بالهوية. | Phase 2C–7 | Phase 2D حسمت أن Same Pair Reunited بعد نهاية فعلية = Operational Episode جديدة، مع استمرار العلاقة نفسها فقط عند Temporary Separation غير المنهي. | Active — Materially Reduced; enforce in Phase 6/7 |
| RSK-016 | اعتبار عدم ظهور قرابة في Pedigree ناقص دليلًا على عدم وجود Inbreeding، أو تفسير Inbreeding Coefficient دون مراعاة عمق/اكتمال النسب. | Medium-High | High | حفظ Pedigree Confidence/Completeness، والتفريق بين No Known Relationship وProven Unrelated، وعدم حساب/تفسير مؤشرات قرابة دون بيانات كافية. | Phase 2C / 6–8 | Phase 2D ثبتت القاعدة في Baseline؛ الخطر يبقى جوهريًا لأن جودته تعتمد على البيانات المتاحة. | Active; address in Phase 6/8 |

## خلاصة مراجعة المخاطر بعد Phase 2D

خفضت Phase 2 خطرين بنيويين مهمين: **Rigid Hierarchy Risk** و**Pair History Rewrite Risk** عبر اعتماد Hierarchy مرنة وحفظ Episode تاريخية مستقلة للزوج. كما خُفضت مخاطر Data Certainty وBreed Classification بوضع قواعد واضحة للـProvenance والبيانات المجهولة والتصنيفات المختلطة.

يبقى `RSK-016` أكثر اعتمادًا على جودة البيانات؛ لا يمكن إلغاؤه بالتوثيق وحده لأن أي Kinship/Inbreeding Analysis مستقبلي يتأثر مباشرة بعمق واكتمال Pedigree.

### Carry-forward للمخاطر الجديدة في Phase 2

- `RSK-012` → Phase 7: منع تحويل الهيكل المرن إلى Hierarchy تقنية جامدة.
- `RSK-013` → Phase 6/7: إظهار الثقة والمصدر وعدم اختلاق قيم.
- `RSK-014` → Phase 6/7: الحفاظ على مرونة Breed/Strain/Line/Crossbred.
- `RSK-015` → Phase 6/7: قواعد التاريخ ونسب الأداء للزوج الصحيح.
- `RSK-016` → Phase 6/8: تحذيرات القرابة وتفسير التحليل بحسب اكتمال النسب.
