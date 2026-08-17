# Commercial Pigeon Farming — Domain Research

> **Phase:** 1A — Commercial Pigeon Farming Domain Research  
> **Status:** Completed — Awaiting Review  
> **Scope:** Commercial Meat Pigeon / Squab Production  
> **Research date:** 2026-08-17  
> **Important:** This document describes the biological and operational domain. It intentionally does **not** define software entities, database tables, APIs, UI, or architecture.

---

## 1. Executive Domain Summary

Commercial squab production is a meat-production system built around **breeding pigeon pairs that repeatedly produce and rear young squabs**. It differs materially from conventional broiler production because the market bird is not normally produced as an independent chick placed into a grow-out flock and fed directly from a feeder from hatch. The young pigeon is an **altricial** bird and, under natural production, depends heavily on both parents for brooding and feeding, initially through crop milk and later through regurgitated feed [SRC-003, SRC-004].

The dominant natural reproductive pattern is a male–female breeding pair, usually two eggs per clutch, about 18 days of incubation, followed by parental rearing of the squabs. The traditional market/weaning window is commonly around **3–4 weeks / approximately 21–28 days**, with several sources describing collection or market at about four weeks, often before full independent flight [SRC-001, SRC-002, SRC-005]. This is not a universal specification: market age and weight vary with breed, management, buyer specification, early-weaning technology, and production objective.

A crucial operational characteristic is that pigeon production can have **overlapping reproductive activity**. A female may begin the next clutch while the pair is still caring for squabs from the previous one. This is why two-nest arrangements appear repeatedly in technical literature and intensive production descriptions [SRC-001, SRC-005]. For domain analysis, this means a “production cycle” is not safely assumed to be a simple non-overlapping block.

The commercial unit can be organized in several ways: communal loft/dovecote systems, colony/fly-pen systems, or individually housed breeding pairs in numbered cages. Egyptian field research identified commercial systems based on **mud dovecotes** and **wooden lofts**, while experimental/commercial studies in Egypt and elsewhere also use individual pair cages [SRC-002, SRC-007, SRC-008]. These systems differ substantially in control of mating, identification, pedigree certainty, nest ownership, record accuracy, labor, welfare considerations, and output measurability.

**Domain conclusion:** the management problem is not merely “count pigeons.” It is the management of a living breeding population in which pair bonds, nest access, eggs, parental care, overlapping cycles, replacement, environment, health, records, and market timing interact.

---

# 2. Commercial Squab Farming Overview

## 2.1 What is Commercial Squab Production?

Commercial squab production is the organized breeding and management of domestic pigeons primarily to produce young pigeons for meat. The commercial objective is repeatable saleable output from breeding stock rather than maintenance of birds for exhibition, racing, hobby, or ornamental traits.

Egyptian socio-economic research separated pigeon production according to both **purpose** and **housing system**. In the surveyed Sharqia sample, family systems were primarily oriented toward household consumption with surplus sales, while most operators in the commercial mud-dovecote and wooden-loft groups reported income generation as the primary objective [SRC-007].

**Evidence classification:** Verified Fact for the cited Egyptian survey; broader classification should be treated as a useful domain framing rather than a universal global taxonomy.

## 2.2 Commercial production vs hobby keeping

The biological bird is the same, but the management objective changes.

| Dimension | Commercial meat/squab production | Hobby / ornamental / racing context |
|---|---|---|
| Primary objective | Repeatable marketable squab output and economic return | Appearance, performance, companionship, breed preservation, racing, exhibition, etc. |
| Breeding decisions | Productivity, fertility, hatchability, growth, parental ability, replacement value | May prioritize lineage, color, conformation, flight/racing traits, rarity, or personal preference |
| Record pressure | Production and cost records become economically important | Record detail varies widely by hobby objective |
| Housing | Selected for control, output, labor, hygiene, and economics | May prioritize flight access, aesthetics, tradition, or sport requirements |
| Pair evaluation | Usually has a production/economic dimension | May emphasize genetic or exhibition goals instead of meat output |
| Market bird | Squab / meat pigeon | Often not the primary output |

This distinction does **not** mean commercial farms are identical. Commercial production ranges from relatively traditional dovecote/loft systems to highly controlled pair-cage systems and industrial techniques including artificial incubation or early feeding [SRC-002, SRC-005, SRC-007].

## 2.3 Primary product

The primary product in the scope of this project is the **squab**: a young pigeon produced for meat before or around the time of weaning/independent flight, depending on the production system and market specification [SRC-001, SRC-003].

Breeding pigeons are the productive stock that generates this output. Eggs, culled breeders, manure, or breeding-stock sales may have value in some businesses, but they are not assumed to be the core product of this study without field validation.

## 2.4 Typical market/weaning age

The strongest recurring domain range in the reviewed sources is approximately **21–28 days**, with many commercial/natural-rearing studies evaluating squabs at 28 days. FAO describes collection at about four weeks, while a recent Egyptian commercial-farm study treats 28-day parent rearing as the conventional control and describes natural weaning as generally 21–28 days [SRC-001, SRC-002]. An Egyptian Baladi study describes squabs leaving the nest around 25–32 days [SRC-005].

### Why market around this stage?

The sources support several linked reasons:

1. Squabs grow very rapidly during the parental-feeding phase [SRC-003, SRC-004].
2. Around this period they approach mature body weight in some production strains [SRC-003].
3. Traditional squab production markets the bird while still young and tender and often before full independent flight [SRC-001].
4. Continuing parental care longer can delay or interact with the parents’ next reproductive effort; intensive systems therefore experiment with earlier separation to increase breeder reproductive throughput [SRC-002].

