---
name: methods-apparatus-functional-catalog
version: 0.1.1
status: draft
dfs_schema_version: n/a
last_changed: 2026-07-19
document_class: specification
provenance: "[AI+] full EN translation per author decision 2026-07-19"
---

# Functional Catalogue of the Method Apparatus

**Inventory:** 20 apparatuses of the prompt-library (17 framework prompts, 2 core pipeline stages, 1 custom-tool prompt; the 21st prompt file, translation, is not catalogued here).
**Basis:** reading of the files, each adversarially evidence-checked. No test on artefacts (see §8).
**Commission:** author session 2026-07-16 — "catalogue the present method apparatus, but not from a genealogical standpoint, rather from a functional one."
**Machine-readable version:** [`catalogue.yaml`](catalogue.yaml) (derived_from **this** file — this prose is authoritative on any discrepancy; the YAML carries the structure, not the reasoning/the hedges). Master index: [`manifest.yaml`](manifest.yaml).

> **Origin:** This file arose 2026-07-16/17 as an internal methodology note and was moved here
> as the operating basis of the tool (a cut, not a copy — so that two versions do not drift).
> **An open follow-on question:** `prompts/core/artifact-triage.md` §7 requires a "prompt-library
> framework catalog (the frameworks' own declared L1/D1/D2/D3 blocks)" — this catalogue is
> de-named and L3-centred, so it does not meet the wording without adaptation. Whether the gate
> means this catalogue or another artefact remains open. Additionally now relevant: the two
> surfaces carry **different licences** (prompt-library CC BY-SA, this repo proprietary) — an
> artefact meant to satisfy the §7 gate would, licence-wise, have to live there, not here.

---

## 1. The cut

The genealogical cut sorts by origin: Frankfurt / Paris / Kyoto / communication research. It makes kinship visible and work invisible.

On the present inventory, the functional cut shows three things the genealogical one conceals:

1. **Eight apparatuses from five mutually and avowedly hostile traditions perform the same move on one artefact** — "this looks self-evident but was in fact produced" (C1). The declared L1 conflicts among them (Habermas ↔ Luhmann ↔ Foucault) concern the justification, not the action.
2. **Auditability and genealogy are complementarily distributed.** The three apparatuses with a falsifier throughout (`content-analysis`, `asemic-pattern-detection`, `source-criticism`) are exactly the three whose proper names are fully strippable. In the present inventory, the tradition density in a file's header correlates inversely with the testability of its core.
3. **The falsifiable apparatuses are, by interop declaration, the suppliers of the unfalsifiable ones.** This is invisible in the genealogical cut, because supplier and consumer belong to different traditions and stand there on different sides.

The catalogue is de-named: operations stand as verb + object. Proper names appear only in §6 (residue) — there they are the object, not the means.

---

## 2. Operations map

Sorted by operation. An apparatus appears several times. `∘` = performs the operation; `∘*` = performs it with a test point that fails on the artefact.

| # | Operation (de-named) | Apparatuses | n |
|---|---|---|---|
| **O1** | Expose what presents itself as self-evident as made | semiotics · critical-theory · poststructuralism∘* · postcolonial-theory · feminist-theory · systems-theory∘* · pragmatism · structuralism (institution op) | 8 |
| **O2** | Hold a ready-made compartment list up to the material, log hits and gaps | content-analysis∘* · structuralism · speech-act-theory · phenomenology · existentialism · stoicism · form-linter · artifact-triage · asemic-pattern-detection∘* | 9 |
| **O3** | Extract the load-bearing pair of opposites | structuralism · semiotics · poststructuralism · feminist-theory (L3) · systems-theory (code) | 5 |
| **O4** | Trace a neutrally-presenting statement back to its place of production | feminist-theory · postcolonial-theory · source-criticism∘* · critical-theory · systems-theory | 5 |
| **O5** | Register absence as a finding | content-analysis∘* · feminist-theory · postcolonial-theory · poststructuralism · semiotics · structuralism | 6 |
| **O6** | Cut a text/an artefact into its smallest self-contained parts | structuralism · semiotics · content-analysis · form-linter · asemic-pattern-detection · critical-theory · feminist-theory · hermeneutics · existentialism | 9 |
| **O7** | List the web of conditions; no part stands alone | systems-theory · eastern-philosophy · pragmatism | 3 |
| **O8** | Suspend one's own categories; describe only what is present | phenomenology · eastern-philosophy | 2 |
| **O9** | Check whether the presentation is covered by the substance | speech-act-theory∘* · form-linter · eastern-philosophy | 3 |
| **O10** | Split the situation into fixed and influenceable | stoicism · existentialism | 2 |
| **O11** | Count the kinds; hold the distribution against chance | content-analysis∘* · asemic-pattern-detection∘* | 2 |
| **O12** | Fix the material's status before interpreting | artifact-triage∘* · source-criticism∘* | 2 |
| **O13** | Inventory the channels; state their ranking | multimodal-analysis∘* · artifact-triage · phenomenology (figure/ground) | 3 |
| **O14** | Propose an intervention | pragmatism∘* · systems-theory · postcolonial-theory · critical-theory · eastern-philosophy · stoicism · existentialism | 7 |
| **O15** | Assign a person's position/role from the material | structuralism · feminist-theory · existentialism · speech-act-theory · semiotics | 5 |
| **O16** | Reconstruct an artefact's mode of address toward its addressee | semiotics · structuralism (institution op) · critical-theory · speech-act-theory | 4 |
| **O17** | Log one's own preassumption; track its shift | hermeneutics · feminist-theory (situatedness) | 2 |
| **O18** | Differentiate two renderings of the same content | multimodal-analysis∘* · source-criticism (transmission chain) | 2 |
| **O19** | Locate the tip-over from unremarkable to remarkable | phenomenology | 1 |
| **O20** | Sort sign-binding by similarity / contact / convention | semiotics∘* | 1 |
| **O21** | Check whether a dispute has any stakes at all | pragmatism | 1 |
| **O22** | Test the crossing of several belonging-markers for an effect that arises only there | feminist-theory | 1 |
| **O23** | Find the spot where pressing produces the counter-pressure | eastern-philosophy | 1 |
| **O24** | Check the independence of concurring pieces of evidence | source-criticism∘* | 1 |

**Reading of the map.** Of 24 operations, 6 are solo operations (O19–O24) — they carry the entire discriminating power of the inventory. The four most-populated operations (O1, O2, O6, O14) together gather 33 apparatus entries. O6 (decompose) is the first step in 9 apparatuses and the finding in none.

---

## 3. The apparatuses individually

Format: **does** | **grips** | **delivers** | **sees alone** | **reads past**

---

**semiotics** (`in-test`, 1.2.1)
Decomposes a meaning-bearing element; sorts its binding to the meant by similarity / physical contact / convention; exposes a meaning that presents itself as self-evident as produced; declines a pair of opposites through four positions and marks the empty ones. | Single item, any modality; historical context + (for the receiver axis) reception data. | Prose reading, sign typology, four-position grid. | **The binding sort** (O20) — no other separates smoke from pictogram from word. And the change of storeys: the surface presents itself as non-surface. | Presupposition "when a meaning appears natural, that naturalisation is itself an ideological operation" — the finding "nothing is produced here" is not provided for in the procedure. The file recommends exactly this operation as its core.

**structuralism** (`in-test`, 1.1.0)
Substitutes an element on a trial basis and checks whether the meaning tips; names which side of a pair is the tacit normal case; holds a ready-made 31-step list up to a narrative. | Single item or corpus; a comparison set mandatory, historical context expressly not. | Grid, procedure log, reconstruction. Valuation expressly outsourced. | What is **not** there but could have been — and the asymmetry (which side must be named, which runs along unstated). | The institution operation puts the answer before the question; "apply the framework generously … identify functional equivalents" is a licence to re-declare the non-fitting as an equivalent. *(Verify: the substitution test has no adjudicating authority — analyst-bound.)*

**source-criticism** (`in-test`, 1.1.0)
Checks a provenance claim against external evidence; traces the transmission chain; reconstructs the maker's interest position; checks whether concurring pieces of evidence descend from one another; assigns a graded mark. | Single item or corpus; comparison set + historical context mandatory. | Four-level reliability mark, chain diagram, evidence map. A licence document for downstream apparatuses. | **The independence question** (O24) — three concurring pieces of evidence are one piece of evidence if they are copied from each other. And: the gap between what an artefact claims to be and what it is. | The ideal-figure comparison ("what would a fully informed, neutral witness have recorded that this source does not?") has no negative outcome. Tendency mapping presupposes the existence of what it finds. The finding stays local (it colours a mark), because the calibration hangs externally.

**multimodal-analysis** (`in-test`, 1.1.0)
Counts the simultaneously speaking channels; holds, per channel, the decision taken against the possible ones; types the channel relation (concurrent / division-of-labour / contradictory); differentiates source from target version on a change of form. | ≥2 occupied channels OR two versions; comparison set. | Channel list, relation typology, difference list. | **The friction at the seam** between two channels — meaning that lies neither in the one nor in the other alone. | Three bars against the null finding, one at L1: "No communication is ever purely verbal or purely visual" rules the single-channel finding out ontologically. "Resemiotization is never neutral" turns every format adaptation into an attribution of interest.

**feminist-theory** (`in-test`, 1.0.3)
Decomposes an attribution into repeated actions and reconstructs the sanction; crosses belonging-markers; traces a neutrally-presenting statement back to its place of production; lists the silenced. | Artefact with persons or a knowledge claim; production conditions obligatory. | Argumentative reading + diagnosis. *(Verify: the declared "matrix" is not licensed in the file — they are prose instructions.)* | **The crossing** (O22) — an effect that arises only at the overlap, including the consequence that single-axis repair can do harm. | Declared step: "identify how interventions may *inadvertently* reproduce intersectional harm by addressing only one axis" — the repair has no outcome at which it repairs.

**postcolonial-theory** (`in-test`, 1.0.3)
Checks by what unspoken standard the represented are measured; maps the knowledge ranking; checks the infrastructure of being heard; traces continuation in the seemingly neutral; demands a criterion-change counter-proposal. | A centre-outside gradient with a historical thread of domination; historical context mandatory. | Reading + reconstruction + counter-proposal + (in one prompt) self-location. | **Absence vs. the structural impossibility of speaking** — not whether someone is missing, but whether the infrastructure for them exists. | "Critique the *benevolent* intellectual … *How* does this representation reinscribe the power differential" — a how-question, not a whether-question. Plus: inclusion is by construction addition, not transformation. Who does nothing reproduces; who does something reproduces benevolently.

**critical-theory** (`in-test`, 1.0.3)
Holds an artefact to its own declared standard; historicises an order that presents itself as natural; checks whether individuality comes out of a kit; checks whether validity claims are redeemed with reasons. | Artefact with a declared claim + addressee; production conditions + historical context. | Reading with a built-in ought, closes with a transformation question. | **The test standard drawn from the tested** — no other draws the norm from the artefact itself. And: produced consent as an object in its own right. | `incorporate` in "what counter-hegemonic possibilities does it foreclose or incorporate?" — absorption and repulsion fall into one finding. "while actually being standardized" puts the result before the test. *(Verify: the claim-against-practice test is framed as a task — "Show the contradiction" — not as a hypothesis.)*

**poststructuralism** (`in-test`, 1.0.3)
Maps what is sayable and who is allowed to speak; checks whether the preferred side of a pair is definable without the devalued one; reconstructs the emergence of a self-evidence at concrete episodes; lists the components of a formation and the capacity that arises only in their interplay. | Artefact with a no-alternative claim; a historical record mandatory. | Rule map, genealogy, aporia demonstration — expressly without resolution and without counter-proposal. | **The aporia** — the spot where a text runs against its own presupposition and this is endured instead of repaired. And the condition of sayability instead of the statement. | "Power is productive" makes every improvement necessarily also a production. The brought-along categories (surveillance / normalisation / examination) inevitably read a feedback conversation as a disciplinary mechanism.

**hermeneutics** (`in-test`, 1.0.3)
Writes down one's own preassumption before the reading and logs its shift; reconstructs the question the artefact was an answer to; goes back and forth several times between passage and whole; decomposes a narrative into turning point/background/breaking point. | Single item with a meaning claim **and distance**; a clarified source declared as a precondition. | Dense reading + the logged path to it. | **The analyst's position as an analysed object** (O17) — not as bias but as a condition whose shift belongs to the result. And: the time difference as a productive quantity. | "What is the text *about*, at its deepest level?" has no null outcome. "Who benefits from this telling, and who or what is suppressed?" is an obligatory step, not an open question — a successful repair without a breaking point appears as a smoothed-over one.

**phenomenology** (`in-test`, 1.0.3)
Sets the prevailing explanations aside and describes the enactment; separates focus from unnoticed background; decomposes the temporal course; locates the tip-over unremarkable→remarkable; keeps a two-column ledger of gain/loss. | Single item with an enactment and a user; no context required. | Inside-perspective account + four-case typology + loss ledger. Valuation expressly prohibited. | **The tip-over** (O19) — the state in which something works and is therefore not noticed, and the moment in which the working breaks off. | "What does it reduce or occlude?" is grammatically forced; the interop line passes the produced loss on to ideologiekritik. The essence claim ("essential structures … that hold across variations") follows from a single case without a variation procedure.

**speech-act-theory** (`in-test`, 1.1.0)
Decomposes an utterance into wording / action / effect; types the action; checks off a condition list; distinguishes misfire from hollowing-out; checks recognition by the addressee; checks the authority against the institutional frame. | An addressed utterance with an identifiable speaker; institutional context mandatory. | Action label + condition ledger (met / not met / undecidable). | **The two forms of failure** — did not come about vs. came about and is hollow. And the recognition condition: no one objects and yet nothing happens. | The counterfactual norm produces a deficit finding on every real conversation; the split into understanding-oriented/success-oriented has no third case, so every effective repair falls into the second category. Pure typing reads past nothing.

**pragmatism** (`in-test`, 1.1.0)
Checks what would behave differently depending on the outcome; translates an abstract claim into observable processes; runs a five-step procedure with a refutation test; checks whether the means fit the declared purpose. | Disturbance / dispute / open choice — built on situations, not on works; comparison set. | Diagnosis + ranking + a small-format, retractable intervention proposal. | **The null finding as an outcome** (O21) — "if no practical difference can be identified, the dispute may be merely verbal". And the means-end control. *(Verify: the null finding is analyst-relative — the file has no test step for the first prompt. The refutation test hangs on the second.)* | Downward: a real difference without a measurable consequence is cleared away as a war of words. Upward: "What habits are at the root of the problem?" presupposes the problem. It does not invert into "ideological" but into "not yet solved".

**existentialism** (`in-test`, 1.0.3)
Looks for the spots where a choice is framed as a compulsion; splits the situation case by case into fixed / influenceable; assigns one of three ways of dealing with irresolvability; closes with an exhortation. | Self-report with an attributable subject; no external context. | Diagnosis + three-compartment grid + exhortation to the addressee. | **The rewriting of a choice into a fact**, from the narrator's inside view. | Fully closed: "I had no choice" = self-deception, "I chose" = authenticity. A real constraint (mortgage, children — the file's example) is grounds for suspicion. Binding oneself to an external certainty is, by vocabulary, capitulation.

