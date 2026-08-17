# Detailed Pigeon Production Lifecycle — Domain Research

> **Phase:** 1B — Detailed Pigeon Production Lifecycle  
> **Status:** Completed — Awaiting Review  
> **Scope:** Commercial Meat Pigeon / Squab Production  
> **Research date:** 2026-08-17  
> **Rule:** This document describes real biological and farm-operational processes only. It does **not** define database tables, status enums, software events, APIs, UI, or architecture.

---

## 1. Lifecycle Executive Summary

Commercial pigeon production is a repeated reproductive process centered on a breeding pair, but it is **not a simple linear cycle**. The biological sequence normally contains courtship, pair bonding, nest selection/building, mating, egg laying, incubation, hatch, parental feeding, squab growth, and a subsequent laying episode. However, the next laying episode may begin **before the previous squabs leave the nest**, creating genuine overlap between two reproductive outputs of the same pair [SRC-001, SRC-002, SRC-004].

A useful operational reading is therefore:

**Breeding-ready birds → Pair formation/bond → Courtship & nest activity → Egg 1 → Egg 2 / clutch completion → Effective incubation → Fertility/development observation → Hatch → Crop-milk-dependent squab → Mixed parental feeding → Pre-weaning/market stage → Next clutch may already be underway.**

The dominant pattern in domestic meat pigeons is a two-egg clutch laid approximately two days apart, incubation around 17–20 days, and natural parental rearing for approximately 3–4 weeks. These are **reference ranges, not universal constants**. Breed, parent age, housing, thermal environment, egg-removal/fostering, artificial incubation, and especially early separation/weaning can materially alter observed cycle length and output [SRC-002, SRC-003, SRC-012, SRC-016, SRC-017].

---

## 2. Entry into the Breeding Population

### 2.1 Biological maturity

Recent reviews report reproductive-organ development beginning around 5–6 months and sexual maturity around 6–7 months in domestic pigeons [SRC-003, SRC-017]. Egyptian research has also worked with base breeding populations around 5–6 months and reported strain-specific body weight at sexual maturity [SRC-012].

**Evidence assessment:** Strong evidence that maturity occurs in this broad age region; weak evidence for any single universal minimum age.

### 2.2 Operational breeding readiness

Sexual maturity does not automatically mean a bird should enter commercial breeding immediately. Operational readiness can depend on:

- body development and weight,
- health and body condition,
- absence of obvious defects,
- known sex,
- desired strain/pedigree,
- availability of a compatible mate,
- housing/nest capacity,
- farm replacement strategy.

No reviewed source establishes one universal commercial admission rule. This remains partly **Requires Field Validation** for the Egyptian target market.

### 2.3 Selection of breeding stock

Research herds commonly select healthy birds of known strain and suitable age/weight. Commercial farms may additionally select replacements from productive parents or based on growth/reproductive traits, but the exact policy varies and must not be inferred as universal.

---

## 3. Pair Formation

### 3.1 Natural pairing

Pigeons naturally form persistent male–female pair bonds. Courtship behavior precedes mating and coordinated nesting. In communal systems the birds may exercise more mate choice; in controlled breeding the producer may deliberately place a selected male and female together [SRC-004].

### 3.2 Controlled / forced pairing

The literature and breeder terminology use controlled pairing and sometimes “forced pairing” for deliberate mate assignment. Operationally this can involve temporarily confining the selected birds together until acceptance is observed. The exact duration and method are not standardized across the sources reviewed.

### 3.3 Observable acceptance indicators

Farm-observable signs can include:

- reduced aggression,
- mutual proximity,
- courtship displays,
- billing/contact,
- joint occupation or defense of a nesting site,
- mating/copulation,
- nest-building behavior.

### 3.4 Pairing failure

Potential operational outcomes include continued aggression, avoidance, failure to mate, failure to occupy a nest, or persistent infertility after apparent pairing. The decision to wait, separate, or attempt a new pairing is a producer rule and requires field validation.

---

## 4. Pair Stability and Re-pairing