**Do not convert 28 days into a universal business rule.** Buyer specification, breed, body weight, welfare, hand-feeding practice, and market culture require validation.

## 2.5 Why the production cycle differs from broiler production

Pigeon production differs from a broiler flow in several biologically important ways:

- The squab is **altricial/superaltricial**, not independently feeding immediately after hatch [SRC-002, SRC-003].
- Both parents produce crop milk and participate in feeding young [SRC-003, SRC-004].
- Both parents share incubation [SRC-001, SRC-005].
- The breeding pair remains an active production resource across repeated clutches, rather than being only the genetic source of a separately managed batch.
- Parent reproductive condition and parental care directly influence squab performance.
- New egg laying can overlap with care of the previous squabs [SRC-001, SRC-005].
- Artificial incubation/early-weaning strategies can change reproductive throughput but also change growth, labor, mortality risk, and management complexity [SRC-002].

These biological facts are central to later analysis but are **not yet software design decisions**.

---

# 3. Commercial Production Models

No single source provides a universally accepted taxonomy covering every farm. The reviewed literature instead describes real systems by **housing**, **pair control**, **intensity**, and **rearing technology**.

## 3.1 Communal loft / dovecote / colony systems

Birds live and breed in a shared structure with multiple nesting sites. Egyptian field work identified mud dovecotes and wooden lofts as two commercial sub-systems in the studied Sharqia region [SRC-007]. Communal fly-pens are also documented in comparative production research [SRC-008].

### Operational characteristics

- Birds share a larger housing environment.
- Pairing may arise naturally and may be less directly controlled than in individual pair cages.
- Nest ownership and nest disputes require observation and suitable nest availability.
- Individual parentage and production attribution can be more difficult if individual identification and nest control are weak.
- Location-based management (loft, section, nest) can become operationally important.

### Advantages

- Can align with traditional/local management practices.
- Potentially simpler housing per bird and more behavioral freedom depending on design.
- Existing breeder knowledge and local materials may support adoption.

### Disadvantages / management challenges

- Harder attribution of eggs/squabs to specific pairs in poorly controlled colonies.
- Greater risk of nest competition, mislaid eggs, or uncertain parentage where identification is weak.
- Record keeping at individual-pair level can become labor-intensive.
- Performance differences between pairs may be hidden by group averages.

### Commercial suitability

Potentially commercial, as demonstrated by Egyptian mud-dovecote and wooden-loft enterprises [SRC-007]. Suitability depends on market, labor, biosecurity, housing quality, ability to identify productive units, and required data precision.

## 3.2 Individual breeding-pair cage system

A known male and female are housed as a controlled breeding unit, usually with numbered cages and dedicated nests. Recent Egyptian research on a commercial farm used individual numbered metal cages for each pair, and an Egyptian Baladi study used pair-based cage units [SRC-002, SRC-005].

### Operational characteristics

- Pair identity is controlled.
- Eggs and squabs can be attributed to a known pair with higher confidence.
- Feed, production, fertility, hatchability, and squab output can be measured at pair level more easily.
- Pair-specific culling or replacement decisions become easier to support with records.
- The cage itself often functions as a location identifier.

### Comparative evidence

Older Philippine research comparing paired cages with communal fly-pens reported more eggs and more squabs from caged pairs, with better feed efficiency/profitability under the conditions studied [SRC-008]. This is useful evidence that housing/control can influence measurable performance, but it is **not sufficient to declare cages universally superior** across welfare, climate, breed, capital, labor, and market contexts.

## 3.3 Intensive systems with artificial incubation / early rearing

Modern intensive research describes systems where eggs may be artificially incubated or squabs separated early and hand-fed/artificially fed to shorten the parent reproductive interval [SRC-002, SRC-004]. Some industrial systems also transfer squabs among foster parents so one pair feeds more than the natural two [SRC-004, SRC-013].

### Benefits under research conditions

- Can increase egg output and reproductive throughput of breeding pairs.
- Can decouple some parental-care time from the next laying cycle.

### Costs and risks

- Requires much more controlled management and labor/technology.
- Early separation can reduce growth and increase mortality if feeding/brooding is not well managed. In the 2025 Egyptian commercial-farm experiment, separation at hatch had substantially worse squab mortality and lower 28-day weight than parent rearing, despite higher parent reproductive output [SRC-002].
- Artificial feeding introduces new process-control and hygiene risks.

**Phase 1A conclusion:** “intensive” should not be used as a single housing label. Intensity can refer to controlled pairs, artificial lighting, artificial incubation, early feeding, foster rearing, feed formulation, or combinations of these.

---

# 4. Farm Population Structure

The research supports a population that is operationally heterogeneous rather than a single undifferentiated flock.

## 4.1 Core categories observed or implied in real operations

### Breeding adults

Sexually mature males and females used for reproduction. In controlled systems they are commonly organized into breeding pairs [SRC-002, SRC-005].

### Active breeding pairs

Male–female pairs currently functioning as reproductive units. Pair performance can be observed through egg production, fertility, hatchability, squab output, and offspring growth [SRC-002, SRC-014].

### Replacement / pre-breeding birds

Young birds retained to become future breeding stock. Sexual maturity is commonly reported in the approximate 5–7 month region depending on source/breed; the reviewed literature includes about 156 days in one meat-breed study and around seven months in reviews/other studies [SRC-003, SRC-008]. The exact entry criterion into production must not be universalized.