**stoicism** (`in-test`, 1.0.3)
Sorts a situation by a **fixed list** into influenceable / not influenceable; separates the incident from the immediate interpretation; runs a four-line checklist; checks means against self-purpose; changes the scale of viewing. | First-person report under pressure to act; no context. | Bipartition + action recommendation + exercise + quotation. | **The limit of a person's radius of action in a situation** — which part of the suffering hangs on the immovable, which on one's own interpretation. | Inverse to the heavy apparatuses: it inverts a real external injury into a thinking error of the injured. The file names it itself ("risks individualising structural harms"). No null finding: "when a person presents any problem". *(Verify: the sorting is set by a fixed list, not raised on the case — thereby unfalsifiable on both levels.)*

**eastern-philosophy** (`in-test`, 1.0.3)
Traces the web of conditions; diagnoses the effort that produces the resistance; matches designation against enactment; suspends one's own categories; counts those who suffer. | Subject with stakes; no context. Six prompt sections. | Course description + action recommendation to the addressee. | **The effort diagnosis** (O23) — the pressing produces the counter-pressure. *(Verify: no performable test — the counter-check step is a counterfactual imagination.)* | Reads every artefact as a plight with an attachment cause. Structural hardship is translated into inner change (the file quotes it itself: "begins not with external structures but with an inner revolution"). A successful repair has no category. Two operations permit, by their wording, a null finding.

