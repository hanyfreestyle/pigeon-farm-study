# إدارة النسب — تحليل المجال (Pedigree Management Domain Analysis)

> **المرحلة:** Phase 2C — تحليل إدارة الأزواج والنسب  
> **الحالة:** Completed — Awaiting Review  
> **التاريخ:** 2026-08-18  
> **النطاق:** فهم النسب الوراثي، اكتماله وثقته وتصحيحه، القرابة وزواج الأقارب واستراتيجيات التربية على مستوى المجال، دون Genetics Model أو خوارزمية أو قاعدة بيانات.  
> **مرجع الحدود:** `09-review/domain-to-system-boundaries.md`.

---

## 1. الملخص التنفيذي

النسب (Pedigree) هو **علاقة وراثية تاريخية** تربط الطائر بأبيه وأمه الوراثيين عندما تكون المعلومة معروفة، ويمكن أن تمتد عبر أجيال متعددة. ولا يتغير النسب بسبب انتقال الطائر أو تغيير زوجه أو Foster/Rearing workflows.

طبقًا لـ `DEC-011` لا يتم فرض عمق ثابت لشجرة النسب. وقد يكون لدى طائر صفر أجيال معروفة، أو أحد الأبوين فقط، أو عدة أجيال موثقة. لذلك:

**Unknown / Partial Pedigree ≠ Invalid Bird Record**

كما يجب الفصل بين:

**Pedigree = Genetic Relationship**

و:

**Pair History = Operational Breeding Relationship**

فالطائر قد يمر بعدة أزواج عبر حياته، لكن أبوه وأمه الوراثيان لا يتغيران.

---

## 2. الأب والأم الوراثيان

### Genetic Father
الأب الوراثي الذي ساهم في تكوين البيضة وراثيًا.

### Genetic Mother
الأم الوراثية التي وضعت البيضة وساهمت وراثيًا في النسل.

قد تكون المعلومة:

- Known؛
- Documented؛
- Claimed؛
- Breeder-reported؛
- Seller-reported؛
- Inferred؛
- Unknown.

لا يجوز مساواة القيمة بمستوى الثقة فيها.

---

## 3. النسب الوراثي مقابل الحضانة والتربية

قاعدة Phase 1/2 الحاكمة:

**Genetic Parentage ≠ Incubating Caregiver ≠ Rearing Caregiver**

إذا نقلت البيضة إلى Foster Pair، يبقى الأب والأم الوراثيان كما هما.

إذا فقست البيضة تحت زوج آخر أو Artificial Incubation، لا يتغير Genetic Parentage.

إذا ربى الزغلول زوج آخر أو أحد الأبوين أو تمت Hand Feeding، لا يتغير Genetic Parentage.

---

## 4. Pedigree كعلاقة مفتوحة العمق

طبقًا لـ `DEC-011`:

لا يوجد حد ثابت مثل جيلين أو ثلاثة أجيال.

قد تتوافر بيانات:

- 0 generation known؛
- 1 generation؛
- 3 generations؛
- 10 generations؛
- أو أكثر.

العمق الفعلي يعتمد على جودة وتاريخ السجلات.

---

## 5. النسب الجزئي (Partial Pedigree)

حالات صحيحة في المجال:

- Known Father + Unknown Mother؛
- Unknown Father + Known Mother؛
- Both Unknown؛
- Claimed Parents؛
- Imported Pedigree؛
- Seller-reported Pedigree؛
- Pedigree معروف لجزء من الأجيال فقط.

لا يجوز ملء النقص بافتراضات.

---

## 6. درجة ثقة النسب (Pedigree Confidence)

يطبق مبدأ Data Confidence / Provenance من Phase 2B.

أمثلة مفاهيمية:

- Verified Parentage؛
- Documented Parentage؛
- Breeder Record؛
- Seller Reported؛
- Imported Certificate؛
- Inferred؛
- Unknown.

هذه ليست Software Enums نهائية.

### لماذا الثقة مهمة؟

لأن أي تحليل لاحق مثل:

- اكتشاف قرابة؛
- تقييم Lineage؛
- حساب Inbreeding Coefficient؛
- Crossbreeding analysis؛