### Squabs

Dependent young birds from hatch through the rearing/weaning/market stage. They require parental or artificial feeding support [SRC-002, SRC-003].

### Growing / young birds retained beyond squab stage

Birds kept after normal meat-market age for replacement, breeding stock, research, or other purposes. Their management is distinct from market squabs because they move toward sexual maturity rather than immediate sale.

### Sick / isolated / quarantine birds

Health literature and basic livestock practice make isolation and health-status separation relevant, but detailed health/quarantine workflows belong to Phase 4. Phase 1A only records that health state can remove birds from normal productive participation.

### Culled / sold / retired / dead birds

These are distinct outcomes and should not be conflated operationally. A bird may leave production because of economic culling, sale as live stock, age/retirement, health removal, or mortality. Detailed criteria require field validation.

## 4.2 Life movement — conceptual, not software statuses

A simplified biological-operational trajectory can be described as:

**Hatch → dependent squab → market bird OR retained young bird → replacement candidate → mature breeder → active breeding pair → continued production → re-pair / removal / sale / cull / retirement / mortality**

Real birds may leave or re-enter productive paths differently. This trajectory is a domain aid only and must not be copied directly into a software state machine.

---

# 5. Breeding Pair as an Operational Unit

## 5.1 Is the pair a basic production unit?

The evidence strongly supports the **breeding pair** as a central operational unit in natural meat-pigeon production.

Reasons include:

- Pigeons form male–female pair bonds and both sexes participate in incubation [SRC-004, SRC-005].
- Both parents produce crop milk and feed squabs [SRC-003].
- Research routinely reports production as eggs, hatchability, feed, or squabs **per pair** [SRC-002, SRC-014].
- Pair-controlled housing allows direct attribution of output to a specific sire–dam combination [SRC-002].

This does **not** prove that every commercial metric or every bird must always be managed only at pair level. Individual identity, flock/location, nest, and squab group also matter.

## 5.2 Pair bond and stability

A 2023 review describes pigeons as non-seasonal breeders that pair as one female and one male with long-term pair bonds, alongside biparental incubation and rearing [SRC-004]. Operationally, this creates persistence: the same male–female combination may produce repeated clutches and can accumulate a meaningful production history.

## 5.3 Biological Pair vs Operational Breeding Pair

**Biological Pair:** the actual bonded male and female participating in courtship, mating, incubation, and/or parental care.

**Operational Breeding Pair:** the male and female that the farm currently treats as a managed productive unit for housing, observation, records, and output evaluation.

In a well-controlled pair-cage system these may normally coincide. In communal systems, re-pairing, uncertain identification, foster rearing, or management intervention may create situations where biological and operational responsibility are not perfectly identical.

## 5.4 Loss of one or both parents

An Egyptian experiment specifically examined parent loss. Squabs can be reared by one remaining parent, foster pigeons, or hand rearing, but performance/welfare differs by method. Both-parent rearing is a meaningful baseline because both parents normally provision young [SRC-005].

Operational implication: parent loss is not simply a “bird missing” event; it can immediately affect dependent squabs and may require a fostering/hand-rearing decision.

## 5.5 Re-pairing and weak pairs

Scientific sources reviewed here establish pair persistence and pair-level production measurement, but they do **not** provide a single validated commercial rule for:

- how long to wait before re-pairing after mate loss,
- the exact production threshold for breaking a pair,
- the number of failed clutches that defines a poor pair,
- whether to replace the male, female, or both when performance is weak.

These require producer/expert validation and later production analysis. They have therefore been added to the Open Questions register.

---

# 6. Nest Management

## 6.1 Nest availability is production infrastructure

Nest management is not decorative. It directly supports courtship, egg laying, incubation, and squab rearing.

Sources describing natural/intensive production repeatedly note the use of **two nests per breeding pair** [SRC-001, SRC-005]. The recent Egyptian commercial-farm experiment used two nests in each individual breeding cage [SRC-002].

## 6.2 Double Nest System

FAO describes intensive females laying the next two eggs while squabs remain in the previous nest, requiring a two-nest structure [SRC-001]. Egyptian research also describes pigeons using two nests alternately for incubation and rearing [SRC-005].

### Operational reason

One nest can contain growing squabs while the second is prepared/used for the next clutch. This reduces direct conflict between the developmental needs of older squabs and new eggs.

## 6.3 Shared or communal nesting challenges

In a communal loft/dovecote, nest identification and ownership are more operationally complex than in a dedicated pair cage. Potential challenges include:

- competition for nest sites,
- uncertain attribution of eggs or squabs if nests/pairs are not controlled,
- disturbances and fights,
- difficulty keeping production records at pair level.

The prevalence and exact handling of these issues in Egyptian commercial wooden-loft and dovecote farms requires field validation.

---

# 7. Overlapping Breeding / Production Cycles

This is one of the most important findings of Phase 1A.

## 7.1 Can a pair rear squabs and begin another clutch?

**Yes.** Reliable sources describe the next egg laying beginning while squabs from the previous clutch are still being reared [SRC-001, SRC-008].

The 1983 housing study reported an average interval of about 20.3 days from hatching of a brood to laying the next batch of eggs under its conditions [SRC-008]. Because squabs are commonly still dependent beyond 20 days, overlap is biologically and operationally plausible and documented.

## 7.2 Role of the second nest

The second nest allows a pair to separate:

- an older brood being fed/reared, and
- the next clutch being laid/incubated.

This is the practical basis of the double-nest concept [SRC-001, SRC-005].