**content-analysis** (`in-test`, 1.1.0)
Cuts material into segments and orders them by a pre-written rulebook; forms categories inductively from the material to saturation; counts the distribution including blanks; contrasts subsets; measures agreement between two coders. | Single item or corpus; a fully formulated question + context unit; source status outsourced. | Codebook + coded corpus + distribution picture + agreement measure. Expressly no understanding. | **Rule-governed, re-countable, repeatable absence across a corpus** (O5 with a test point). And: one's own assignment as a measurable quantity instead of a reader competence. | Overwrites instead of reading past: the innovation gets the nearest label or lands under "Other" and quietly disappears. Secondly: it **passes on** the authority of the number to the evaluating apparatuses (interop instruction).

**systems-theory** (`in-test`, 1.1.0)
Traces feedbacks including delay; orders intervention points by depth; reads the boundary of a configuration off its operation; checks whether a functionally equivalent substitute is nameable; reconstructs an observer's standard. | Recurring enactments at meso/macro level; process data + comparison set; historical context expressly not. | Circuit map + intervention ranking + state diagnosis. Forecast expressly excluded. | **An effect that strikes back on its cause — with a delay.** No other models time as a circle. | Self-production absorption: every enactment is describable as self-maintenance, so the apparatus has no predicate for "here an error was fixed". Contingency as a task, not a hypothesis. The anti-humanism compulsion does not let a declared intention stand as an intention. *(Verify: the lever ranking is brought along, not raised — no falsifier.)*