Domestic pigeons show strong monogamous/pair-fidelity behavior and coordinated biparental care [SRC-004]. This does not mean pair membership is biologically immutable.

Re-pairing may occur after:

- mate death,
- deliberate separation,
- poor reproductive performance,
- infertility attributed to one bird,
- health/culling decision,
- loss of pair compatibility.

The operational consequence can include a temporary production interruption while a new social bond and reproductive rhythm establish. No robust universal “re-pairing delay” was found.

In colony housing, social interaction and nest competition can complicate certainty about mate identity and nest ownership compared with individually housed pairs.

---

## 5. Courtship, Mating and Pre-laying Events

A simplified behavioral sequence supported by breeding-cycle literature is:

1. courtship,
2. mate acceptance/pair bond,
3. nest-site selection,
4. nest construction/material carrying,
5. mating/copulation,
6. increased nest attendance,
7. first egg laying.

These are useful **real-world observable farm events**. They are not guaranteed to occur as perfectly separated stages and should not be treated as software statuses.

---

## 6. Nest Preparation and Nest Ownership

Pairs select and defend nesting locations. Nest material may be provided by the producer, while the birds arrange it. In pair cages, nest ownership is operationally clearer because the housing constrains access. In colony/loft systems, competition, intrusion, nest switching, and uncertain parentage can occur more readily.

A second nest is important in many controlled/intensive systems because the female may begin another clutch while previous squabs are still being reared [SRC-001, SRC-002, SRC-005].

**Domain conclusion:** “pair has a nest” is not always equivalent to “pair has exactly one permanent nest for life.” The relationship depends on housing and active reproductive stage.

---

## 7. Egg Laying

### 7.1 First and second egg

The dominant domestic-pigeon pattern is a two-egg clutch. Reviews describe the two eggs as usually laid within roughly 48 hours; a 2026 Poultry Science study of 900 breeding pairs reported a stable two-day oviposition interval across 1–3-year-old breeders [SRC-004, SRC-016].

### 7.2 Important event distinction

The following must remain conceptually separate:

- **Egg laid:** one egg has physically appeared.
- **Clutch complete:** the laying episode has reached its final egg.
- **Incubation started:** sustained parental incubation behavior has begun.

Parents may show some sitting after the first egg, but full incubation behavior and the timing used for hatch prediction may align more closely with clutch completion/consistent incubation. Sources vary in wording; therefore hatch prediction should preserve the farm's observed incubation basis rather than blindly count from first egg.

### 7.3 Exceptional clutch sizes

Two eggs are dominant, but one-egg clutches and uncommon larger/abnormal situations can occur. A one-egg laying episode is still biologically a clutch if it represents the completed laying episode for that reproductive attempt; “clutch” is not defined by requiring two surviving eggs.

---

## 8. Domain Definition of Clutch

**Clutch:** the eggs produced by one female as one discrete laying episode before the next reproductive laying interval.

Operational consequences:

- an egg belongs to the laying episode from the moment it is laid;
- the clutch may later contain only one surviving egg even if two were originally laid;
- loss of Egg 1 before Egg 2 does not mean Egg 1 never belonged to that clutch;
- a naturally completed one-egg episode can still be described as a one-egg clutch;
- clutch outcome and individual egg outcome are different concepts.

A clutch can therefore be reproductively unsuccessful even when its eggs have different outcomes.

---

## 9. Incubation

### 9.1 Duration

Across reviewed domestic-pigeon sources, incubation is commonly around **17–20 days**, with ~18 days frequently reported [SRC-001, SRC-004, SRC-005, SRC-017]. Egyptian strain work reported hatching time around 17.7–18.0 days across Local Egyptian, Zagel and White Mirthys groups [SRC-012].

### 9.2 Biparental incubation

Both parents incubate. Review literature describes a characteristic division in which the male commonly takes a daytime/noon shift and the female covers much of the remainder [SRC-004]. Exact clock times are not universal farm rules.

### 9.3 What date should incubation be counted from?

