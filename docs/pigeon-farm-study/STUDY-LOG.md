# Pigeon Farm Management System — Study Log

> سجل مختصر زمني لما تم تنفيذه في كل مرحلة/مهمة. يضاف Entry جديد بعد كل مهمة رئيسية مع النطاق، الملفات، النتائج، الأسئلة، المخاطر، والحالة التالية.

## LOG-001 — Phase 1A: Commercial Pigeon Farming Domain Research

- **Date:** 2026-08-17
- **Phase:** Phase 1A
- **Status:** Completed — Awaiting Review
- **Scope:** Commercial Meat Pigeon / Squab Production Domain Research

### Work Completed
- دراسة مفهوم الإنتاج التجاري للزغاليل والفرق عن تربية الهواية.
- دراسة نماذج الإسكان والإنتاج المستخدمة فعليًا في المصادر.
- تحليل تركيب القطيع ومسارات الطيور تشغيليًا بدون تحويلها إلى Software Statuses.
- دراسة الزوج كـ operational breeding unit وPair Bond.
- دراسة Nest Management وDouble Nest System.
- التحقق من Overlapping Production Cycles.
- دراسة العمليات اليومية والدورية وEvent-driven operations.
- مراجعة Record Keeping وIdentification Methods.
- دراسة Replacement & Culling.
- دراسة أثر الحرارة والموسمية والبيئة.
- مراجعة مؤشرات الأداء الإنتاجي بدون تحويلها إلى System KPIs.
- إضافة سياق مصري من أبحاث ودراسات محلية.

### Evidence Summary
- **Tracked Sources:** 15
- المصادر تضمنت أبحاثًا محكمة ومصادر جامعية/رسمية ومراجع دولية مع أدلة مصرية.

### Key Findings
1. الزوج المنتج وحدة تشغيلية أساسية.
2. الزغلول يعتمد على الأبوين وCrop Milk في بداية العمر.
3. Clutch غالبًا صغير والحضانة تقارب 18–20 يومًا حسب السياق.
4. عمر التسويق/الفطام الشائع حول 3–4 أسابيع لكنه ليس ثابتًا عالميًا.
5. دورات الإنتاج قد تتداخل لنفس الزوج.
6. Double Nest له وظيفة تشغيلية مهمة.
7. Production Cycle لا تُعرّف كفترة خطية غير متداخلة دون سياق.
8. توجد نظم loft/dovecote/colony وindividual pair cages.
9. توجد أدلة مصرية على mud dovecotes وwooden lofts وindividual cages.
10. Heat Stress قد يخفض الأداء صيفًا دون إثبات توقف بيولوجي موسمي مطلق.

### Open Questions
- تمت إضافة `OQ-014` إلى `OQ-021` للتحقق الميداني.

### Assumptions
- **New assumptions:** 0

### Risks
- تمت إضافة `RSK-007` إلى `RSK-011`.

### Master Status
- Phase 0: Completed
- Phase 1: In Progress
- Phase 1A: Completed — Awaiting Review
- Phase 1B: Pending
- Phase 1C: Pending

### Next Step
**Phase 1B — Detailed Pigeon Production Lifecycle**

---

## LOG-002 — Phase 1B: Detailed Pigeon Production Lifecycle

- **Date:** 2026-08-17
- **Phase:** Phase 1B
- **Status:** Completed — Awaiting Review
- **Scope:** Detailed real-world pigeon reproductive and squab production lifecycle.

### Work Completed
- تحليل Entry into Breeding Population والفرق بين Sexual Maturity وOperational Breeding Readiness.
- تحليل Pair Formation، Pair Stability، Courtship، Mating وRe-pairing.
- تحليل Nest Preparation وNest Ownership وDouble Nest.
- فصل أحداث Egg 1 / Egg 2 / Clutch Completion / Incubation Start.
- وضع Domain Definition واضحة لـ Clutch دون تحويلها إلى Software Model.
- تحليل incubation duration/shifts والاختلاف في anchor المستخدم للعد.
- دراسة Candling/Fertility Checking وموقعها الزمني التقريبي.
- تحديد egg outcomes وحالات hatch failure وdead-in-shell.
- تحليل Squab early life، Crop Milk، النمو الأسبوعي، weaning وmarket readiness.
- دراسة Parent–Squab dependency وfostering ومشكلة فقد أحد الأبوين.
- تحليل Next Clutch وOverlapping Production Cycles بعمق.
- دراسة failed-cycle scenarios وإعادة بدء الإنتاج بعد الفشل.
- توضيح تعدد التعريفات الممكنة لـ Production/Reproductive Cycle.
- تحليل continuous farm production عبر أزواج غير متزامنة.
- مراجعة reproductive interruptions وmolt.
- إنشاء Reference Production Timeline وReal-world Observable Events وExceptions.
- مقارنة timeline المصري بالأدلة الدولية.