**artifact-triage** (`in-test`, 1.2.2, `core/`)
Types the piece; maps channels and their ranking; separates the spoken-out from the co-meant; locates the order of magnitude; determines the provenance standing; assigns procedures — **only from a present list**; marks stumbling blocks. | Everything; preconditions lie in the environment (catalogue in the context; model capability level), not on the object. | Eight-part profile + graded recommendation (primary / secondary / contraindicated). No reading. | **The jurisdiction question** — the gap between what the thing is and what is being asked. Plus a refusal gate: "If NO catalog is present: do NOT route." | Forced cell: it forces a decision on pieces whose whole point is undecidedness (the minimal variant has no ambiguity flag). And: it claims frame neutrality, while the load-bearing distinction is, per its own conflicts line, frame-dependent.

**form-linter** (`draft`, 0.1.0, `core/`)
Decomposes a generated text into moves; looks for four named presentation patterns; decides, per site, covered / put-on / undecidable; cites verbatim; stops — rewriting is excluded; matches against the output contract of the upstream procedure. | **Generated analytical text**, not the artefact; prior history + output contract. | Finding list with a count line. Null finding permitted and declared. | **It reads the output of another apparatus** — the only downstream stage. And: a form held constant across changing objects as an index of the producer. | Declares itself: "Silent application to framework-conformant output produces systematic false positives." The discriminator is, by self-declaration, not operationalised — the honest retrospection is not separable from the self-curation.

**asemic-pattern-detection** (`draft`, 0.2.3, custom-tool)
Declares the counting unit or **refuses**; forms kinds to saturation with visual validation; counts them out and tests against chance; tests predictability against 1000 randomised comparison collections; contrasts subsets by place and surroundings; compares collections for signature distance. | Corpus of writing-shaped marks without an accessible meaning side; reading direction + position data. | Codebook + significance results + signature matrix. Each block with a limitations statement. | **Checkable statements on an artefact without an accessible meaning side.** | Positive guarantee: the file says itself that a Zipf finding "does not isolate semantic shaping from motor/cognitive shaping" — the main test is almost always passed. Bracketing inversion (hedged): the asemic positing comes unchecked from outside; if wrongly posited, the apparatus turns a meaning-bearing artefact into a distribution object and delivers technically flawless findings that do not show the error.

---

## 4. Redundancy clusters

Four clusters in which several apparatuses functionally coincide on one artefact. **All verdicts are hypotheses from file reading** (§8).

### C1 — Constructedness (8 apparatuses, 1 operation)
O1. semiotics · critical-theory · poststructuralism · postcolonial-theory · feminist-theory · systems-theory · pragmatism · structuralism.