Sources often state “18 days incubation” without using one identical operational anchor. Because two eggs are separated by approximately two days and incubation intensity may change across laying, counting from first egg, second egg, or confirmed sustained incubation can produce different hatch expectations.

**Domain recommendation for later field study:** record what actually happened (egg dates and observed incubation) rather than forcing a single theoretical start date.

---

## 10. Fertility Checking / Candling

Manual candling is a real method used to evaluate pigeon egg development. Engineering research on pigeon eggs notes that practical fertility information is commonly visually available around **days 5–7 of incubation**, and traditional manual candling remains a reference method [SRC-018].

Candling can reveal:

- vascular/embryonic development consistent with fertility,
- apparently clear/undeveloped eggs,
- early embryonic death patterns such as a blood ring in avian eggs.

Benefits include earlier recognition of non-developing eggs and improved reproductive diagnosis. Risks include excessive handling, breakage, chilling, and disturbance if performed poorly.

**Scientific recommendation vs farm practice:** scientific feasibility is established; routine use, exact day, frequency, and whether every Egyptian farm candles eggs remain **Field Validation Required**.

---

## 11. Egg Outcomes

Real biological/operational egg outcomes found or supported by avian/pigeon reproduction literature include:

- fertile and developing,
- infertile / no embryo development,
- embryonic death (early, mid, or late),
- dead-in-shell / failed hatch,
- cracked,
- broken,
- lost/missing/displaced,
- abandoned/not adequately incubated,
- removed/transferred/fostered,
- successfully hatched,
- unknown/unverified outcome.

These labels describe observed outcomes; they are not proposed software enums.

---

## 12. Hatching

Expected hatch is commonly near the end of the ~17–20-day incubation range. The two eggs do not have to hatch at exactly the same moment. Differences in laying order and onset/intensity of incubation can create a hatch interval and size difference between siblings.

Possible hatch problems include:

- embryo dies before pipping,
- pipping without successful emergence,
- prolonged hatch,
- weak hatchling,
- shell/membrane problems,
- egg damaged before hatch.

Routine manual hatch assistance is not established as a universal best practice in the reviewed commercial evidence. Intervention can help selected cases but can also harm a viable embryo if done at the wrong time. It should remain a specialist husbandry decision rather than a default workflow.

---

## 13. Squab Early Life

Newly hatched squabs are altricial, poorly independent, nest-bound, and heavily reliant on parents for warmth and nutrition. Both parents produce crop milk [SRC-003, SRC-004].

A useful evidence-based nutritional progression is:

- **approximately days 0–3:** crop milk is dominant/sole feed in review descriptions;
- **first week:** crop milk remains central;
- **after the first several days:** regurgitated grain/feed is progressively mixed with crop milk;
- **toward 3–4 weeks:** natural squabs become increasingly able to eat independently [SRC-003, SRC-006, SRC-021].

The first two weeks show very rapid weight gain in Egyptian strain studies [SRC-012].

Farm-observable priorities include:

- hatch presence and vitality,
- crop filling/feeding evidence,
- warmth and parental attendance,
- visible injury/deformity,
- growth/weight trend where weighing is practiced,
- sibling size imbalance,
- disappearance/death,
- nest hygiene and disturbance.

---

## 14. Growth Stages — Domain-oriented View

The literature more often reports age and growth measurements than a single standardized commercial stage vocabulary. Therefore the following are **descriptive age landmarks**, not standardized statuses:

| Age region | Observable development / production meaning | Evidence |
|---|---|---|
| Hatch / Day 0 | highly dependent, crop-milk feeding begins | Strong |
| Days 1–7 | fastest early growth region; crop milk central | Strong |
| Days 7–14 | rapid growth continues; increasing mixed parental feed | Strong |
| Days 14–21 | feather development and body mass continue; still parent dependent | Strong |
| Days 21–28 | pre-weaning/market region in many meat systems | Strong for broad region |
| ~28 d onward | many squabs can increasingly feed independently; traditional separation/market common | Strong but management dependent |