## 7.3 What does this mean for “Production Cycle”?

The research shows that a simplistic definition such as:

> cycle starts with egg laying and ends only when the squab leaves, then the next cycle starts

may be wrong for many real systems.

A pair can have reproductive responsibilities associated with more than one clutch at the same time. Phase 1A therefore leaves **OQ-003** open: the exact management definition of “production cycle” must be resolved in Phase 1B/Phase 3 based on events and measurement goals, not assumed now.

---

# 8. Daily Farm Operations

Published pigeon studies often describe husbandry procedures rather than a standardized commercial SOP. The following workflow is therefore separated into well-supported recurring husbandry tasks and field-validation items.

## 8.1 Daily operations — strong support

### Feed provision and intake observation

Breeding pigeons must be fed consistently because parental feed intake supports both adult maintenance and crop-milk/regurgitated feeding of squabs [SRC-003, SRC-006].

### Water provision

Clean water provision is a routine husbandry requirement and is explicitly described in Egyptian experimental housing [SRC-005].

### Nest / egg / squab observation

Because eggs, incubation, hatch, dependent squabs, and overlapping laying can coexist, nest inspection is a core operational observation point.

### Health and mortality observation

Daily squab survival was recorded in intensive research; mortality and health records are also prominent in established pigeon colony record systems [SRC-006, SRC-009].

### Cleaning / hygiene

Cleaning cages, drinkers, nests, and housing is repeatedly described or measured in Egyptian work [SRC-005, SRC-007]. Detailed sanitation protocols are reserved for Phase 4.

## 8.2 Periodic operations

Examples supported by the domain include:

- banding/identifying offspring,
- weighing squabs or selected breeders,
- reviewing breeding performance,
- replacing nest material,
- parasite/health monitoring,
- selecting replacements,
- evaluating poor-performing pairs,
- periodic selling/marketing.

Frequency is farm-specific and must be validated.

## 8.3 Event-driven operations

Examples include:

- first egg laid,
- second egg laid,
- fertility/egg check where practiced,
- hatch,
- squab death,
- parent death,
- fostering/hand-rearing decision,
- new clutch while older squabs remain,
- pair formation or pair break,
- disease signs,
- sale/market selection,
- culling/removal.

These are **domain events in the ordinary operational sense only**; they are not yet software Domain Events.

---

# 9. Record Keeping in Real Farms

## 9.1 Evidence of practical record categories

A published pigeon breeding-colony record system maintained offspring, location, production, health, and mortality information. When offspring were banded, recorded fields included permanent leg-band number, hatch date, strain, pen, and parents’ band numbers. Individual pen records tracked occupants; health and death records were also maintained [SRC-009].

Modern production studies additionally measure:

- egg cycle / laying interval,
- eggs laid per pair,
- egg weight,
- fertility,
- hatchability,
- squabs produced per pair,
- squab weight at multiple ages,
- mortality/survival,
- feed intake,
- economic feed cost/return [SRC-002, SRC-006, SRC-014].

## 9.2 Common Practice vs Recommended Management Practice

### Common Practice

Actual small and medium farms may use partial records, memory, nest/cage labels, notebooks, or no detailed individual records. The Egyptian socio-economic survey shows significant variation in management intensity and infrastructure among production systems, but Phase 1A did not find a strong source quantifying digital vs paper record adoption in Egyptian commercial pigeon farms [SRC-007].

### Recommended Management Practice — research-derived

For meaningful production evaluation, records should be capable of relating at least:

- identity/location of breeding stock,
- pair relationship,
- laying/hatch outcome,
- squab output/survival,
- health/mortality,
- feed/economic information where profitability is assessed.

This recommendation follows what researchers and controlled colonies must measure to evaluate performance; it is not evidence that every commercial farm currently records all of it.

---

# 10. Identification Methods

## 10.1 Individual identification

**Leg/ring bands** are well-established for permanent individual identification. A research colony used permanent leg-band numbers linked to hatch date, strain, pen and parent identities [SRC-009]. Egyptian experimental work also used leg bands / colored identifiers for distinguishing birds [SRC-005].

### Permanent identification

- unique numbered leg ring/band,
- potentially other durable identifiers if used by the farm.

### Temporary/visual identification

- colored bands or markers,
- temporary location association.

## 10.2 Pair identification

Pair identity can be represented operationally by the identities of the male and female and, in controlled farms, by a pair/cage number. Research frequently organizes records and output per pair [SRC-002].

## 10.3 Location identification

Numbered cages, pens, loft sections, and nest numbers can act as location identifiers. The recent Egyptian commercial study explicitly used numbered metal cages [SRC-002].

## 10.4 Identification risks

- A location number is not necessarily a permanent bird identity.
- A pair number is not necessarily an individual identity.
- Colored markers may not be globally unique or permanent.
- Communal systems may create more uncertainty about parentage if individual identification and nest assignment are weak.
- Lost or unreadable bands can break historical continuity unless a farm has a replacement procedure.

The identification standard actually used in target Egyptian farms remains a field-validation question.

---

# 11. Replacement, Culling, Selling, Retirement and Mortality

These concepts must remain separate.

## 11.1 Replacement

Replacement birds are retained to enter the breeding population when mature and suitable. Scientific sources report sexual maturity in the broad region of approximately 5–7 months depending on breed/source and management [SRC-003, SRC-008]. Entry should therefore depend on more than calendar age alone; body development, sex, health, pair formation, and farm policy may matter.

## 11.2 Culling