### Sources Used
- أعيد استخدام مصادر Phase 1A ذات الصلة `SRC-001` إلى `SRC-015`.
- تمت إضافة/توسيع مصادر `SRC-016` إلى `SRC-021`.
- المصادر الجديدة شملت Poultry Science 2026، Genetics review، Computers and Electronics in Agriculture، Journal of Avian Biology، وأبحاث crop milk.

### Key Lifecycle Findings
1. Sexual maturity ليست مساوية تلقائيًا للجاهزية التجارية للتكاثر.
2. Egg laid وClutch complete وIncubation started أحداث مختلفة.
3. داخل الـ clutch، الفاصل بين البيضتين يقارب يومين في الأدلة القوية.
4. الحضانة الطبيعية غالبًا نحو 17–20 يومًا، لكن anchor العد قد يختلف.
5. Candling ممكن عمليًا قرب days 5–7 حيث يُستخدم.
6. Weaning وMarket Readiness وEarly Separation ليست مفاهيم متطابقة.
7. Squab growth سريع جدًا خصوصًا في أول أسبوعين ويتأثر بالسلالة.
8. Hatch-to-next-lay يختلف بشدة بين السلالات والإدارة.
9. نفس الزوج قد يرعى Cycle A ويبدأ/يحضن Cycle B بالتزامن.
10. فشل الـ clutch قد يؤدي إلى restart أسرع من دورة ناجحة كاملة.
11. “Production Cycle” لها أكثر من تعريف صالح حسب غرض القياس.
12. Molt عامل إنتاجي/فسيولوجي لكنه ليس توقفًا إلزاميًا كاملًا للتكاثر.

### Egyptian Context
- البيانات المصرية تدعم incubation قريبًا من 18 يومًا.
- White Mirthys وZagel وLocal Egyptian تختلف بوضوح في نمو 28 يومًا.
- hatch-to-next-lay كان أقصر بوضوح في White Mirthys من Local/Zagel في الدراسة المستخدمة.
- early separation في مزرعة تجارية مصرية غيّر توقيت العودة لوضع البيض ونتائج الزغاليل.
- لا توجد حتى الآن مواصفة سوق مصرية موحدة مثبتة لعمر/وزن الزغلول.

### Evidence Conflicts
- تم توسيع `consistency-review.md` من 4 إلى 9 بنود اختلاف/سياق.
- أهمها: maturity vs readiness، incubation anchor، weaning vs market age، next-lay interval، molt vs reproduction.

### Terminology
- تم توسيع القاموس حتى `TERM-030` وإضافة مفاهيم مثل Sexual Maturity، Operational Breeding Readiness، Oviposition Interval، Candling، Embryonic Death، Dead-in-shell، Fostering، Market Readiness، Weaning، Reproductive Cycle.

### Open Questions
- **New IDs added:** 0.
- الأسئلة الميدانية الحالية `OQ-014` إلى `OQ-021` ما زالت تغطي أهم فجوات Phase 1B؛ تم تفصيل نقاط التحقق داخل `production-lifecycle.md` بدل إنشاء IDs مكررة.

### Assumptions
- **New assumptions:** 0.
- لم يتم ملء أي فجوة بافتراض غير موثق.

### Risks
- **New risk IDs added:** 0.
- المخاطر الحالية `RSK-007` إلى `RSK-011` تغطي أخطر نتائج الـ lifecycle، خصوصًا overlap والbenchmarks والهوية والسياق المصري.

### Files Updated
- `01-domain-research/production-lifecycle.md`
- `01-domain-research/terminology.md`
- `09-review/consistency-review.md`
- `MASTER.md`
- `STUDY-LOG.md`

### Files Reviewed but Not Changed
- `09-review/open-questions.md`
- `09-review/assumptions.md`
- `09-review/risks.md`

### Master Status
- Phase 0: Completed
- Phase 1: In Progress
- Phase 1A: Completed — Awaiting Review
- Phase 1B: Completed — Awaiting Review
- Phase 1C: Pending

### Technical Boundary
لم يتم إنشاء Database Design أو ERD أو Models أو Migrations أو Software Status Enums أو APIs أو UI أو Filament Resources أو Architecture أو Code.

### Next Step
**Phase 1C — Domain Terminology, Evidence Consolidation & Validation Review**

### Stop Condition
Phase 1C لم تبدأ. العمل متوقف عند نهاية Phase 1B لحين المراجعة وتعليمات مستقلة.