Egyptian 2022/2023 data demonstrate major strain differences at 28 days: Local Egyptian approximately low-300 g region, Zagel around ~400 g, and White Mirthys around ~500 g in the studied population [SRC-012]. These are research observations, **not market specifications**.

---

## 15. Weaning

### 15.1 Traditional parent-reared system

In traditional squab production, the bird is typically marketed or separated near the end of the parental rearing period, often around 3–4 weeks. Consequently, **market age and true physiological independence are close but not guaranteed to be identical**.

A squab can be sold as a meat bird before it would be managed as a fully independent replacement pigeon.

### 15.2 Early-weaning systems

Early separation is a specialized/intensive intervention. Egyptian commercial-farm research compared separation at hatch, 7 days, and 28 days in White Mirthys pairs [SRC-002]. Early separation can shorten the interval to the next laying and increase reproductive throughput of parents, but growth, labor requirements, artificial feeding reliability, mortality and welfare risk change substantially.

Therefore:

**Early weaning is not merely “selling earlier.” It creates a different rearing pathway.**

---

## 16. Market Readiness

No universal market-ready rule was found.

Relevant dimensions include:

- age,
- live weight or dressed weight,
- strain,
- feathering/appearance,
- buyer preference,
- whether sold live or processed,
- local culinary preference,
- season and growth rate.

The frequently cited 21–28-day region is a useful production reference, but it should not be converted into a hard commercial rule without Egyptian field validation.

**Market Age ≠ Weaning Age in all systems.**

---

## 17. Parent–Squab Relationship

Both parents normally feed and care for squabs. Parent-loss research in Egyptian Baladi pigeons confirms that removal/loss of one or both parents changes growth/welfare outcomes and may require management intervention [SRC-005].

Potential real-world responses include:

- remaining parent continues care,
- fostering to another pair,
- hand/artificial feeding,
- transfer of egg/squab to synchronized foster parents,
- loss of the squab if adequate care is not provided.

Fostering and egg transfer are known pigeon husbandry techniques [SRC-005, SRC-017], but current prevalence in Egyptian meat farms requires validation.

---

## 18. Next Clutch

This is the central reason pigeon production should not be modeled mentally as a simple serial cycle.

The female may begin the next laying episode while the previous brood is still dependent. In natural systems the hatch-to-next-lay interval can be around several weeks and varies strongly by strain and management. Egyptian strain data reported approximately **19.5 days after hatch for White Mirthys** versus about **31 days for Local Egyptian/Zagel** in the cited study population [SRC-012]. A recent Egyptian early-weaning experiment demonstrated that removal of squabs can markedly shorten the return to laying [SRC-002].

Thus a pair can simultaneously be:

- parenting squabs from Clutch A,
- occupying/preparing another nest,
- laying or incubating Clutch B.

---

## 19. Overlapping Production Cycles — Deep Analysis

### 19.1 Biological reality

Overlap is supported by FAO husbandry descriptions, double-nest systems, Egyptian studies, and measured hatch-to-next-lay intervals [SRC-001, SRC-002, SRC-005, SRC-012].

### 19.2 Reference example — natural/parent-reared pathway

This example uses evidence-based ranges rather than one universal schedule:

- **Day 0:** first egg of Cycle A observed.
- **~Day 2:** second egg / typical clutch completion.
- **~Day 17–20 from effective incubation:** Cycle A hatches.
- **Hatch + ~19–31 days in Egyptian strain data:** next laying may occur depending on strain/management.
- Meanwhile Cycle A squabs may remain with parents through roughly 21–28+ days.

Therefore, under shorter hatch-to-next-lay intervals, **Cycle B eggs can appear while Cycle A squabs are still in the nest**.

### 19.3 Double-nest function

A second nesting site separates functions:

- Nest 1: older squabs from Cycle A.
- Nest 2: new eggs / incubation for Cycle B.

This reduces physical conflict between brooding older squabs and incubating a new clutch and supports continuous output.