For this study, **culling** means intentional removal from the breeding/production population because the bird or pair no longer meets the farm’s health, welfare, genetic, or productivity criteria. It does not automatically mean death; the eventual disposition may differ.

Potential reasons supported as production concerns include:

- poor egg production,
- repeated infertility,
- low hatchability,
- poor squab survival/growth,
- poor parental care,
- chronic health or physical problems,
- age-related management strategy.

The sources confirm these traits are economically measurable, but do **not** establish one universal culling threshold [SRC-002, SRC-006, SRC-014].

## 11.3 Selling

Selling is a commercial disposition. A healthy bird may be sold as breeding stock or meat without being a “cull” in the poor-performance sense.

## 11.4 Retirement

Retirement means intentional withdrawal from active breeding while the bird may remain alive. Whether target farms actually use a retirement category instead of sale/cull requires validation.

## 11.5 Mortality

Mortality is an unplanned biological outcome and must not be merged conceptually with culling, sale, or retirement. It can also create immediate operational consequences for a bonded mate and dependent squabs [SRC-005].

---

# 12. Seasonality and Environment

## 12.1 Are pigeons seasonal breeders?

A major review describes pigeons as **non-seasonal breeders** [SRC-004]. Therefore the statement “pigeons naturally stop laying every summer” should **not** be accepted as a universal biological rule.

## 12.2 Heat stress and Egyptian summer

An Egyptian study conducted under summer heat-stress conditions found reduced egg production, egg weight, fertility, and hatchability, along with behavioral and physiological effects [SRC-010]. This supports a more precise interpretation:

> Severe summer conditions can depress reproduction, but that is not equivalent to a mandatory species-wide seasonal reproductive shutdown.

The magnitude of the decline likely depends on temperature, humidity, ventilation, housing, feeding, water availability, breed, acclimatization, and management.

## 12.3 Photoperiod / lighting

Controlled White King research demonstrates that photoperiod program can materially affect reproductive performance and fertility [SRC-011]. A short rearing photoperiod followed by longer laying-period stimulation improved reproductive measures under the study conditions.

This is strong evidence that light management can influence production, but **the exact Chinese White King lighting program should not be copied directly into an Egyptian farm standard without validation**.

## 12.4 Ventilation, humidity and temperature

Environmental control affects heat load, hygiene, air quality, feed/water behavior, and reproductive performance. Phase 1A confirms environment as a production driver but does not define engineering set points. Those belong to later husbandry/technical research and must account for local climate and housing style.

## 12.5 Summer belief — evidence assessment

| Claim | Assessment |
|---|---|
| “Pigeons are obligate seasonal breeders that naturally stop in summer.” | **Not supported by reviewed evidence.** |
| “Production may fall sharply in hot summer conditions.” | **Supported.** Egyptian heat-stress evidence shows reproductive decline [SRC-010]. |
| “Every farm should expect the same summer reduction.” | **Unsupported.** Climate, housing, breed and management differ. |
| “Environmental management may influence continuity.” | **Supported in principle** by heat-stress and photoperiod research [SRC-010, SRC-011]. |

---

# 13. Commercial Performance Benchmarks

Performance values vary significantly by breed, housing, feeding, parent load, early-weaning practice, climate and measurement definition. The table below is a **research benchmark map**, not a target KPI specification.

| Measure | Evidence / observed range | Conditions / interpretation | Confidence |
|---|---|---|---|
| Clutch size | Commonly ~2 eggs | Repeated across FAO/reviews and production studies; exceptions/management manipulations exist [SRC-001, SRC-004] | High |
| Incubation | ~18–20 days | FAO and multiple studies/reviews [SRC-001, SRC-005, SRC-008] | High |
| Natural weaning/market window | ~21–28 days commonly; some reports 25–32 days to leave nest | Breed/market/management dependent [SRC-001, SRC-002, SRC-005] | High for broad range; not a universal sale rule |
| Sexual maturity | Approx. 5–7 months in reviewed sources | Breed and management dependent [SRC-003, SRC-008] | Moderate–High |
| Squabs per pair per year | About 12 quoted for natural weaning in recent Egyptian paper; FAO example implies similar order under repeated broods | Strongly management dependent; early weaning can increase output [SRC-001, SRC-002] | Moderate |
| Egg/reproductive cycle | ~51–53 d in some local systems; ~37–39 d in some breeds/studies; ~10–12 d reported experimentally after separation at hatch | Definition and management differ substantially [SRC-002, SRC-012] | High evidence of variability; low confidence in any single universal value |
| 28-day body weight | ~458–465 g for parent/7-day weaning White Mirthys in one Egyptian commercial study; literature cited there describes 450–700 g depending on pigeons | Breed and feeding system highly influential [SRC-002] | Moderate for study conditions |
| Fertility / hatchability | Often reported as percentages per eggs laid/fertile eggs; values vary by study, breed, diet, environment | Must preserve numerator/denominator definitions [SRC-006, SRC-010, SRC-014] | High that they are core measures; no universal target |
| Squab mortality/survival | Management-sensitive; hatch-day artificial separation caused much higher mortality in one Egyptian study | Should be segmented by age and rearing method [SRC-002] | High for management sensitivity |

## 13.1 Why benchmarks must be contextual

A benchmark without conditions can mislead. At minimum, later analysis should preserve context such as:

- breed/strain,
- breeder age,
- housing model,
- natural vs artificial incubation,
- natural vs early weaning,
- number of squabs reared per pair,
- feed program,
- season/environment,
- exact definition of fertility/hatchability/mortality,
- market age at measurement.