Discriminator at the result: **what must be presented?**
- systems-theory: a nameable functionally equivalent substitute — if none is found, the claim falls.
- poststructuralism: concrete historical episodes.
- postcolonial-theory: a thread to imperial expansion (jurisdiction gate — can be non-jurisdictional).
- The remaining five: **nothing.**

Seven of the eight are unfalsifiable for the same reason: the question has no null answer.

**Test.** An artefact set with declared negative cases (technical specification, bug report, documented open error correction, measurement protocol) plus positive cases (advertising, mission statement). Run all eight blind against it, take the verdict binary. **Forecast:** semiotics / critical-theory / feminist-theory / pragmatism deliver a 100 % positive rate; systems-theory and poststructuralism split; postcolonial refuses or splits. Whoever does not split is not a checker.

### C2 — Grid application (9 apparatuses, 1 operation)
O2. content-analysis · structuralism · speech-act-theory · phenomenology · existentialism · stoicism · form-linter · artifact-triage · asemic-pattern-detection.

Discriminator: **is there a second-coder test?**
- content-analysis: yes (κ, saturation, resistance segments). *(Verify: the resistance clause offers "category revision **or** a residual Other category" — the revision is optional, and the counter-evidence thus disposable.)*
- asemic-pattern-detection: yes (visual pass + permutation).
- form-linter: declared as an exit condition, unrun, n=1.
- The remaining six: self-adjudicating.

structuralism's own neighbour determination says it: "content-analysis validates the category application across several coders … this apparatus has no such test."

**Test.** Two analysts, the same artefact, the same apparatus, independently. For structuralism / existentialism / stoicism / phenomenology / speech-act-theory compare the grid assignments. If κ falls below what content-analysis demands of itself, the list is controlled at the analyst, not at the material. **Never run on any of the six.** Cost: one artefact, two runs, one comparison.

### C3 — Place of production (5 apparatuses, 1 operation)
O4. feminist-theory · postcolonial-theory · source-criticism · critical-theory · systems-theory.

**No extractor names one of the first three as a neighbour of another.** The difference is not the procedure but the consumer: source-criticism books into a graded evidence mark (local), feminist/postcolonial into a condemnation. source-criticism's own failure field describes the ramp: the tendency finding "has three consumers that escalate it and none that cancels it".

**Test.** Blind assignment (see below) over source-criticism Op. 4 vs. feminist-theory situatedness, on an artefact with a known interest position. Forecast open — this is the only cluster without a prior conjecture.

### C4 — The declared self-dissolutions (4 pairs)
Four clusters in which the files **concede their redundancy in writing** and are nonetheless kept separate:

| Pair | File self-disclosure | Discriminator |
|---|---|---|
| **O8** phenomenology ≡ eastern-philosophy | "independent discoveries of the same methodological move" | none |
| **O7** systems-theory ≡ eastern-philosophy | eastern-philosophy's subtraction: "de-named not distinguishable from systems-theory, only without its notation" | notation, stocks/rates, delay, lever rank |
| **O9** speech-act-theory ≡ eastern-philosophy (≈ form-linter) | the overlap is noted in eastern-philosophy | speech-act: institutional authority proof. form-linter: contract matching. eastern: nothing |
| **O10** stoicism ≡ existentialism | stoicism names existentialism as a neighbour, the break as an L1 incompatibility | cut identical, conclusion figure opposite. **But:** stoicism's cut is set by a fixed list, existentialism's case by case |

*(Verify note on O10: stoicism contradicts itself internally — Conflicts says "cannot run simultaneously", Interop says "can be run in parallel if the difference in tone is declared".)*

**Balance for eastern-philosophy:** of five residual items from its own subtraction, three are duplicates (O7, O8, O9), one is a prescription. Genuine: **one** operation (O23) — without a performable test.

### Neighbour contradictions (not smoothed over)
- **structuralism** is named as a neighbour by five apparatuses and itself names two. It is the operative core of half the inventory and does not declare that.
- **phenomenology** is named by three and names hermeneutics. Its verify finding shows: the second neighbour (multimodal-analysis) is attributed **against the file** — the file addresses the figure/ground neighbourhood to semiotics.
- **structuralism ↔ content-analysis** name each other — the only mutual neighbourhood **across the tradition axis**, and the only one with a nameable winner (second-coder test).
- **critical-theory → poststructuralism**, but **poststructuralism → structuralism**. Genealogically the enmity is symmetrical; the declared closeness is not.

### The one test for all clusters
**Blind-assignment test.** One artefact, two apparatuses of the same cluster, two analysts, separate runs. Both outputs de-named (proper names and school terms replaced by the generic formulations), presented to a third, blind reader: *which output comes from which apparatus?*

- Chance level → functionally one apparatus with two dialects.
- Above chance → operatively different; the distinguishing features become the routing criterion.

Cost: per pair one artefact, three runs, one blind reader. The four redundancy-suspect clusters are decided with ~20 runs.

---

## 5. Falsifiability gradient

Sorted by hardness of the falsifier. "Falsifier" = a feature on the artefact whose presence overturns the statement.