### 19.4 Early-separation pathway

If squabs are removed at hatch or at 7 days, parental-care load changes and return to laying may be earlier [SRC-002]. The biological reproductive chain is therefore modified by management intervention.

### 19.5 Domain implication

There is no safe assumption that “pair has only one active production cycle.” At minimum, real-world analysis must tolerate contemporaneous parental care for one brood and reproductive activity for the next.

---

## 20. Failed Cycle Scenarios

A reproductive attempt can fail at different points:

1. pairing/courtship failure,
2. mating without laying,
3. one-egg or abnormal laying episode,
4. infertile clutch,
5. egg breakage/loss,
6. embryonic death,
7. hatch failure / dead-in-shell,
8. hatch followed by early squab death,
9. parental abandonment,
10. mate loss or illness,
11. management removal/transfer.

The response to failure is not uniform. If eggs are lost/removed, pigeons may return to laying sooner than if they complete incubation and rear squabs. Classical pigeon husbandry literature notes that egg removal can accelerate repeat laying [SRC-017].

A failed cycle therefore does **not** necessarily consume the same time as a successful parent-reared cycle.

---

## 21. Production Reset / What Counts as a New Cycle?

The industry/research literature uses several valid anchors depending on purpose:

- **Pairing cycle:** begins when a new pair is formed.
- **Egg-laying cycle:** often measured from one laying event/clutch to the next.
- **Clutch:** begins with the first egg of a laying episode.
- **Incubation period:** begins from effective incubation/set date.
- **Brooding/rearing period:** begins at hatch.
- **Reproductive cycle:** may be defined by study authors from laying-to-laying or through hatch-to-next-lay components.

**Conclusion:** there is no single universal domain definition suitable for every measurement purpose. Phase 3 must choose analytical definitions explicitly without erasing the underlying events.

---

## 22. Continuous Squab Production

Farm-level continuity is achieved by combining many asynchronous biological units:

- multiple pairs at different reproductive stages,
- repeated clutches,
- overlapping brooding and next-clutch activity,
- double nests where used,
- replacement breeders entering production,
- removal/culling of poor performers,
- environmental and nutritional management,
- sometimes artificial incubation or early separation in intensive systems.

Thus “continuous production” is a **population scheduling effect**, not one pair producing a saleable squab every day.

---

## 23. Reproductive Interruptions

Factors documented or strongly supported as capable of delaying/reducing reproduction include:

- heat stress,
- illness,
- poor body condition,
- inadequate nutrition,
- pair incompatibility,
- infertility,
- mate loss,
- nest disturbance/competition,
- environmental stress,
- molt-related resource allocation,
- deliberate management separation or culling.

The magnitude of each effect depends on housing, season, strain and farm management.

---

## 24. Molting

Pigeons undergo an annual molt rhythm, but breeding and molt can overlap. Historical work specifically on pigeons reports that females can lay during the molting period and that molt may pause/interact with reproductive activity [SRC-019]. Modern feral-pigeon work also documents an annual molt cycle [SRC-020].

Therefore the evidence does **not** support treating molt as an automatic total production shutdown for all domestic meat pigeons.

More accurate wording:

**Molt can compete with reproduction for physiological resources and may coincide with reduced performance, but its operational effect varies and requires local validation.**

---

## 25. Reference Production Timeline

> The table is a reference map. It is not a farm standard or future software schedule.