---

# 14. Egyptian Context

## 14.1 Evidence base found

Phase 1A located useful Egyptian evidence from:

- Animal Production Research Institute / Agricultural Research Center work in Sharqia [SRC-007].
- Zagazig University / Egyptian Baladi pigeon research [SRC-005, SRC-015].
- A commercial farm on the Cairo–Alexandria Desert Road using White Mirthys pigeons [SRC-002].
- Matrouh University and Alexandria University work comparing Local Egyptian, Zagel and White Mirthys strains [SRC-012].
- Alexandria Journal of Veterinary Sciences heat-stress work under Egyptian summer conditions [SRC-010].

## 14.2 Production systems documented in Sharqia

The 2016 Sharqia survey classified rural pigeon production into:

1. Family production.
2. Commercial production, including:
   - mud dovecotes,
   - wooden lofts.

Wooden-loft enterprises in the sample showed stronger economic-efficiency measures than mud-dovecote and family systems under the conditions and prices of that survey [SRC-007]. This finding is useful historically and structurally but must **not** be treated as a current 2026 profitability benchmark because prices, feed costs, labor and markets have changed.

## 14.3 Egyptian breeds/strains in research

Recent Egyptian work includes:

- Local Egyptian / Baladi,
- Zagel,
- White Mirthys.

A 2022 Egyptian study reported White Mirthys as superior in several growth traits among the three studied strains [SRC-012]. This supports breed as an important performance context variable, not a decision that White Mirthys must be the target breed.

## 14.4 Egyptian climate

The heat-stress evidence makes Egyptian climate operationally significant. Summer decline should be studied as an interaction among environment, housing, nutrition, water, and management rather than encoded as a fixed seasonal shutdown [SRC-010].

## 14.5 Evidence gap in Egypt

The reviewed Egyptian literature is useful but does not yet provide enough robust, current evidence to standardize:

- national prevalence of cage vs loft vs dovecote commercial systems in 2026,
- current typical farm size,
- current commercial market age/weight specifications by region/customer type,
- current record-keeping tools,
- current adoption of individual leg bands,
- current adoption of artificial incubation/early weaning,
- standard pair-culling thresholds,
- current biosecurity/vaccination protocols across commercial farms.

These gaps require field validation and later targeted research.

---

# 15. Evidence-Based Domain Findings

## 15.1 Verified / Strong Evidence

1. Squabs are altricial and depend on parental or artificial feeding in early life [SRC-002, SRC-003].
2. Both male and female pigeons produce crop milk [SRC-003].
3. Both sexes participate in incubation and parental care [SRC-001, SRC-004, SRC-005].
4. Two eggs per clutch is the dominant pattern in the reviewed literature [SRC-001, SRC-004].
5. Incubation is approximately 18–20 days [SRC-001, SRC-005, SRC-008].
6. Around 3–4 weeks is a common natural squab market/weaning region [SRC-001, SRC-002].
7. Overlap between care of existing squabs and the next clutch occurs [SRC-001, SRC-008].
8. Double-nest arrangements support that overlap [SRC-001, SRC-002, SRC-005].
9. Breeding-pair performance is a major unit of measurement in commercial research [SRC-002, SRC-006, SRC-014].
10. Housing system can materially affect productivity and measurability [SRC-007, SRC-008].
11. Heat stress can reduce reproductive performance in Egyptian summer conditions [SRC-010].
12. Photoperiod can affect reproductive performance [SRC-011].
13. Breed/strain affects growth and therefore market/performance expectations [SRC-012].
14. Parent loss directly affects dependent squabs and may trigger foster/hand-rearing management [SRC-005].
15. Individual banding and parent/location-linked record keeping are established practical identification methods [SRC-009].

## 15.2 Industry / Producer Practice Requiring Validation

- Exact frequency of double nests in Egyptian commercial lofts.
- Whether Egyptian farms primarily identify birds individually or manage by pair/nest/cage.
- Actual thresholds used to classify a pair as weak.
- Frequency of deliberate re-pairing.
- Whether replacement birds are selected mainly on lineage, body weight, parent output, phenotype, or farmer judgment.
- Actual daily paper/Excel/app record workflows.
- Current use of artificial incubation and hatch-day/early hand feeding.

---

# 16. Important Contradictions and Variability

## CON-001 — Length of the production/egg cycle

**Source pattern A:** Local Indonesian pigeon work reports around 51 days; recent Egyptian literature cites local Egyptian cycles around 52.75 days [SRC-002, SRC-013].  
**Source pattern B:** Other breeds/systems report substantially shorter periods, e.g. around 37–39 days [SRC-002].  
**Experimental intervention:** Hatch-day separation in White Mirthys dramatically shortened the measured egg/reproductive cycle in one 2025 experiment [SRC-002].

**Interpretation:** “cycle length” is a function of breed, definition, parental-care load, and management intervention.  
**System impact later:** cycle duration must not be hard-coded as a universal constant.

## CON-002 — Natural production vs artificial early weaning

Natural parental rearing protects squab growth/survival but occupies parental resources. Early separation can increase breeder egg throughput but may increase squab mortality or reduce growth if artificial rearing is inadequate [SRC-002].

**Interpretation:** higher egg throughput is not automatically higher economic or welfare performance.

## CON-003 — Housing model

Pair cages gave better output/economics than communal fly-pens in one historical controlled study [SRC-008], while commercial Egyptian production also exists in wooden lofts and mud dovecotes [SRC-007].