### A — Falsifier throughout (3)
1. **asemic-pattern-detection** — null hypothesis **before** execution, permutation tests ≥1000, null finding declared as a result. The only one with a pre-registered structure. Limit: the superordinate attribution (structure = producer imprint) is cause-underdetermined, which the file spells out itself.
2. **content-analysis** — κ, recounting, saturation refutation. *(Verify: the fourth, "sharpest" falsifier — resistance segments — has an equal-rank disposal option and does not carry.)*
3. **source-criticism** — anachronism, carrier material, dependency proof; a declared not-decidable case ("uncontrolled"). Weakest point: the tendency reconstruction has no declared falsifier.

### B — Split: checkable periphery, immunised core (7)
The majority — and the place where the periphery supplies the authority for the core.

| Apparatus | checkable | immune |
|---|---|---|
| **speech-act-theory** | authority, uptake, effect that occurred | sincerity; ideal speech situation (counterfactual ⇒ always a deficit) |
| **systems-theory** | loop course, delay, functionally equivalent substitute | observation/contingency core; lever ranking (brought along) |
| **pragmatism** | Prompt 2: evidence question + test step | L1; Prompt 1 ("no difference identifiable" is analyst-relative) |
| **artifact-triage** | profile, quote fidelity, catalogue existence | **the assignment — that is, the purpose**: "a recommendation, not a constraint" |
| **semiotics** | index typing (narrow: only absence of the binding); reception claim against audience data | myth operation (constructive). *(Verify: the blank-space claim, too, is a sociological claim without a checking authority)* |
| **phenomenology** | four-case typology against the defined cases | core description (epoché excludes third-person evidence); essence claim. *(Verify: breakdown and loss claims are diligence criteria, not falsifiers)* |
| **structuralism** | sequence claim (but softened by "functional equivalents") | deep-structure thesis; mediation statement. *(Verify: the substitution test has no adjudicating authority)* |
| **multimodal-analysis** | channel inventory (positive direction only), single decisions, contradiction claim, omission when the source is present | three-task assignment; attribution of interest |

*(This row contains 8 — multimodal-analysis lies between A and B; the checkable points are more numerous than in the other B cases, the core test is absent.)*

### C — Apparent or no falsifier (9)
- **critical-theory** — "Whose interests does it serve?" permits no "none"; `incorporate` books absorption *and* repulsion as confirmation. *(Verify: the two sharp falsifiers claimed in the extraction do not carry — Op. 5 is presuppositive, Op. 2 imperative.)*
- **postcolonial-theory** — "always already macro-level" + "an implicit Western norm": the single item can refute nothing. The file reports the objection ("risks reinscribing the silencing it critiques by making it theoretically insurmountable") and does not decide it.
- **feminist-theory** — L1 as declared predecisions; every neutrality claim is rebooked in advance as an "encoded standpoint". Self-disclosure: "does not generate automatic predictions".
- **poststructuralism** — if "every system of meaning harbours internal contradictions", the find is guaranteed before reading; failure counts as "not yet read closely enough".
- **hermeneutics** — "fusion of horizons" has no feature whose absence would refute it; the checker is, per L1, co-biased.
- **existentialism** — both outcomes confirm. Fully closed.
- **eastern-philosophy** — every counter-example is read as a further web of conditions; the two-level operation catches every objection on the other level. *(Two operations permit, by their wording, a null finding — the apparatus is not entirely closed.)*
- **stoicism** — *(Verify: the extraction reported a falsifiable sorting; the file sets the assignment by a fixed list. Unfalsifiable on both levels.)*
- **form-linter** — declares its own non-falsifiability: "The discriminator … is judgment-based, not yet operationalized"; marker absence expressly does not exonerate.

### Balance
| | n |
|---|---|
| Falsifier that meets a severity requirement | **3** |
| Split (only periphery testable) | **8** |
| Not testable | **9** |
| carries `evaluative-normative` | 14 / 20 |
| `normative: no` | 5 (structuralism, phenomenology, content-analysis, artifact-triage, asemic) |
| statement kinds **only** [descriptive, relational] | 3 (content-analysis, artifact-triage, asemic) |

**The finding beyond the individual rows — falsifiability laundering.** content-analysis declares in its own interop the passing-on of its numbers to the evaluating apparatuses ("The coded category distribution is a direct input for Critical Theory → ideology critique"). source-criticism passes on its tendency finding. phenomenology passes on its forced loss column. The three falsifiable apparatuses are, by blueprint, the suppliers of the nine non-testable ones. "In 40 of 60 texts X is missing" is reproducible; "that is systematic silencing" is not — but it inherits the authority of the count. **Carried as a conflict in no file.**

---

## 6. Residue finding

What remains after subtracting the proper names and the school vocabulary? Here proper names are the object.

### Vocabulary, not method

