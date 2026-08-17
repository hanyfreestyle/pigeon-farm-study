# Domain Terminology Glossary

> **Phase 1C Status:** Reviewed and normalized.  
> These are domain terms, not software entities. Preferred Arabic wording may still be refined through Egyptian field validation where noted.

## Terminology Rules

- Every term has a stable ID.
- English and preferred Arabic terms are kept together.
- Alternative Arabic wording is preserved when producer usage may vary.
- Definitions describe the real domain, not software structure.
- Operational meaning explains how the term matters on a farm.
- Ambiguous terms must always be used with their context or measurement anchor.
- A domain term does not automatically become a database table, class, enum, or software event.

---

## Normalized Terminology Index

| ID | English Term | Preferred Arabic Term | Alternative Arabic Terms | Definition | Operational Meaning | Related Terms | Evidence / Source | Notes |
|---|---|---|---|---|---|---|---|---|
| TERM-001 | Squab | زغلول حمام | زغلول | Young dependent pigeon; in meat production commonly the young bird produced for meat before/around weaning or independent flight. | Primary commercial output in this study. | Hatch, Weaning, Market Readiness | SRC-001, 002, 003 | Market age/weight is not inherent in the word. |
| TERM-002 | Pigeon | حمام | طائر حمام | Domestic pigeon used in the production population. | May be breeder, replacement, squab, retained young bird, etc. | Breeding Bird, Squab | Phase 1 synthesis | Do not assume one software identity model. |
| TERM-003 | Breeding Bird | طائر تربية / طائر إنتاج | حمام أمهات/آباء حسب الجنس والسياق | Bird admitted or intended for active reproduction. | Member of breeding population before or within a productive pair. | Breeding Readiness, Breeding Pair | Phase 1 synthesis | Sex-specific local wording needs validation. |
| TERM-004 | Breeding Pair | زوج إنتاج | زوج تربية | Male and female functioning together as a reproductive unit, typically sharing incubation and parental care. | Central production unit for natural squab production. | Pair Bond, Pairing, Clutch | SRC-002, 004, 005 | Biological and operational pair can diverge in exceptional management situations. |
| TERM-005 | Pair Bond | رابطة الزوج | الارتباط الزوجي | Persistent social/reproductive association between a male and female pigeon. | Supports mating, nest use, incubation and parental coordination. | Pairing, Re-pairing | SRC-004 | Does not mean pair membership can never change. |
| TERM-006 | Pairing | تكوين الزوج | التزاوج الموجّه/اختيار الزوج حسب السياق | Formation or deliberate establishment of a male–female breeding pair. | Can occur naturally or through controlled mate assignment. | Pair Bond, Controlled Pairing | SRC-004, Phase 1B | Pairing is not synonymous with one mating act. |
| TERM-007 | Re-pairing | إعادة تكوين الزوج | إعادة التزاوج | Formation of a new productive pair after loss, separation, infertility or management decision. | May interrupt production and changes pair history. | Pair Bond, Culling, Mate Loss | Phase 1A/1B | No universal timing/threshold. |
| TERM-008 | Clutch | بطن بيض | دفعة البيض / مجموعة البيض في دورة وضع واحدة | Eggs produced by one female as one discrete laying episode before the next laying interval. | Groups related eggs as one reproductive attempt. | Egg, Incubation, Hatch | SRC-001, 004; Phase 1B | Two eggs dominant, but one-egg clutch is possible. |
| TERM-009 | Egg | بيضة | — | Individual pigeon egg laid during a reproductive episode. | Has its own date, condition and outcome even when part of a clutch. | Clutch, Fertility, Incubation | Phase 1B | Egg outcome ≠ clutch outcome. |
| TERM-010 | Nest | عش | — | Physical nesting site used for laying, incubation and/or squab rearing. | Working reproductive location. | Nest Box, Double Nest | SRC-001, 005 | Pair may use more than one nest. |
| TERM-011 | Nest Box | صندوق عش | خانة عش | Defined housing structure/compartment intended to provide a nesting site. | Makes nest location more controlled/identifiable. | Nest, Pair Cage | Phase 1A sources | Physical form varies. |
| TERM-012 | Double Nest System | نظام العشّين | العش المزدوج | Provision of two nesting sites to a breeding pair. | Supports simultaneous older-squab rearing and a new clutch. | Overlapping Production Cycle | SRC-001, 002, 005 | Prevalence in target Egyptian farms requires validation. |
| TERM-013 | Incubation | حضانة البيض | الرقاد على البيض | Period/behavior maintaining eggs under conditions supporting embryo development until hatch. | Both parents normally participate. | Clutch, Hatch | SRC-001, 004, 005 | Start anchor can be ambiguous. |
| TERM-014 | Hatching / Hatch | الفقس | — | Successful emergence of a squab from an egg. | Key observable reproductive outcome. | Hatchability, Dead-in-shell | SRC-001, 005, 012 | Hatch timing depends on effective incubation anchor. |
| TERM-015 | Brooding / Rearing | رعاية الزغاليل | التحضين/التربية بعد الفقس | Parent or substitute care of dependent squabs after hatch. | Includes warmth, feeding and protection. | Crop Milk, Fostering | SRC-003, 004, 005 | “Brooding” may be used differently across poultry contexts. |
| TERM-016 | Crop Milk / Pigeon Milk | لبن الحوصلة | حليب الحمام | Nutrient-rich crop secretion produced by both parent pigeons for early squab feeding. | Critical early nutrition. | Squab, Parental Care | SRC-003, 004, 021 | Not mammalian milk. |
| TERM-017 | Fertility | الخصوبة / نسبة البيض المخصب | الإخصاب حسب السياق | Proportion or condition of eggs that are fertilized. | Used to evaluate reproductive performance. | Candling, Hatchability | SRC-006, 010, 014 | Denominator must be explicit. |
| TERM-018 | Hatchability | نسبة الفقس | قابلية الفقس | Measure of successful hatching. | Used for reproductive performance diagnosis. | Fertility, Hatch | SRC-006, 010, 014 | May be per eggs laid/set or per fertile eggs. |
| TERM-019 | Embryonic Death | نفوق الجنين داخل البيضة | موت الجنين | Death of a previously developing embryo before successful hatch. | Distinct from infertility. | Dead-in-shell, Hatch Failure | Phase 1B / avian literature | Can occur at different stages. |
| TERM-020 | Dead-in-shell | جنين نافق داخل القشرة | فشل فقس متأخر | Late-stage embryo dies/fails to complete hatch. | Important hatch-failure outcome. | Embryonic Death, Hatchability | Phase 1B sources | Diagnostic criteria may need veterinary context. |
| TERM-021 | Weaning | الفطام | الاستقلال عن تغذية الأبوين | Transition toward independent feeding; research may also use it for managed separation. | Determines end/alteration of parental feeding pathway. | Early Separation, Market Readiness | SRC-002, 017 | Physiological weaning and management separation can differ. |
| TERM-022 | Early Separation / Early Weaning | الفصل المبكر | الفطام المبكر | Deliberate removal from parents earlier than conventional natural rearing, with artificial/hand feeding as needed. | Creates an alternate intensive lifecycle. | Weaning, Artificial Feeding | SRC-002 | Not simply “selling earlier.” |
| TERM-023 | Market Readiness | الجاهزية للتسويق | جاهز للبيع | Commercial condition satisfying buyer/farm requirements for sale. | May depend on age, weight, feathering and sale form. | Market Age, Weaning | Phase 1A/1B synthesis | Not a universal biological status. |
| TERM-024 | Replacement Bird | طائر إحلال | بديل تربية | Bird retained/selected to replace breeding stock and enter future production. | Maintains breeder population. | Breeding Readiness, Culling | Phase 1A/1B | Admission criteria require field validation. |
| TERM-025 | Culling | الاستبعاد من قطيع الإنتاج | استبعاد | Intentional removal from active breeding/production for health, welfare, genetic or productivity reasons. | Ends active productive role. | Sale, Retirement, Replacement | Phase 1A | Not synonymous with mortality. |
| TERM-026 | Fostering | التربية بواسطة زوج بديل | التحضين البديل / أبوين بديلين | Transfer of an egg or dependent squab to another pair for incubation/care. | Changes caregiving responsibility and may rescue output after parent problems. | Foster Parent, Parent Loss | SRC-005, 017 | Prevalence in commercial Egypt unknown. |
| TERM-027 | Sexual Maturity | النضج الجنسي | — | Biological stage at which reproductive capacity is developed. | Necessary but not sufficient for commercial breeding entry. | Breeding Readiness | SRC-003, 012, 017 | Broadly ~5–7+ months depending on strain/definition. |
| TERM-028 | Operational Breeding Readiness | الجاهزية لدخول قطيع الإنتاج | الجاهزية التشغيلية للتكاثر | Farm judgment that a mature bird is sufficiently developed, healthy and suitable for active breeding. | Admission decision for replacement stock. | Sexual Maturity, Body Condition | Phase 1B synthesis | Analytical domain phrase; not standardized threshold. |
| TERM-029 | Oviposition Interval | الفاصل بين وضع البيض | فاصل وضع البيض | Time between successive egg-laying events in a stated context. | Within-clutch interval is commonly about two days. | Egg 1, Egg 2, Clutch | SRC-016 | Must state whether within clutch or between clutches. |
| TERM-030 | Candling | فحص البيض بالضوء | تسليط الضوء على البيضة | Non-destructive visual inspection using transmitted light to assess development. | Can support fertility/development checking. | Fertility, Embryonic Death | SRC-018 | Routine farm adoption needs validation. |
| TERM-031 | Production Cycle | دورة الإنتاج | الدورة الإنتاجية | General farm/research phrase for repeated production activity; no single universal boundary. | Must be qualified by exact start/end anchor. | Reproductive Cycle, Clutch Cycle | Phase 1A/1B | **Ambiguous term.** |
| TERM-032 | Reproductive Cycle | دورة التكاثر | الدورة التناسلية | Repeated reproductive sequence/interval defined by a study or farm. | May include laying, incubation, rearing and next-lay components. | Production Cycle | SRC-002, 012; Phase 1B | Anchor must be stated. |
| TERM-033 | Egg-laying Cycle | دورة وضع البيض | دورة البيض | Interval or sequence focused specifically on repeated laying output. | Useful when studying laying-to-laying timing. | Oviposition Interval, Clutch | Phase 1B | Not equal to full squab-rearing cycle. |
| TERM-034 | Overlapping Production Cycle | تداخل دورات الإنتاج | تداخل دورات التكاثر | Condition where a pair begins a subsequent clutch while still caring for squabs from an earlier clutch. | Core characteristic of commercial pigeon lifecycle. | Double Nest, Next Clutch | SRC-001, 002, 005, 012 | Must not be flattened into one linear timeline. |
| TERM-035 | Loft | مسكن جماعي للحمام | لوفت / حظيرة حمام | Shared housing containing multiple birds and nesting locations. | Communal production environment. | Dovecote, Colony | SRC-007, 008 | Not one standardized physical design. |
| TERM-036 | Dovecote | برج حمام | مسكن حمام تقليدي | Structure designed for communal pigeon housing/nesting with multiple nest openings/compartments. | Traditional/commercial housing form. | Loft, Colony | SRC-007 | Mud dovecote documented in Sharqia. |
| TERM-037 | Colony System | نظام تربية جماعي | نظام مستعمرة / إسكان جماعي | Multiple pigeons/pairs share a housing area and nesting environment. | Pair/nest attribution may be less controlled. | Loft, Dovecote | SRC-007, 008 | Exact form varies. |
| TERM-038 | Individual Pair Cage | قفص زوج إنتاج منفرد | بطارية/قفص زوجي حسب المزرعة | Housing where one known male–female pair occupies a controlled cage/unit. | Improves pair attribution and pair-level recording. | Breeding Pair, Nest Box | SRC-002, 005, 008 | Do not assume universally superior. |
| TERM-039 | Parent-reared Squab | زغلول مُربّى بواسطة الأبوين | — | Squab naturally fed/cared for by its parent pair through the dependent period. | Natural baseline pathway. | Early Separation, Fostering | SRC-002, 005 | Useful comparison category. |

