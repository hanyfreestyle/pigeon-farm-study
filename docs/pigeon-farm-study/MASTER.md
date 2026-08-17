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

### Out of Scope During Domain Research

- تصميم Software Entities.
- تصميم Database Tables أو Schema.
- تنفيذ Migrations أو Models أو Resources أو Services أو Enums أو Controllers.
- تنفيذ Filament Resources أو واجهات تطبيق.
- كتابة كود Laravel / PHP / SQL.
- تعريف MVP قبل انتهاء التحليل السابق له.
- تجميع التقرير النهائي.

## Study Methodology

**Research** → **Domain Understanding** → **Operational Analysis** → **Business Analysis** → **Business Rules** → **Data Modeling** → **System Design** → **MVP Definition** → **Technical Architecture** → **Final Review**

المبدأ الحاكم: **التحليل يولّد التصميم، وليس العكس.**

## Study Phases

| Phase | Name | Status | Files | Dependencies | Review Status | Notes |
|---|---|---|---|---|---|---|
| Phase 0 | Study Initialization | Completed | `MASTER.md`, review files, placeholders | None | Approved by transition | متطلبات التهيئة اكتملت، والانتقال إلى Phase 1 تم بتعليمات صريحة. |
| Phase 1 | Domain Research | In Progress | `01-domain-research/*` | Phase 0 | Phase 1A & 1B Awaiting Review | Phase 1A وPhase 1B مكتملتان؛ Phase 1C لم تبدأ. |
| Phase 2 | Farm Structure & Core Domain | Pending | `02-farm-structure/*` | Phase 1 | Pending | فهم الهيكل التشغيلي ومفاهيم الحمام/السلالات/الأزواج/النسب. |
| Phase 3 | Production Analysis | Pending | `03-production/*` | Phases 1–2 | Pending | تحليل دورة الإنتاج والتكاثر والبيض والفقس والزغاليل والأداء. |
| Phase 4 | Health & Feed | Pending | `04-health-feed/*` | Phases 1–3 | Pending | الصحة والعلاجات والتحصينات والنفوق والتغذية. |
| Phase 5 | Operations & Finance | Pending | `05-operations-finance/*` | Phases 1–4 | Pending | المخزون والمشتريات والموردون والعملاء والمبيعات والمصروفات. |
| Phase 6 | System Analysis | Pending | `06-system-analysis/*` | Phases 1–5 | Pending | KPIs، التقارير، التنبيهات، الصلاحيات، Business Rules وDomain Events. |
| Phase 7 | Technical Design | Pending | `07-technical-design/*` | Phase 6 | Pending | Data Model والعلاقات والمعمارية وAudit Trail بعد اكتمال تحليل المجال. |
| Phase 8 | MVP Definition | Pending | `08-mvp/*` | Phases 6–7 | Pending | تحديد MVP ومراحل التطوير واتجاهات AI المستقبلية. |
| Phase 9 | Final Review & Consolidation | Pending | `09-review/*`, `FINAL-STUDY.md` | Phases 1–8 | Pending | مراجعة الاتساق وإغلاق الأسئلة وتجميع الدراسة النهائية بعد الاعتماد. |

## Phase 1 Subphase Progress

| Subphase | Name | Status | Primary File | Notes |
|---|---|---|---|---|
| Phase 1A | Commercial Pigeon Farming Domain Research | Completed — Awaiting Review | `01-domain-research/commercial-pigeon-farming.md` | 15 tracked sources; Egyptian and international evidence; contradictions and field-validation gaps documented. |
| Phase 1B | Detailed Pigeon Production Lifecycle | Completed — Awaiting Review | `01-domain-research/production-lifecycle.md` | Lifecycle timeline, overlapping cycles, failures, observable events and Egyptian timing evidence documented. |
| Phase 1C | Domain Terminology, Evidence Consolidation & Validation Review | Pending | To be defined by Phase 1C instruction | Do not start without independent user instruction. |

## Decision Log

| Decision ID | Date | Phase | Decision | Reason | Impact | Status |
|---|---|---|---|---|---|---|
| DEC-001 | 2026-08-17 | Phase 0 | التركيز الرئيسي للدراسة هو Commercial Meat Pigeon / Squab Production. | منع Scope Drift. | يحدد اتجاه البحث والتحليل. | Approved |
| DEC-002 | 2026-08-17 | Phase 0 | لا يتم تصميم Software Entities أو Database Tables قبل فهم Domain Entities ودورة العمل. | منع التصميم المبكر. | Data Modeling نتيجة للتحليل. | Approved |
| DEC-003 | 2026-08-17 | Phase 0 | التقنية المستهدفة مبدئيًا Laravel 12 + PHP 8.2+ + Filament 4 + MySQL بدون تنفيذ تقني مبكر. | تثبيت السياق التقني دون فرضه على المجال. | يعاد تقييمه في Phase 7. | Approved |
| DEC-004 | 2026-08-17 | Phase 0 → Phase 1 | اعتبار تعليمات Phase 1A الصريحة موافقة على اكتمال Phase 0 والانتقال إلى Domain Research. | Phase 0 كانت مستوفاة والمستخدم بدأ المرحلة التالية. | Phase 0 Completed وPhase 1 In Progress. | Approved |

## Research Evidence Policy

تصنف المعلومات المهمة إلى:

