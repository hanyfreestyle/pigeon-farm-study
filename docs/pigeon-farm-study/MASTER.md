# Pigeon Farm Management System — Master Study File

> Central source of truth for the study status, decisions, working rules, assumptions, open questions, and review direction.

## Project Vision

دراسة وتحليل وتصميم نظام متكامل لإدارة مزارع الحمام التجاري، مع التركيز الأساسي على **Commercial Meat Pigeon / Squab Production** وإدارة العمليات المرتبطة بإنتاج الزغاليل بصورة قابلة للقياس والتحليل والتحويل لاحقًا إلى نظام برمجي عملي.

الهدف في هذه الدراسة ليس البدء من افتراضات برمجية، بل فهم المجال التشغيلي أولًا، ثم استخلاص متطلبات العمل وقواعده وكياناته وعلاقاته، وبعد ذلك فقط الانتقال إلى تصميم النظام والبيانات والـ MVP والبنية التقنية.

## Study Objectives

- بناء فهم موثق لمجال مزارع الحمام التجاري الموجه لإنتاج الزغاليل/الحمام اللاحم.
- توثيق دورة الإنتاج والعمليات اليومية ونقاط القرار والقياس.
- تحديد مفاهيم المجال وكياناته التشغيلية قبل تحويلها إلى مفاهيم برمجية.
- استخراج Business Rules بصورة منفصلة عن الافتراضات والممارسات المتغيرة بين المزارع.
- تحديد مؤشرات الأداء والتقارير والتنبيهات المطلوبة لإدارة المزرعة.
- تحديد احتياجات الصحة، التغذية، المخزون، المشتريات، المبيعات والمصروفات ضمن نطاق المشروع.
- الوصول تدريجيًا إلى Data Model وSystem Design مبنيين على التحليل وليس على التخمين.
- تعريف MVP واضح ومحدود قابل للتنفيذ لاحقًا.
- تجهيز أساس معماري مناسب للتقنية المستهدفة بدون تنفيذ تقني خلال مراحل الدراسة المبكرة.
- إنتاج دراسة نهائية متسقة بعد مراجعة واعتماد جميع المراحل.

## Scope

### In Scope

التركيز الرئيسي للدراسة هو:

**Commercial Meat Pigeon / Squab Production**

ويشمل — عند الوصول إلى مراحله المناسبة — فهم وإدارة الجوانب التشغيلية والتجارية والصحية والإنتاجية اللازمة لمزرعة حمام تجاري لإنتاج الزغاليل، بما في ذلك ما يرتبط بالبنية التشغيلية للمزرعة، الحمام، السلالات، الأزواج، النسب، دورة التكاثر، البيض، الفقس، الزغاليل، الأداء، الصحة، التغذية، النفوق، المخزون، المشتريات، الموردين، العملاء، المبيعات، المصروفات، التقارير، التنبيهات، الصلاحيات، وقواعد العمل.

يمكن دراسة الجوانب المشتركة مع أنماط أخرى من تربية الحمام **فقط عند الحاجة لفهم المجال الأساسي**، دون تحويل الدراسة إلى نظام عام لكل أنواع تربية الحمام.

### Out of Scope — Current Study Initialization

في Phase 0 لا يدخل ضمن العمل:

- البحث التفصيلي في تربية الحمام التجاري.
- تحديد قيم أو معايير إنتاجية أو بيطرية.
- تصميم Software Entities.
- تصميم Database Tables أو Schema.
- تنفيذ Migrations أو Models أو Resources أو Services أو Enums أو Controllers.
- تنفيذ Filament Resources أو أي واجهات تطبيق.
- كتابة كود Laravel / PHP / SQL.
- تعريف تفاصيل الـ MVP قبل انتهاء التحليل السابق له.
- تجميع التقرير النهائي.

## Study Methodology

تسير الدراسة بالتسلسل التالي، ولا يتم القفز إلى مرحلة لاحقة إذا كانت تعتمد على فهم لم يكتمل بعد:

**Research**
→ **Domain Understanding**
→ **Operational Analysis**
→ **Business Analysis**
→ **Business Rules**
→ **Data Modeling**
→ **System Design**
→ **MVP Definition**
→ **Technical Architecture**
→ **Final Review**

المبدأ الحاكم: **التحليل يولّد التصميم، وليس العكس.**

## Study Phases