| Apparatus | Finding |
|---|---|
| **eastern-philosophy** | Five residual items: two duplicates (O7 ≡ systems-theory without notation; O8 ≡ phenomenology suspension — declared by the file as an "independent discovery of the same methodological move"), one a prescription. Genuine: **one** operation. For that, eleven thinkers, ~40 transcriptions, six prompt sections. Additionally, the file says itself it is not an analytical method ("cannot serve as a systematic analytical method") — misrouted as an analytical apparatus. |
| **postcolonial-theory** | Four prompts collapse after subtraction to **two** (1≡3, 2≡4 — the overlap is described in the file). Four of the eight head thinkers carry zero operations. **The most expensive case:** the only jurisdiction gate hangs on the proper name ("not a universal cognitive error but a historically specific discursive formation"). De-name it without replacement and the apparatus becomes a universal suspicion. The genealogy here carries the application lock, not just prestige. |
| **existentialism** | The operations survive, their **justification does not**. Three tripartitions — why three and not four is nowhere stated as an argument, only as authorship. Grid authority from attribution. Two head thinkers never appear again. |
| **feminist-theory** | Two of the four procedures (O4 situatedness, O5 absence) are congruent with postcolonial-theory and source-criticism — the file says "maps directly onto". Own: O1 decomposition + O22 crossing. One declared L2 object has **not a single prompt step**. *(Verify: the balance "four procedures, no more" is not tenable against the file — at least three further prompt steps are neither catalogued nor marked as genealogy. The yield balance is an over-claim.)* |
| **semiotics** (partial) | Two head thinkers do not appear in the remainder **a single time**. The triply declared main conflict axis is a dispute over ways of counting ("two parts or three?") — the file half-concedes its inconsequence ("The two can complement each other operationally (L3) but not ontologically (L1)") and gives it more declaration surface than any single operation. The yield (O20) stands as a sober list item; the one recommended is the only unfalsifiable operation. |
| **critical-theory** (half) | Four of the nine head thinkers: zero operations. After subtraction the apparatus falls into **two unequal halves** — one that checks and one that brings along its result. Held together only by the family tree. *(Verify: the L2 layer is already name-free in the file — the labels sit in the header, key concepts, prompt titles, role line.)* |

### Survives the de-naming
content-analysis ("the practitioner loses zero steps"; L2 objects carry no author name), asemic-pattern-detection (names as shorthand for spelled-out computational procedures), source-criticism ("the estate is strikingly small — that is the finding"), form-linter (declares its own names as after-the-fact framing, n=1), artifact-triage (has no genealogy — no tradition field, no thinker field, no personal name in the file), speech-act-theory, pragmatism, phenomenology, multimodal-analysis, systems-theory (2/3), stoicism (six hands-on moves), structuralism (~1/2).

### The mediating variable
The naive thesis "little residue ⇒ no falsifier" has clean counter-examples: stoicism (six hands-on moves, no core test), phenomenology (five, immune core), form-linter (zero genealogy load, self-declared undecidable discriminator). What matters is not name density but **what the name carries**:

| What the name carries | Residue | Falsifier | Cases |
|---|---|---|---|
| **Recipe attribution** (who standardised the procedure) | high | hard | content-analysis, asemic, source-criticism, structuralism, multimodal |
| **Value-setting without procedure** (the licence to conclude) | high | none | stoicism, phenomenology, form-linter, speech-act (one prompt step), systems-theory (one part) |
| **Ontological predecision** (a brought-along answer about the world, declared as L1) | **low** | **none** | eastern-philosophy, postcolonial-theory, existentialism, feminist-theory, critical-theory (half), poststructuralism, hermeneutics |

The third row has a hallmark: the L1 is not the premise of a procedure but the conclusion, anticipated — "nothing is neutral", "nothing exists independently", "freedom cannot be escaped", "power is productive", "colonial structures are always already macro-level". Because the answer is already there, no procedure that works it out is needed — hence the small residue. Because the answer is already there, no artefact can topple it — hence the missing falsifier. One defect with two symptoms, not two correlated ones.

In this class the proper name is not ornament but the load-bearing structure: it replaces the justification that the procedure does not supply.

*(Hedge: the assignment is a reading of the files. The cells of the first and third rows are each supported by at least two independent features — name density in the operative part + the formulation grammar of the L1. The second row is the weakest: it gathers heterogeneous cases.)*

---

## 7. Coverage gaps

**Modality × scale** — cells with carriers (not apparatuses that merely formally trigger):

| | Single item | Corpus |
|---|---|---|
| **text** | dense (17) | 6 |
| **institution/practice** | 11 | 3 |
| **interaction/transcript** | 8 | **1** (content-analysis) |
| **image** | **2** (multimodal, semiotics) | **1** (asemic — and only asemic) |
| **mixed-media** | **1** (multimodal) | 2 |
| **sound / moving image** | **0** | **0** |
| **number / log / table** | **0** | **0** |
| **code / specification** | **0** | **0** |

Five findings:

1. **Everything numerical.** 19 of 20 files list it in their own idle field — and yet produce prose there. The only counting apparatus codes language.
2. **Sound and moving image.** No apparatus lists the modality. multimodal-analysis names sound as a channel and blocks itself: "developed for static print media", audiovisual "not fully capture[d]".
3. **Image without a second channel and without a corpus.** multimodal needs ≥2 channels, semiotics a reconstructable meant, asemic quantity. A single photo without text falls through all three.
4. **Transcript corpus: one cell, one inhabitant.** speech-act-theory declares itself "methodologically insufficient for discourse analysis … across large bodies of text"; content-analysis can do quantity, not enactment. **The crossing quantity × enactment is unoccupied.**
5. **Effect.** No apparatus measures it. Four files (semiotics, multimodal, critical-theory, postcolonial) declare the reception gap and refer to one another for it — in a circle. semiotics names its own limit verbatim: "outputs Hall cannot use without audience data". **This is the falsifier that three apparatuses name for their main finding and none serves.**