- **Verified Fact:** مدعومة بمصادر جيدة.
- **Strong Evidence:** أدلة قوية ومتعددة أو مباشرة.
- **Moderate Evidence:** دعم جيد لكن محدود بالسياق أو عدد الدراسات.
- **Industry Practice:** ممارسة شائعة قد تختلف بين المزارع.
- **Expert/Producer Practice:** ممارسة ميدانية تحتاج تحققًا أوسع.
- **Assumption:** افتراض مؤقت مسجل ولا يتحول إلى Fact بدون دليل.
- **Design Decision:** قرار تصميمي لاحق مبني على تحليل موثق.
- **Open Question / Requires Field Validation:** نقطة تحتاج صاحب مزرعة أو متخصصًا أو سياق السوق المستهدف.

### Evidence Rules

- لا يتم عرض الرأي أو الممارسة الشائعة كحقيقة علمية ثابتة.
- عند اختلاف المصادر يسجل التعارض ولا يُخفى.
- المعلومات التي تختلف حسب السياق المحلي تميز بوضوح.
- الأولوية للمصادر الأكاديمية والجامعية والحكومية والبيطرية والمهنية الموثوقة.
- Blogs وForums لا تستخدم منفردة لإثبات معلومة مهمة.
- الاستنتاجات المركبة توصف بأنها Analysis / Inference.

## Source Tracking

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

## Working Rules for All Future Phases

1. قراءة `MASTER.md`.
2. قراءة الملفات السابقة المرتبطة بالمرحلة.
3. مراجعة `09-review/open-questions.md`.
4. مراجعة `09-review/assumptions.md`.
5. عدم تكرار بحث معتمد إلا للتحقق/التوسع/حل تعارض.
6. عدم تغيير قرار Approved بدون Decision Log جديد.
7. تسجيل تعارضات المصادر.
8. تسجيل أي Assumption جديد.
9. تسجيل أي Open Question جديد.
10. تحديث حالة المرحلة و`STUDY-LOG.md` بعد كل مهمة رئيسية.

## Domain-First Design Rule

**لا تصمم Software Entities قبل فهم Domain Entities، ولا تصمم Database Tables قبل الانتهاء من تحليل دورة العمل ذات الصلة.**

لا يجوز افتراض أن `Pigeon = database table` أو `Pair = database table`. أسماء المجال لا تتحول تلقائيًا إلى Classes أو جداول.

## Scope Control / Scope Creep Prevention

أي موضوع مفيد خارج المرحلة الحالية يسجل في Future Research Queue ولا يُفتح تفصيليًا قبل مرحلته.

## Future Research Queue

| Queue ID | Topic | Why It Matters | Recommended Phase | Status | Notes |
|---|---|---|---|---|---|
| FRQ-001 | Detailed chronological egg lifecycle and egg-management workflow | تم بناء الأساس الزمني في Phase 1B؛ الإدارة التفصيلية للبيض لاحقة. | Phase 3 | Partially Researched | لا Software workflow الآن. |
| FRQ-002 | Detailed squab growth, weaning and market-readiness workflow | Phase 1B أثبت فصل weaning عن market readiness والحاجة لسياق السوق. | Phase 3 / 5 | Partially Researched | يحتاج Egyptian field validation. |
| FRQ-003 | Disease, vaccination, treatment, quarantine and biosecurity protocols | عوامل تشغيلية خارج نطاق Phase 1. | Phase 4 | Queued | لا قواعد علاجية الآن. |
| FRQ-004 | Feed formulation, nutrient requirements and feed strategy | التغذية تؤثر على breeder/squab performance. | Phase 4 | Queued | — |
| FRQ-005 | Feed inventory, purchasing and supplier operations | feed مدخل وتكلفة إنتاج. | Phase 5 | Queued | — |
| FRQ-006 | Formal production KPI definitions and benchmark normalization | lifecycle كشف اختلاف التعريفات والـ anchors والdenominators. | Phase 6 | Queued | بعد اكتمال domain analysis. |
| FRQ-007 | Software representation of pair, nest, clutch, bird identity and overlapping cycles | Phase 1B أكد التداخل والتعدد الزمني. | Phase 7 | Queued | ممنوع البدء الآن. |
| FRQ-008 | Artificial incubation / early-weaning workflow as optional production model | يغير lifecycle بصورة جوهرية ومدى استخدامه المصري غير محسوم. | Phase 3 | Partially Researched | Field validation أولًا. |
| FRQ-009 | Formal operational definition(s) of Production Cycle | Phase 1B أثبت وجود عدة anchors صحيحة حسب غرض القياس. | Phase 3 / 6 | Queued | لا تعريف Software في Phase 1. |

## Target Technology Context

- Laravel 12
- PHP 8.2+
- Filament 4
- MySQL

هذه التقنية سياق مستقبلي وليست نقطة انطلاق لتحليل المجال.

### Technical Prohibition During Domain Research

لا يتم خلال Phase 1 إنشاء أو تنفيذ Migrations, Models, Resources, Services, Software Enums, Controllers, Filament Resources, ERD, Database Schema, APIs, UI, Dashboard Design, Software Architecture أو Application Code.

## Current Study Position

- **Current Phase:** Phase 1 — Domain Research
- **Completed Subphase:** Phase 1A — Commercial Pigeon Farming Domain Research
- **Completed Subphase:** Phase 1B — Detailed Pigeon Production Lifecycle
- **Subphase Review:** Phase 1A & 1B Awaiting Review
- **Phase 1 Overall Status:** In Progress
- **Next recommended subphase:** Phase 1C — Domain Terminology, Evidence Consolidation & Validation Review
- **Stop condition:** Do not start Phase 1C until independent user instruction is received.
