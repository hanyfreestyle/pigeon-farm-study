# Risk Register

| Risk ID | Description | Probability | Impact | Mitigation | Related Phase | Status |
|---|---|---|---|---|---|---|
| RSK-001 | القفز مبكرًا إلى تصميم الجداول أو الـ Software Entities قبل فهم المجال. | High | High | تطبيق Domain-First Design Rule ومنع Data Modeling قبل اكتمال التحليل المعتمد. | Phases 1–7 | Active |
| RSK-002 | اختلاف ممارسات المزارع يؤدي إلى اعتبار ممارسة محلية Business Rule عامة. | High | High | تصنيف المعلومات إلى Verified Fact / Industry Practice / Assumption والتحقق من أكثر من سياق. | Phases 1–6 | Active |
| RSK-003 | الاعتماد على مصادر ضعيفة أو تجارية منفردة في معلومات Domain Knowledge مؤثرة. | Medium | High | تطبيق Research Evidence Policy وأولوية المصادر الأكاديمية/الرسمية/البيطرية. | Phases 1–6 | Active |
| RSK-004 | Scope Creep نحو أنواع تربية الحمام غير المرتبطة مباشرة بإنتاج الزغاليل التجاري. | Medium | Medium | استخدام Future Research Queue وعدم فتح موضوع خارج المرحلة الحالية دون قرار. | All Phases | Active |
| RSK-005 | تضارب المصطلحات أو استخدام نفس المصطلح بمعانٍ مختلفة بين المصادر والمزارع. | High | Medium | بناء Terminology Glossary تدريجيًا وتسجيل السياق والمصدر والتعارضات. | Phases 1–6 | Active |
| RSK-006 | بناء MVP قبل معرفة القرارات التشغيلية الحقيقية قد ينتج نظام تسجيل بيانات بدل أداة إدارة. | Medium | High | تأجيل MVP Definition حتى اكتمال Domain وSystem Analysis وربط الميزات بالقرارات والمخرجات. | Phases 6–8 | Active |
| RSK-007 | التعامل مع Production Cycle كدورة زمنية بسيطة غير متداخلة رغم أن الزوج قد يرعى زغاليل ويبدأ clutch جديدًا في الوقت نفسه. | High | High | دراسة lifecycle تفصيليًا في Phase 1B ثم تعريف حدود القياس في Phase 3 قبل أي Data Model. | Phases 1B–7 | Active |
| RSK-008 | نقل ممارسات intensive/industrial من الدراسات الصينية أو التجريبية إلى السوق المصري باعتبارها الوضع القياسي. | High | High | فصل Verified Biology عن Production Practice، وربط كل benchmark بظروفه، وإجراء Field Validation للمزارع المصرية المستهدفة. | Phases 1–6 | Active |
| RSK-009 | استخدام benchmark واحد للعمر أو الوزن أو طول الدورة أو الخصوبة دون مراعاة السلالة، نظام الإسكان، الفطام، البيئة وتعريف المؤشر. | High | High | حفظ ranges والسياق وتعريف numerator/denominator والمؤثرات؛ منع hard-coded universal constants قبل التحليل. | Phases 1–7 | Active |
| RSK-010 | الخلط بين انخفاض إنتاج الصيف بسبب Heat Stress وبين توقف بيولوجي موسمي إلزامي، ما قد يؤدي إلى تفسير خاطئ للأداء. | Medium | High | اعتبار الحرارة/الإضاءة/الإدارة عوامل تفسيرية، وجمع baseline محلي والتحقق ميدانيًا حسب المسكن والمناخ. | Phases 1 / 4 / 6 | Active |
| RSK-011 | الاعتماد على رقم القفص أو العش كأنه هوية دائمة للطائر أو الزوج في النظم الجماعية. | Medium | High | دراسة identification practices فعليًا في Phase 1B/2 والتمييز بين individual, pair and location identification. | Phases 1B–2 / 7 | Active |