| Event | Typical Timing | Possible Range / Variation | Dependencies | Evidence Level | Source |
|---|---|---|---|---|---|
| Sexual maturity | ~6–7 months | approx. 5–7+ months depending on strain/definition | strain, growth, condition | Strong | SRC-003, SRC-012, SRC-017 |
| Pair formation | before laying | variable; no universal duration | mate acceptance, housing | Moderate | SRC-004 |
| Nest/courtship activity | before first egg | variable | pairing, nest access | Strong biologically | SRC-004 |
| First egg | Day 0 reference | — | successful pairing/reproduction | Strong | SRC-004 |
| Second egg | ~2 days after Egg 1 | commonly within ~48 h | normal laying rhythm | Strong | SRC-004, SRC-016 |
| Effective incubation | around clutch laying/completion | anchor differs by source/observation | sitting behavior | Strong process / Moderate anchor | SRC-004 |
| Candling | commonly ~day 5–7 of incubation where practiced | farm method varies | handling, egg visibility | Moderate–Strong | SRC-018 |
| Hatch | ~17–20 d incubation | strain/anchor/environment dependent | fertile viable embryo | Strong | SRC-001, SRC-005, SRC-012 |
| Crop-milk dominant feeding | first days / first week | review descriptions vary | parent condition | Strong | SRC-003, SRC-021 |
| Rapid squab growth | 0–14 d especially | strain-specific | crop milk/feed, brood size | Strong | SRC-012 |
| Traditional market/weaning region | ~21–28 d | sometimes 25–32 d to leave nest; market varies | strain, buyer, production system | Strong broad range | SRC-001, SRC-002, SRC-005 |
| Next laying after hatch | about ~19–31 d in cited Egyptian strain data | can be much earlier with early separation | strain, parental load, management | Strong variability | SRC-002, SRC-012 |
| Next clutch while previous squabs remain | possible/common in managed systems | depends on interval and nest system | double nest, pair condition | Strong | SRC-001, SRC-005, SRC-012 |

---

## 26. Observable Real-world Farm Events

Events a worker/manager can potentially observe include:

- replacement bird admitted to breeder group,
- proposed pair placed together,
- pair acceptance observed,
- pair aggression/incompatibility observed,
- mating observed,
- nest selected/occupied,
- nest material carried/building observed,
- first egg found,
- second egg found,
- one-egg clutch remains incomplete/ends,
- egg cracked/broken/missing,
- incubation observed,
- candling performed,
- fertile development observed,
- infertility suspected/confirmed,
- embryonic death suspected,
- hatch observed,
- hatch failure/dead-in-shell observed,
- squab crop appears fed/empty,
- squab weighed,
- poor growth observed,
- squab injured/missing/dead,
- foster transfer performed,
- parent lost/died,
- remaining parent continues/fails care,
- squab separated/weaned,
- squab marketed,
- new nest occupied while older squabs remain,
- next clutch begins,
- pair separated/re-paired,
- breeder culled/retired.

These are **farm observations**, not software Domain Events.

---

## 27. Exceptions & Non-standard Scenarios

Supported or biologically credible scenarios that must not be erased by a “perfect” lifecycle narrative include:

- one-egg clutch,
- uncommon clutch-size deviation,
- egg broken or missing before clutch completion,
- egg laid outside intended nest,
- nest switching or competition in communal housing,
- uncertain parentage in colony systems,
- abandoned egg/nest,
- fostered egg,
- fostered squab,
- one parent dies,
- both parents lost,
- pair separation,
- aggression/incompatibility,
- infertile eggs,
- embryonic death,
- asynchronous hatch,
- only one squab survives,
- early artificial separation,
- artificial incubation/feeding where practiced.

Some producer-reported scenarios such as two females sharing a nest or egg stealing are plausible/known pigeon behaviors but were not supported strongly enough in the reviewed commercial evidence to define as standard lifecycle branches; they should remain Field Validation items if important to the target farms.

---

## 28. Egyptian Production Timeline Findings

Egyptian evidence provides unusually useful lifecycle context:

### 28.1 Growth

Research on Local Egyptian, Zagel and White Mirthys pigeons measured hatch, 7-, 14-, 21-, and 28-day weights. White Mirthys showed substantially higher later body weight than Local Egyptian under the study conditions [SRC-012].

### 28.2 Incubation

The same Egyptian strain research reported hatching time around **17.7–18.0 days**, consistent with international literature [SRC-012].

### 28.3 Hatch-to-next-lay interval

Reported values differed strongly by strain: about **19.5 days in White Mirthys** and roughly **31 days in Local Egyptian/Zagel** in that study [SRC-012]. This is direct evidence that overlap intensity can differ by genetics/production type.