---

## Ambiguous Domain Terms

### Production Cycle

**Possible meanings:** pairing cycle, first-egg-to-next-first-egg, clutch-to-clutch, incubation period, hatch-to-next-lay, full reproduction plus rearing, or a farm-defined accounting interval.

**Context:** research papers and farms can legitimately use different anchors.

**Risk of misuse:** a future system could silently calculate the wrong duration, prevent overlapping cycles, or compare unlike records.

**Recommended wording during future analysis:** avoid the unqualified phrase in calculations. Use explicit wording such as `first egg → next first egg`, `hatch → next laying`, `clutch → next clutch`, or `rearing period`.

### Weaning

**Possible meanings:** true feeding independence; physical separation from parents; research treatment called “weaning” even when artificial feeding continues.

**Risk of misuse:** early separation could be mistaken for physiological independence or sale age.

**Recommended wording:** state `parent separation`, `independent feeding`, or `market sale` explicitly.

### Market Readiness

**Possible meanings:** buyer-specified live age/weight, dressed-bird specification, farm-defined target, or general 3–4-week traditional reference.

**Risk of misuse:** turning research age/weight into a commercial rule.

**Recommended wording:** state customer/market, live vs dressed, age, weight and other criteria separately.

### Fertility

**Possible meanings:** egg is biologically fertilized; farm percentage of fertile eggs; result inferred by candling.