**Interpretation:** no universal “correct” housing model can be selected from Phase 1A alone.

## CON-004 — Summer production

Review literature describes pigeons as non-seasonal breeders [SRC-004], while Egyptian heat stress research demonstrates summer reproductive depression [SRC-010].

**Interpretation:** environmental suppression is not the same as an obligatory seasonal reproductive stop.

---

# 17. Field Validation Required

The following should be explicitly checked with Egyptian commercial producers / animal-production specialists:

1. Which commercial housing models are actually common in the target customer segment: wooden loft, mud dovecote, colony room, pair cage/battery, mixed?
2. Is each breeding pair normally assigned one nest or two nests in the target farms?
3. How are overlapping clutches recognized and recorded in practice?
4. Are breeders individually ringed, or identified only by pair/cage/nest/location?
5. What defines a “production cycle” in the farmer’s own records?
6. What Egyptian buyers currently consider the desired squab age and live/dressed weight?
7. What thresholds trigger pair review, re-pairing or culling?
8. How are replacements selected and at what stage are they admitted to breeding?
9. How severe is summer production decline by housing type and region, and what mitigation is used?
10. What records are actually kept today and at what granularity?
11. Is artificial incubation or early hand feeding economically practiced in the target market, or mainly experimental/specialized?
12. What happens operationally when one parent dies while dependent squabs are present?

---

# 18. Future Research Queue Candidates

The following topics appeared during Phase 1A but should **not** be expanded here:

- Detailed egg lifecycle and egg-quality management → **Phase 1B / Phase 3**.
- Detailed squab growth/weaning management → **Phase 1B / Phase 3**.
- Disease, vaccination, treatment, quarantine and biosecurity protocols → **Phase 4**.
- Feed formulation, nutrient requirements and feed inventory → **Phase 4 / Phase 5**.
- Financial unit economics and cost allocation → **Phase 5**.
- Formal KPI definitions → **Phase 6**.
- Software representation of pair, clutch, nest, bird identity or overlapping cycles → **Phase 7 only after domain analysis**.
- Artificial intelligence / prediction → **Phase 8**.

---

# 19. Source Register

> Access Date for all sources below: **2026-08-17**. Reliability reflects suitability for the specific information used, not a universal rating of the publication.

### SRC-001
- **Source:** Livestock keeping in urban areas — pigeon section
- **URL:** https://www.fao.org/4/Y0500E/y0500e05.htm
- **Organization / Author:** FAO
- **Publication Date:** Not clearly stated on accessed page
- **Reliability:** High
- **Information Used:** maturity, incubation, two-egg clutch, parental crop milk, ~4-week collection, two-nest intensive overlap.

### SRC-002
- **Source:** Early weaning in pigeons (Columba livia domestica): effects on squabs performance and reproductive performance of parents
- **URL:** https://pmc.ncbi.nlm.nih.gov/articles/PMC11998371/
- **Organization / Author:** Mohamed OA, Khattab IM, Elsagheer MA et al.; BMC Veterinary Research
- **Publication Date:** 2025-04-14
- **Reliability:** High — peer reviewed, Egyptian commercial farm
- **Information Used:** White Mirthys commercial farm, pair cages, two nests, 28-day control, early weaning effects, cycle variability, mortality, weights, reproductive performance.

### SRC-003
- **Source:** Chemical composition of pigeon crop milk and factors affecting its production: a review
- **URL:** https://pmc.ncbi.nlm.nih.gov/articles/PMC10149254/
- **Organization / Author:** Jin C-L et al.; Poultry Science
- **Publication Date:** 2023
- **Reliability:** High — peer-reviewed review
- **Information Used:** altricial development, crop milk from both parents, sexual maturity context, growth dependence on parents.

### SRC-004
- **Source:** Pigeon during the Breeding Cycle: Behaviors, Composition and Formation of Crop Milk, and Physiological Adaptation
- **URL:** https://pmc.ncbi.nlm.nih.gov/articles/PMC10533064/
- **Organization / Author:** Life (MDPI), 2023 review
- **Publication Date:** 2023-09
- **Reliability:** High — peer-reviewed review
- **Information Used:** non-seasonal breeding, pair bond, two eggs, biparental incubation/care, breeding-cycle biology and artificial production context.

### SRC-005
- **Source:** Comparing the Effect of Different Management and Rearing Systems on Pigeon Squab Welfare and Performance after the Loss of One or Both Parents
- **URL:** https://pmc.ncbi.nlm.nih.gov/articles/PMC6523572/
- **Organization / Author:** Abdel Fattah AF et al.; Animals
- **Publication Date:** 2019-04-14
- **Reliability:** High — peer reviewed; Egyptian Baladi pigeons
- **Information Used:** Egyptian housing, two nests, parent loss, fostering, parental care, incubation and nestling period, identification.

### SRC-006
- **Source:** Perspectives approaches using dietary glutamine and L-carnitine toward enhancement of reproductive performance of breeding pigeons...
- **URL:** https://pmc.ncbi.nlm.nih.gov/articles/PMC12274820/
- **Organization / Author:** Poultry Science; Egyptian and regional university authors
- **Publication Date:** 2025
- **Reliability:** High
- **Information Used:** production measurements used for breeders/squabs: feed intake, egg cycle, eggs, fertility, hatchability, squabs/pair, growth and economics.