### 28.4 Early weaning

A 2025 commercial-farm study on the Cairo–Alexandria Desert Road demonstrated that separation at hatch or 7 days changes reproductive timing and squab performance relative to conventional 28-day separation [SRC-002].

### 28.5 Market weight

Egyptian research provides 28-day live-weight observations but does **not** prove one national market specification. Market age/weight remains an open field-validation item.

### 28.6 Summer

Existing Egyptian heat-stress findings from Phase 1A remain relevant: summer heat can reduce reproductive performance, but the magnitude cannot be inserted into the lifecycle as a fixed seasonal pause.

---

## 29. Lifecycle Evidence Conflicts

### LC-CON-001 — Sexual maturity vs breeding readiness
- **Source A:** reviews commonly place maturity around 6–7 months.
- **Source B:** Egyptian research uses/observes strain-specific maturity age and body weight.
- **Difference:** biological maturity does not define a universal farm admission threshold.
- **Likely explanation:** genetics, growth, sex, body condition and management.
- **Impact later:** avoid one hard-coded breeder-entry age.

### LC-CON-002 — Incubation start anchor
- **Source A:** general literature states ~18 days incubation.
- **Source B:** laying occurs over ~48 h and parental sitting behavior changes around clutch completion.
- **Difference:** “18 days from what exact timestamp?” is often unstated.
- **Likely explanation:** biological incubation is gradual while research/farm records use simplified anchors.
- **Impact later:** preserve egg dates and hatch dates before choosing derived calculations.

### LC-CON-003 — Natural weaning vs market age
- **Source A:** traditional literature places weaning/market around 3–4 weeks.
- **Source B:** early-weaning systems separate at 0–7 days while artificial feeding continues.
- **Difference:** separation age, physiological independence, and slaughter/market age are not the same concept.
- **Impact later:** do not merge them.

### LC-CON-004 — Hatch-to-next-lay / cycle length
- **Source A:** Egyptian Local/Zagel data show longer intervals.
- **Source B:** White Mirthys and early-separation systems show much shorter intervals.
- **Difference:** major variation in cycle timing.
- **Likely explanation:** breed, parental rearing load and management intervention.
- **Impact later:** production cycle must be event-based and context-aware, not a universal duration.

### LC-CON-005 — Molt and reproductive interruption
- **Source A:** molt is an annual physiological process.
- **Source B:** pigeons can continue breeding during molt and molt itself may pause around reproduction.
- **Difference:** molt does not equal mandatory reproductive shutdown.
- **Impact later:** treat molt as a performance/context factor unless farm evidence establishes stronger operational rules.

---

## 30. Field Validation Required

1. At what age/weight do target Egyptian farms actually admit males and females to breeding?
2. How long do controlled pairings usually take before acceptance or rejection?
3. What observable criteria define successful pair formation locally?
4. Do farms record Egg 1 and Egg 2 dates separately?
5. What date do farmers use when predicting hatch: first egg, second egg, or another convention?
6. Is candling routine, occasional, or absent? On which day?
7. How are infertile/dead-in-shell/missing eggs recorded in practice?
8. Is double nesting used routinely, and in which housing systems?
9. What is the actual hatch-to-next-lay interval by common Egyptian strain and season?
10. What defines a market-ready squab for each buyer type?
11. Is sale normally before, at, or after true feeding independence?
12. How common are fostering and egg/squab transfer?
13. What procedure is used after one-parent loss?
14. What thresholds cause re-pairing or breeder removal?
15. How does molt affect production in real commercial Egyptian farms?
16. How common are early separation/artificial feeding systems outside specialized farms?

---

## 31. Phase 1B Domain Conclusions