يعتمد على جودة النسب الأصلي.

---

## 7. تصحيح النسب

قد يكتشف لاحقًا أن الأب أو الأم المسجلين خطأ نتيجة:

- خطأ تسجيل؛
- خلط في التعريف؛
- شهادة/سجل جديد؛
- تحقق جيني؛
- تصحيح من المربي.

المجال يحتاج الحفاظ على معرفة:

- القيمة السابقة؛
- القيمة الجديدة؛
- سبب التغيير؛
- مصدر التصحيح؛
- تاريخ التصحيح.

هذه Information / History Requirements وليست Audit Architecture.

---

## 8. Pedigree مقابل Pair History

مثال:

```text
Bird A
Genetic Father = Bird F
Genetic Mother = Bird M

ثم خلال حياته:
Pair P1 مع Bird X
Pair P2 مع Bird Y
Pair P3 مع Bird Z
```

الأزواج الثلاثة لا تغير الأب أو الأم الوراثيين.

إذن:

**Pedigree ≠ Pair History**.

---

## 9. Foster Pair مقابل Genetic Pair

Foster Pair لا يصبح Genetic Parent بمجرد:

- حضانة البيضة؛
- فقسها تحت الزوج؛
- تربية الزغلول؛
- التغذية الأبوية البديلة.

يجب الحفاظ على الفصل التاريخي بين:

- من أنجب وراثيًا؛
- من حضن؛
- من ربى.

---

## 10. Crossbreeding

بناءً على Phase 2B:

إذا كان:

```text
Male Breed/Line A × Female Breed/Line B
```

فقد يكون الأبناء:

- Crossbred؛
- Mixed Lineage؛
- أو مصنفين وفق سياسة تربية محددة.

Phase 2C لا تضع Naming Rules ولا Genetics Model.

المهم ألا يجبر المجال الابن على Pure Breed واحدة عندما يدل النسب على أصول مختلطة.

---

## 11. القرابة وزواج الأقارب (Inbreeding)

زواج الأقارب يعني تزاوج أفراد يشتركون في أسلاف مشتركة بدرجات مختلفة. في إدارة التربية الحيوانية، القرب الوراثي قد يرفع احتمال اجتماع نسخ متماثلة موروثة من أصل مشترك، وقد يرتبط بتراجع بعض صفات اللياقة عند الزيادة المستمرة [SRC-032, SRC-033].

### علاقات يجب أن يستطيع التحليل المستقبلي اكتشافها عند توفر النسب

- Parent × Offspring؛
- Full Sibling × Full Sibling؛
- Half-sibling × Half-sibling؛
- أفراد يشتركون في أجداد أو أسلاف مشتركة؛
- تكرار نفس الأسلاف عبر أكثر من فرع.

لا تحدد Phase 2C سياسة منع أو سماح للتزاوج.

---

## 12. Known Close Relationship مقابل Unknown Pedigree Risk

قاعدة مهمة:

**No Known Relationship ≠ Proven Unrelated**

إذا كان Pedigree ناقصًا، فإن عدم ظهور قريب مشترك لا يثبت عدم وجود قرابة.

لذلك يجب التمييز بين:

- قرابة معروفة ومثبتة؛
- لا توجد قرابة ظاهرة ضمن السجل المتاح؛
- بيانات غير كافية للحكم.

هذه النقطة أساسية لتجنب ثقة زائفة في تحليلات Genetics مستقبلًا.

---

## 13. معامل زواج الأقارب (Inbreeding Coefficient)

معامل زواج الأقارب `F` مفهوم علمي مناسب كميزة تحليلية مستقبلية، ويصف احتمال التطابق الوراثي الناتج عن أصل مشترك وفق التعريفات التقليدية المعتمدة على Pedigree. كما أن معامل القرابة بين فردين يرتبط بالتوقع الوراثي لنسلهما [SRC-032].

### ما يحتاجه مستقبلًا

- Pedigree متعدد الأجيال؛
- هوية صحيحة للأسلاف؛
- روابط أبوية موثوقة؛
- عمق واكتمال معروفان للشجرة؛
- سياسة واضحة للتعامل مع founders/unknown parents.