### SRC-007
- **Source:** Socio-economic analysis of pigeon production systems in Al-Sharqia Governorate, Egypt
- **URL:** https://www.researchgate.net/publication/312173925_SOCIO-ECONOMIC_ANALYSIS_OF_PIGEON_PRODUCTION_SYSTEMS_IN_AL-SHARQIA_GOVERNORATE_EGYPT
- **Organization / Author:** Omar AS et al.; Egyptian Poultry Science Journal; Animal Production Research Institute / Agricultural Research Center
- **Publication Date:** 2016
- **Reliability:** Medium-High — peer-reviewed journal article accessed via author-hosted copy; survey is regional/historical
- **Information Used:** family vs commercial purpose, mud dovecotes, wooden lofts, management variation, economics and Egyptian context.

### SRC-008
- **Source:** Systems of Housing and Feeding of Pigeons for Squab Production
- **URL:** https://www.searca.org/pubs/abstracts-theses-dissertations/database/view?absid=1043
- **Organization / Author:** Warlito A. Baticados; University of the Philippines Los Baños / SEARCA
- **Publication Date:** 1983
- **Reliability:** Medium — doctoral research, historical
- **Information Used:** cage vs communal fly-pen performance, maturity, incubation, hatch-to-next-lay interval, biparental care.

### SRC-009
- **Source:** A record-keeping system for a pigeon breeding and research colony
- **URL:** https://pubmed.ncbi.nlm.nih.gov/642443/
- **Organization / Author:** PubMed-indexed research report
- **Publication Date:** 1978
- **Reliability:** Medium-High — indexed but research-colony rather than commercial-farm context
- **Information Used:** permanent leg bands, hatch date, strain, parent identity, pen, health and mortality records.

### SRC-010
- **Source:** Impact of Heat Stress on Reproductive Behavior, Performance and Biochemical Parameters of Pigeon
- **URL:** https://www.alexjvs.com/index.php?mno=292429
- **Organization / Author:** El Shoukary RD, Abdel-Raheem GS, Osman AS; Alexandria Journal of Veterinary Sciences
- **Publication Date:** 2018
- **Reliability:** High for study conditions — peer-reviewed Egyptian summer experiment
- **Information Used:** heat stress reduced egg production, egg weight, fertility and hatchability.

### SRC-011
- **Source:** Effect of different photoperiodic programs from rearing period on the reproductive performance and hormone secretion of White King pigeons
- **URL:** https://pmc.ncbi.nlm.nih.gov/articles/PMC10900098/
- **Organization / Author:** Poultry Science
- **Publication Date:** 2024
- **Reliability:** High — peer reviewed
- **Information Used:** photoperiod influences egg production/fertility and sexual maturation; environmental management matters.

### SRC-012
- **Source:** Productive Performance of Three Strains of Pigeons (Columba livia domestica) Under Egyptian Conditions
- **URL:** https://www.researchgate.net/publication/371667245_PRODUCTIVE_PERFORMANCE_OF_THREE_STRAINS_OF_PIGEONS_COLUMBA_LIVIA_DOMESTICA_UNDER_EGYPTIAN_CONDITIONS
- **Organization / Author:** Ahmed O, Bahie El-Deen M, Abaza IM, Abou Khadiga G; Egyptian Poultry Science Journal; Matrouh/Alexandria universities
- **Publication Date:** 2022
- **Reliability:** Medium-High — journal article accessed through hosted full text
- **Information Used:** Local Egyptian, Zagel, White Mirthys growth differences under Egyptian conditions.

### SRC-013
- **Source:** Productivity of Local Pigeon Fed with Cafeteria Method in Intensive Rearing
- **URL:** https://repository.ipb.ac.id/handle/123456789/76755
- **Organization / Author:** IPB University repository; Darwati S et al.
- **Publication Date:** 2009
- **Reliability:** Medium
- **Information Used:** individual-cage intensive production, egg output, fertility, hatching rate, approximately 51-day production interval and phase-based feed use.

### SRC-014
- **Source:** Effect of different dietary energy/protein ratios on growth performance, reproductive performance of breeding pigeons and slaughter performance, meat quality of squabs in summer
- **URL:** https://pmc.ncbi.nlm.nih.gov/articles/PMC10206179/
- **Organization / Author:** Poultry Science
- **Publication Date:** 2023
- **Reliability:** High
- **Information Used:** practical research measurements: breeder/squab weights, survival, feed conversion, egg-laying interval/rate, fertilization and hatching rate.

### SRC-015
- **Source:** Effect of the number of incubated eggs and nurturing squabs on the behaviour and performance of breeding pigeons
- **URL:** https://www.advetresearch.com/index.php/AVR/article/view/1626
- **Organization / Author:** Journal of Advanced Veterinary Research; Zagazig University-linked authors
- **Publication Date:** 2024
- **Reliability:** Medium-High
- **Information Used:** Egyptian Baladi pair response to different incubated-egg/squab loads; evidence that parental load affects behavior/performance.

---

# 20. Phase 1A Research Conclusion

The research establishes five domain principles that must carry forward:

1. **The dependent squab and biparental care are defining features of the production system.**
2. **The breeding pair is a central operational production unit, but not the only level of management.**
3. **Nest management—especially the possibility of two nests—is structurally important because reproductive cycles can overlap.**
4. **Housing and production intensity change how reliably a farm can control pairing, attribute output, and keep records.**
5. **Performance is contextual. Breed, environment, parental load, housing, and rearing strategy materially change the numbers; universal constants would be misleading.**

Phase 1A is complete for review. Detailed chronological analysis of the pigeon production lifecycle is intentionally deferred to **Phase 1B — Detailed Pigeon Production Lifecycle**.