**Output forms.** Of 20 apparatuses, 2 output a measured value with significance (content-analysis, asemic), 2–3 a reproducibility measure, 0 a forecast (systems-theory expressly excludes it), 0 an effect size. The inventory reads; it measures at two edges of the material.

**The missing operation.** Not a further apparatus, but **an abort condition as a pipeline stage**: an upstream test that checks whether the artefact *meets* the `precondition` of the chosen apparatus, and on non-fulfilment refuses the output. The blueprint exists twice — artifact-triage refuses without a catalogue ("do NOT route"), asemic refuses without a segmentable unit ("declare and refuse rather than force-fit"). **Both refusal gates sit in non-genealogical files. No interpretation apparatus has one.** And artifact-triage itself routes on the *Key Analytical Question* but never checks the precondition of the target apparatus — the heuristics are assignment settings without a success condition ("a recommendation, not a constraint").

**Docking points for this catalogue** (from the routing inventory, not newly invented):
- The catalogue that `artifact-triage` §7 demands as a gate ("is a prompt-library framework catalog … present in your context?") does not exist as an artefact. `docs/taxonomy-review-schema.md` is the nearest (16 frameworks × L1/L2/L3 + D1–D3), but framed as a review checklist and expressly anti-functional ("not classification into fixed categories"). **The gate has no designated referent.**
- The question axis in `artifact-triage` §6 is declared and underpinned: only 2 of 10 heuristics are question-shaped, the rest are type/modality/scale predicates. The docking point is §7's heuristic list, not a new file (`skills/triage.md` l.150: single-source rule).
- `docs/instantiation-patterns.md` sets the evidence bar for a new classification class: "documented from repeated instances, not invented from single ones", n=2. Whether an external question matrix (business questions) + artifact-triage §6 (analytical questions) count as two *independent* occurrences is a judgement, not a fact in the files.
- **Functional axis ⊥ conformity axis, unreconciled.** A functional catalogue routes onto apparatuses that are declared-but-not-conformity-checked (9 of 16). Nothing in the repo says what routing onto a deferred framework means.

---

## 8. What this catalogue does not prove

**This is a reading of 20 files, not a test on artefacts.** Every statement here is derived from prompt text, not from observed output. Concretely:

1. **The collision claims (§4) are hypotheses.** "Eight apparatuses do the same thing" means: their prompt steps can, de-named, be brought to the same formulation. Whether two runs on one artefact produce distinguishable outputs is **open**. Decisive test: the blind-assignment test (§4). Cost for the four redundancy-suspect clusters: ~20 runs.

2. **The reads-past diagnoses (§3) are forecasts from prompt grammar.** Where a file declares them itself (multimodal, stoicism, eastern-philosophy, form-linter, structuralism institution op, content-analysis), the finding is evidenced. Where not (critical-theory, feminist-theory, hermeneutics, phenomenology, systems-theory, poststructuralism), it is **derived** — the Conflicts sections of these files carry theory conflicts, not failure modes. Decisive test: the benchmark artefact (a documented, working repair with an open error correction), blind through all 14 evaluating apparatuses. Forecast: 14 positive findings.

3. **The falsifiability gradient (§5) is nowhere empirically checked.** "Falsifiable" here means: the file names a test point whose outcome lies on the artefact. Whether the test in a real run actually leads to a negative verdict is untested. In five cases (structuralism, critical-theory, stoicism, phenomenology, semiotics) the verify findings have retracted claimed falsifiers as analyst-relative or presuppositive — class A is therefore smaller than a first reading suggests, and further retractions are possible.

4. **The residue assignment (§6) is n=1 per file.** The subtraction is a thought experiment ("strike the names — what remains?"), not a run with a de-named prompt. Decisive test: implement one of the class-3 apparatuses de-named (all proper names and school terms replaced by the generic formulations) and run it against the original. If the de-named run delivers the same, the name was ornament; if it collapses, it was load-bearing structure. For postcolonial-theory the forecast is collapsing (the gate hangs on the name) — it is not tested.

5. **The laundering argument (§5, Balance) is a blueprint reading.** The interop lines say the number is passed on. Whether the consumer actually inherits the authority of the number in a real run is not observed. Decisive test: hand content-analysis output to critical-theory, repeat the same critical-theory run without the number, compare verdict hardness.

6. **Status limits.** 16 apparatuses stand at `in-test`, 2 at `draft`. `in-test` permits the claim of DFS (Declarative Frame Schema) conformity (eight components declared) and "in use" — **not** that of output validity ("not yet validated by Discovery Session"). `draft` does not even permit the conformity claim. Additionally: as long as `SCHEMA.md` itself stands at `in-test`, no prompt that form-adopts generation 2.0 can, per the foundation-stability gate, be `stable`. This catalogue claims no more about any apparatus than its status permits.

7. **Not captured.** `artefact-triage/skills/` and reference files declare no DFS components and are not a DFS object — they are not catalogued here. The sequencing rules (source criticism first; multimodal in parallel; interpretive after; critical third or later) lie a layer above the apparatuses and are not checked here.

8. **Contraindications are empirically empty.** `artifact-triage` standard emits Primary/Secondary/**Contraindicated**, but only the minimal variant has ever run — the negative half of every functional catalogue has no data basis.