### فائدته

- مقارنة مستوى القرابة داخل خطة تزاوج؛
- دعم تجنب التزاوجات عالية القرابة إذا كانت سياسة المزرعة تتطلب ذلك؛
- مراقبة التنوع الوراثي في برامج التربية؛
- دعم Breeding Strategy.

### حدوده

- يتأثر بقوة بعمق واكتمال Pedigree؛
- المقارنة بين مجموعات ذات عمق نسب مختلف قد تكون مضللة؛
- Unknown Parents تقلل قوة الاستنتاج؛
- يمكن للبيانات الجينومية أن تقدم تقديرات مختلفة عن Pedigree-based measures، لكنها خارج نطاق المشروع الحالي.

Phase 2C لا تنفذ Formula أو Algorithm.

Carry Forward إلى Phase 6/8.

---

## 14. استراتيجيات التربية (Breeding Strategy)

عالي المستوى فقط، قد تستخدم المزارع أو برامج التربية مفاهيم مثل:

- Linebreeding؛
- Outcrossing؛
- Crossbreeding؛
- Maintaining Pure Line؛
- Performance Mating؛
- Genetic Diversity Management.

هذه استراتيجيات إدارة وانتخاب ولا تعني أن واحدة منها قاعدة موحدة للمشروع.

### Linebreeding
استخدام قرابة محسوبة نسبيًا للحفاظ على صفات/أصل محدد، مع خطر زيادة Inbreeding إذا أسيء استخدامها.

### Outcrossing
اختيار طيور أقل قرابة أو من خطوط مختلفة لزيادة التنوع أو دمج صفات.

### Crossbreeding
استخدام طيور من سلالات/خطوط مختلفة لأهداف محددة.

### Performance Mating
اختيار الشركاء بناءً على أداء أو نتائج تاريخية، لا على الاسم الوراثي وحده.

مدى استخدام هذه المصطلحات فعليًا في المزارع المصرية يحتاج Field Validation.

---

## 15. النسب والأداء

النسب يصف **العلاقة الوراثية** ولا يضمن الأداء.

لا يجوز استنتاج:

- Fertility؛
- Hatchability؛
- Growth؛
- Parenting؛
- Market Weight؛

من Pedigree وحده دون بيانات أداء فعلية.

وبالعكس، الأداء الجيد لا يثبت صحة Pedigree غير موثق.

---

## 16. تقييم الفرد عبر الشركاء والنسب

يمكن الجمع تحليليًا مستقبلًا بين:

- أصل الطائر؛
- أدائه الفردي؛
- أداء أزواجه المختلفة؛
- أداء الأبناء؛
- خطوط الشركاء؛
- مستوى القرابة.

لكن Phase 2C لا تبني نموذج التقييم أو KPIs.

---

## 17. Pedigree لمشتريات خارجية

عند شراء طائر أو زوج، قد تكون شهادة النسب:

- رسمية/موثقة؛
- سجل مربي؛
- صورة Pedigree؛
- تصريح بائع؛
- Imported Document؛
- غير موجودة.

لا يجوز تحويل Claim إلى Verified Parentage تلقائيًا.

---

## 18. استثناءات مهمة

- الأب معروف والأم مجهولة؛
- الأم معروفة والأب مجهول؛
- كلاهما مجهول؛
- Parentage claimed ثم تم تصحيحه؛
- Imported Pedigree غير مكتمل؛
- طائر Crossbred؛
- Foster-reared bird؛
- طائر تم شراؤه دون أي نسب؛
- نفس السلف يظهر عبر أكثر من فرع؛
- اختلاف أسماء السلالات/الخطوط بين وثيقتين؛
- Pedigree عميق لكن جزءًا منه Seller-reported فقط.

---

## 19. المخطط المفاهيمي للنسب

