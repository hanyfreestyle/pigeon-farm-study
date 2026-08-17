# Risk Register

| Risk ID | Description | Probability | Impact | Mitigation | Related Phase | Status |
|---|---|---|---|---|---|---|
| RSK-001 | القفز مبكرًا إلى تصميم الجداول أو الـ Software Entities قبل فهم المجال. | High | High | تطبيق Domain-First Design Rule ومنع Data Modeling قبل اكتمال التحليل المعتمد. | Phases 1–7 | Active |
| RSK-002 | اختلاف ممارسات المزارع يؤدي إلى اعتبار ممارسة محلية Business Rule عامة. | High | High | تصنيف المعلومات إلى Verified Fact / Industry Practice / Assumption والتحقق من أكثر من سياق. | Phases 1–6 | Active |
| RSK-003 | الاعتماد على مصادر ضعيفة أو تجارية منفردة في معلومات Domain Knowledge مؤثرة. | Medium | High | تطبيق Research Evidence Policy وأولوية المصادر الأكاديمية/الرسمية/البيطرية. | Phases 1–6 | Active |
| RSK-004 | Scope Creep نحو أنواع تربية الحمام غير المرتبطة مباشرة بإنتاج الزغاليل التجاري. | Medium | Medium | استخدام Future Research Queue وعدم فتح موضوع خارج المرحلة الحالية دون قرار. | All Phases | Active |
| RSK-005 | تضارب المصطلحات أو استخدام نفس المصطلح بمعانٍ مختلفة بين المصادر والمزارع. | High | Medium | بناء Terminology Glossary تدريجيًا وتسجيل السياق والمصدر والتعارضات. | Phases 1–6 | Active |
| RSK-006 | بناء MVP قبل معرفة القرارات التشغيلية الحقيقية قد ينتج نظام تسجيل بيانات بدل أداة إدارة. | Medium | High | تأجيل MVP Definition حتى اكتمال Domain وSystem Analysis وربط الميزات بالقرارات والمخرجات. | Phases 6–8 | Active |