| Phase | Name | Status | Files | Dependencies | Review Status | Notes |
|---|---|---|---|---|---|---|
| Phase 0 | Study Initialization | In Progress | `MASTER.md`, review files, placeholders | None | Needs Review | إنشاء هيكل الدراسة وقواعد العمل فقط. |
| Phase 1 | Domain Research | Pending | `01-domain-research/*` | Phase 0 | Pending | Commercial Pigeon Farming & Production Lifecycle. |
| Phase 2 | Farm Structure & Core Domain | Pending | `02-farm-structure/*` | Phase 1 | Pending | فهم الهيكل التشغيلي ومفاهيم الحمام/السلالات/الأزواج/النسب. |
| Phase 3 | Production Analysis | Pending | `03-production/*` | Phases 1–2 | Pending | تحليل دورة الإنتاج والتكاثر والبيض والفقس والزغاليل والأداء. |
| Phase 4 | Health & Feed | Pending | `04-health-feed/*` | Phases 1–3 | Pending | الصحة والعلاجات والتحصينات والنفوق والتغذية. |
| Phase 5 | Operations & Finance | Pending | `05-operations-finance/*` | Phases 1–4 | Pending | المخزون والمشتريات والموردون والعملاء والمبيعات والمصروفات. |
| Phase 6 | System Analysis | Pending | `06-system-analysis/*` | Phases 1–5 | Pending | KPIs، التقارير، التنبيهات، الصلاحيات، Business Rules وDomain Events. |
| Phase 7 | Technical Design | Pending | `07-technical-design/*` | Phase 6 | Pending | Data Model والعلاقات والمعمارية وAudit Trail بعد اكتمال تحليل المجال. |
| Phase 8 | MVP Definition | Pending | `08-mvp/*` | Phases 6–7 | Pending | تحديد MVP ومراحل التطوير واتجاهات AI المستقبلية. |
| Phase 9 | Final Review & Consolidation | Pending | `09-review/*`, `FINAL-STUDY.md` | Phases 1–8 | Pending | مراجعة الاتساق وإغلاق الأسئلة وتجميع الدراسة النهائية بعد الاعتماد. |

## Decision Log

> أي قرار مؤثر في الدراسة يجب تسجيله هنا. القرار Approved لا يتم تغييره بصمت؛ إذا استدعى الأمر تغييره، يُسجل قرار جديد يوضح سبب التعديل وتأثيره.

| Decision ID | Date | Phase | Decision | Reason | Impact | Status |
|---|---|---|---|---|---|---|
| DEC-001 | 2026-08-17 | Phase 0 | التركيز الرئيسي للدراسة هو Commercial Meat Pigeon / Squab Production. | منع تحول المشروع إلى نظام عام لكل استخدامات الحمام والحفاظ على وضوح المجال. | يحدد اتجاه البحث والتحليل في جميع المراحل التالية. | Approved |
| DEC-002 | 2026-08-17 | Phase 0 | لا يتم تصميم Software Entities أو Database Tables قبل فهم Domain Entities ودورة العمل. | منع التصميم المبكر القائم على افتراضات برمجية. | يؤخر Data Modeling حتى اكتمال التحليل اللازم ويجعل النموذج نتيجة للدراسة. | Approved |
| DEC-003 | 2026-08-17 | Phase 0 | التقنية المستهدفة مبدئيًا: Laravel 12، PHP 8.2+، Filament 4، MySQL، بدون أي Technical Implementation في Phase 0. | تثبيت سياق تقني مستقبلي دون السماح له بقيادة تحليل المجال. | يستخدم لاحقًا كقيد معماري بعد اكتمال مراحل التحليل المناسبة. | Approved |

## Research Evidence Policy

كل معلومة Domain Knowledge مؤثرة يجب — قدر الإمكان — دعمها بمصدر موثوق، مع الفصل الصريح بين درجة المعرفة وطبيعتها.

### Evidence Classes

**Verified Fact**  
معلومة مدعومة بمصدر أو أكثر من مصادر جيدة وموثوقة، ويمكن استخدامها كأساس للتحليل مع تسجيل المصدر.

**Industry Practice**  
ممارسة شائعة أو نمط تشغيلي معروف، لكنها قد تختلف حسب حجم المزرعة أو البلد أو السلالة أو أسلوب الإدارة. لا تُعامل كقاعدة عامة ثابتة بدون تحقق.

**Assumption**  
افتراض مؤقت يسمح بمواصلة الدراسة عند نقص معلومة. يجب تسجيله في `09-review/assumptions.md` وربطه بطريقة تحقق. **لا يجوز تحويله إلى Fact دون دليل.**

**Design Decision**  
قرار نتخذه لبناء النظام أو الدراسة استنادًا إلى متطلبات واضحة وتحليل موثق. القرارات المهمة تسجل في Decision Log.

**Open Question**  
نقطة لا يمكن حسمها بأمان من المصادر وحدها أو تحتاج إلى تحديد من صاحب مزرعة/خبير/Stakeholder. تسجل في `09-review/open-questions.md`.

### Evidence Rules