```text
Genetic Father ─┐
                ├─> Bird / Offspring
Genetic Mother ─┘

Bird / Offspring
   ├─ may enter Operational Pair P1
   ├─ may enter Operational Pair P2
   └─ may enter Operational Pair P3

Incubating Pair / Artificial Incubation
                ↓
              Egg

Rearing Pair / One Parent / Hand Feeding
                ↓
             Squab

Genetic Parentage remains unchanged.
```

---

## 20. تحقق ميداني مطلوب

- هل يحتفظ المربون المصريون بـ Pedigree أصلًا؟
- عدد الأجيال المعتاد إن وجد؛
- معنى "نسب مضمون" عمليًا؛
- استخدام شهادات النسب في حمام اللحم مقابل الزينة؛
- الاعتماد على Ring Numbers في Pedigree؛
- مدى صحة الأنساب عند شراء طيور بالغة؛
- هل يعرف المربون close inbreeding ويتجنبونه؟
- استخدام Linebreeding / Outcrossing / Crossbreeding؛
- وجود Pairing Plans مبنية على النسب؛
- هل يستخدم أي معامل رقمي للقرابة أو Inbreeding؟
- كيفية تصحيح Pedigree إذا ظهر خطأ.

هذه البنود غير حابسة.

---

## 21. الأدلة المضافة في Phase 2C

### SRC-032
**Framework for assessing genetic variation in livestock using demographic, pedigree, and genomic measures. Frontiers in Genetics. 2026.**  
الاستخدام: تعريف Inbreeding/Coancestry، أهمية Pedigree completeness وعمق الشجرة عند تفسير معاملات القرابة.

### SRC-033
**FAO — In situ conservation of livestock and poultry — Inbreeding section.**  
الاستخدام: توضيح أثر تزاوج الأقارب على homozygosity والتنوع واللياقة في سياق إدارة التربية الحيوانية؛ ليس مرجعًا خاصًا بالحمام المصري.

### SRC-034
**How depressing is inbreeding? A meta-analysis of 30 years of research on the effects of inbreeding in livestock. 2021.**  
الاستخدام: دعم أن inbreeding depression مفهوم موثق على نطاق الثروة الحيوانية وأن الأثر يعتمد على الصفة والسياق؛ لا تستخدم الدراسة لوضع Threshold للحمام.

---

## 22. Carry Forward

### إلى Phase 2D

- توحيد Pair + Pedigree + Bird + Breed + Farm Structure في baseline Phase 2؛
- مراجعة Same Pair Reunited؛
- مراجعة أي Open Questions جديدة/Field Validation؛
- تقييم جاهزية Phase 2 للاعتماد.

### إلى Phase 3

- ربط الأبناء بالأحداث الإنتاجية الفعلية؛
- Attribution إلى Genetic Parents مقابل Incubating/Rearing Pair؛
- Crossbred offspring؛
- أداء الأبناء؛
- Foster Transfer history.

### إلى Phase 6

- Inbreeding alerts / relationship checks؛
- Cross-pair performance analysis؛
- Parent/offspring performance reports؛
- Data Confidence in pedigree reports؛
- قواعد قرار التزاوج إن اعتمدها المستخدم لاحقًا.

### إلى Phase 8

- تقييم إدخال Pedigree depth؛
- Inbreeding Coefficient؛
- Pairing warnings؛
- Pedigree visualization؛
- Advanced breeding analytics

ضمن MVP أو Future Scope.

---

## 23. نتيجة Phase 2C — إدارة النسب

أهم المبادئ:

1. `Pedigree ≠ Pair History`.
2. `Genetic Parentage ≠ Incubating/Rearing Caregiving`.
3. Unknown/Partial Pedigree حالة صحيحة.
4. Pedigree له Confidence / Provenance.
5. تصحيح Parentage يجب أن يحفظ سبب ومصدر التعديل تاريخيًا.
6. `No Known Relationship ≠ Proven Unrelated`.
7. Inbreeding Coefficient مناسب مستقبلًا فقط عند توفر Pedigree كافٍ وموثوق.
8. Pedigree depth مفتوح ولا يفرض عدد أجيال ثابتًا.
9. Crossbreeding يجب أن ينعكس من الأبوين دون إجبار الابن على Pure Breed واحدة.
10. Pedigree لا يساوي Performance.