1. The production lifecycle is event-rich and partially overlapping, not a simple state chain.
2. Pairing, egg laying, clutch completion, incubation, hatch, rearing, market readiness, and next laying are distinct operational concepts.
3. Two eggs and ~18-day incubation are strong baseline biological patterns, but exceptions and anchor ambiguity matter.
4. Natural parent rearing creates a direct dependency between breeder condition and squab outcome.
5. The next clutch can start before the previous squabs leave, especially in faster strains/management systems.
6. Double nests are an operational mechanism supporting overlap.
7. Early separation creates a materially different lifecycle pathway, not merely a shorter version of the traditional one.
8. Failed cycles can restart sooner than successful full parent-reared cycles.
9. “Production cycle” has several legitimate measurement definitions; the future system must not choose one implicitly.
10. Egyptian evidence confirms both international biological patterns and meaningful strain/management differences.

---

## 32. Source Register — New / Expanded Phase 1B Sources

> Phase 1B reuses Phase 1A sources `SRC-001` through `SRC-015` where cited. Access date for new sources: **2026-08-17**.

### SRC-016
- **Source:** Age-related dynamics of reproductive performance and egg quality in breeding pigeons
- **URL:** https://www.sciencedirect.com/science/article/pii/S0032579126006498
- **Organization / Author:** Poultry Science
- **Publication Date:** 2026
- **Reliability:** High — peer reviewed
- **Information Used:** stable two-egg clutch, approximately two-day oviposition interval, breeder-age context.

### SRC-017
- **Source:** Pigeonetics takes flight: evolution, development, and genetics of intraspecific variation
- **URL:** https://pmc.ncbi.nlm.nih.gov/articles/PMC5521274/
- **Organization / Author:** Genetics Society of America review
- **Publication Date:** 2017
- **Reliability:** High for general domestic-pigeon reproductive biology
- **Information Used:** two-egg clutch, 17–19-day incubation, biparental care, 3–4-week weaning, ~6-month maturity, foster/egg-removal husbandry context.

### SRC-018
- **Source:** Early-stage fertilization detection in pigeon eggs during incubation using improved lightweight model
- **URL:** https://www.sciencedirect.com/science/article/pii/S0168169923008104
- **Organization / Author:** Computers and Electronics in Agriculture
- **Publication Date:** 2024
- **Reliability:** High for pigeon-egg candling/fertility-detection context
- **Information Used:** manual candling as practical reference method; fertility information typically visible around incubation days 5–7.

### SRC-019
- **Source:** Molting of pigeon in relation to reproductive cycle
- **URL:** https://cir.nii.ac.jp/crid/2050870367028374528
- **Organization / Author:** Zoological Society of Japan archive
- **Publication Date:** 1949
- **Reliability:** Medium — direct pigeon study but historical
- **Information Used:** coexistence/interactions of molt and reproduction; molt interruption around breeding.

### SRC-020
- **Source:** Grooming time parallels molt intensity in wild-caught feral rock pigeons
- **URL:** https://nsojournals.onlinelibrary.wiley.com/doi/full/10.1002/jav.03489
- **Organization / Author:** Journal of Avian Biology
- **Publication Date:** 2025
- **Reliability:** High for molt phenology; feral rather than meat-farm context
- **Information Used:** annual rock-pigeon molt cycle and feather-replacement timing.

### SRC-021
- **Source:** Exploration of Proteomics Analysis of Crop Milk in Pigeons during the Lactation Period
- **URL:** https://pmc.ncbi.nlm.nih.gov/articles/PMC8552352/
- **Organization / Author:** ACS Omega / peer-reviewed research
- **Publication Date:** 2021
- **Reliability:** High
- **Information Used:** crop milk dominance in early squab life, transition to mixed parental feed through the rearing period.

---

## 33. Scope Boundary / Next Research

Phase 1B intentionally does not define:

- database representation of bird/pair/clutch/egg/squab,
- lifecycle status enums,
- system Domain Events,
- KPIs or alert rules,
- UI workflows,
- Laravel architecture,
- MVP features.

Those decisions must wait for the appropriate later phases.

**Next recommended step after review:** Phase 1C — Domain Terminology, Evidence Consolidation & Validation Review.