- لا يتم عرض الرأي أو الممارسة الشائعة كحقيقة علمية ثابتة.
- عند اختلاف المصادر، يسجل التعارض بدل إخفائه، ويؤجل الحسم إذا لزم.
- المعلومات التي قد تختلف حسب السياق المحلي يجب تمييزها بوضوح.
- الأولوية للمصادر الأكاديمية والجامعية والحكومية والبيطرية والمهنية الموثوقة.
- Blogs وForums ومواد التسويق قد تستخدم كإشارة أو لفهم الممارسة الواقعية، لكن لا تعتمد منفردة كأساس لمعلومة مهمة.
- عند الحاجة إلى استنتاج تحليلي من عدة مصادر، يوصف بأنه **Analysis / Inference** وليس نصًا من المصدر.

## Source Tracking

عند استخدام مصدر مهم داخل أي ملف من ملفات الدراسة، يسجل بالصيغة الموحدة التالية:

```text
Source ID: SRC-XXX
Source: <Title / Document / Page>
URL: <URL>
Organization / Author: <Organization or Author>
Publication Date: <YYYY-MM-DD or Unknown>
Access Date: <YYYY-MM-DD>
Reliability: High | Medium | Low
Information Used: <What information was used from this source>
Notes: <Optional limitations / conflicts / context>
```

### Source Selection Priority

1. Academic research and peer-reviewed literature.
2. Universities and agricultural extension material.
3. Government and official veterinary/agricultural authorities.
4. Recognized professional, veterinary, breeding, or livestock organizations.
5. High-quality technical/professional publications.
6. Commercial sources, blogs, forums, and informal practitioner material only as supplementary evidence where useful.

## Working Rules for All Future Phases

قبل تنفيذ أي Phase مستقبلية يجب:

1. قراءة `MASTER.md`.
2. قراءة الملفات السابقة المرتبطة بالمرحلة.
3. مراجعة `09-review/open-questions.md`.
4. مراجعة `09-review/assumptions.md`.
5. عدم تكرار بحث تم اعتماده سابقًا إلا عند الحاجة للتحقق أو ظهور تعارض أو معلومات أحدث.
6. عدم تغيير قرار حالته Approved بدون تسجيل قرار جديد في Decision Log يشرح التغيير.
7. تسجيل أي تعارض يظهر بين المصادر في الملف المناسب ومراجعته في `09-review/consistency-review.md`.
8. تسجيل أي Assumption جديد في `09-review/assumptions.md`.
9. تسجيل أي Open Question جديد في `09-review/open-questions.md`.
10. تحديث حالة المرحلة في هذا الملف بعد العمل.

## Domain-First Design Rule

**لا تصمم Software Entities قبل فهم Domain Entities.**

**ولا تصمم Database Tables قبل الانتهاء من تحليل دورة العمل ذات الصلة.**

أسماء المجال لا تتحول تلقائيًا إلى جداول أو Classes. على سبيل المثال، لا يجوز افتراض أن:

- `Pigeon = database table`
- `Pair = database table`

قبل دراسة معنى هذه المفاهيم في التشغيل الفعلي، دورة حياتها، علاقاتها، حالات التغيير، القيود، ومتطلبات التتبع والتقارير.

تصميم البيانات يجب أن يكون **نتيجة للتحليل** وليس نقطة البداية.

## Scope Control / Scope Creep Prevention

إذا ظهر أثناء أي Phase موضوع مفيد ولكنه خارج المرحلة الحالية:

- لا تتم دراسته تفصيليًا في نفس المرحلة.
- يسجل في **Future Research Queue** أدناه.
- يحدد سبب أهميته والمرحلة المناسبة لدراسته.
- لا ينتقل إلى نطاق التنفيذ إلا عند بدء مرحلته أو صدور قرار واضح بذلك.

## Future Research Queue

| Queue ID | Topic | Why It Matters | Recommended Phase | Status | Notes |
|---|---|---|---|---|---|
| — | No queued topics yet | — | — | — | يتم تحديث الجدول عند ظهور موضوع خارج نطاق المرحلة الحالية. |

## Target Technology Context

التقنية المتوقع استخدامها لاحقًا للتنفيذ:

- Laravel 12
- PHP 8.2+
- Filament 4
- MySQL

هذه التقنية **سياق مستقبلي وليست نقطة انطلاق لتحليل المجال**.

### Phase 0 Technical Prohibition

لا يتم في Phase 0 إنشاء أو تنفيذ أي من التالي:

- Migrations
- Models
- Resources
- Services
- Enums
- Controllers
- Filament Resources
- Database Schema
- Application Code

## Phase 0 Completion Gate

Phase 0 يقتصر على تهيئة الدراسة. لا يبدأ Phase 1 إلا بتعليمات مستقلة وصريحة.

الحالة الحالية: **In Progress — awaiting review/approval.**