**Risk of misuse:** percentages become incomparable when denominators/methods differ.

**Recommended wording:** always state numerator, denominator, and confirmation method.

### Hatchability

**Possible meanings:** hatched eggs / all eggs; hatched eggs / fertile eggs; eggs set rather than eggs laid.

**Risk of misuse:** apparently contradictory farm performance.

**Recommended wording:** use `hatchability of all eggs` or `hatchability of fertile eggs` with formula.

### Breeding Readiness

**Possible meanings:** sexual maturity, producer decision, minimum age, minimum weight, acceptable body condition.

**Risk of misuse:** treating biological maturity as automatic farm admission.

**Recommended wording:** keep `Sexual Maturity` and `Operational Breeding Readiness` separate.

### Loft / Dovecote / Colony

**Possible meanings:** vary substantially by country and local building form.

**Risk of misuse:** assuming a term defines cage layout, pair control, nesting arrangement, identification or capacity.

**Recommended wording:** use the term plus an actual physical/operational description in Phase 2.

---

## Terminology Review Result

- Core Phase 1 terms are normalized.
- Ambiguous lifecycle and performance terms are explicitly flagged.
- Arabic farm vocabulary that may vary locally remains open for field validation.
- No terminology item has been converted into a software entity, table, enum, or business rule.
