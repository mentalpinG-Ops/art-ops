---
name: operations-spec
version: 0.5.1
status: draft
last_changed: 2026-07-19
---

<!-- 0.5.1 (2026-07-19): full EN translation of the entire file (prose, tables, HTML comments) —
     translation only, no content added, dropped, or reinterpreted; British spelling "artefact".
     Header version bumped 0.5.0 → 0.5.1.
     [AI+] full EN translation per author decision 2026-07-19. -->

<!-- 0.5.0 (2026-07-19): O19/O12 authorship test entered (§5, under the screening) —
     o19-o12-urheber-2026-07-18 + gnomic follow-up test 2026-07-19: O19 real-but-probabilistic
     exposed (0/3 on easily-attributable, 1/3 unanimous on gnomic material); O12
     robust across both material tiers (0/3 both). Balance carried forward: O19 confirmed (not
     refuted), O12 practically relieved despite identical "high" rank. Open: mitigated
     cells B19g/B12g (next cheap step), O7/O9 still untested.
     MINOR: one test finding adds its first result to an existing candidate list;
     no structure broken, no table cell changed.
     [AI+] Claude, author commission as maintainer upkeep, drift-fix direct commission 2026-07-19.
     Evidence: test run o19-o12-urheber (internal test documentation) (+ gnomic/). -->

<!-- 0.4.0 (2026-07-19): O8×O2 (§3.2 D2) EMPIRICALLY REFUTED — first decided test result
     (o8-knot-v3, C 3/3 + A both 3/3 + GATE 6/6 + AC1 1.0). The two-clause fix (0.3.0) made O8
     fully instructable; the collision was an artefact of the underdetermined instruction.
     D2 struck through + §8 status carried forward. First tested conflict of the register, does not hold;
     supports the ~63%-inconsequential thesis with 1 data point. K2 class as a whole still untested.
     [AI+] Claude Opus 4.8 on author commission; finding from the test run.
     Evidence: test run o8-knot-v3 (internal test documentation) -->

<!-- 0.3.0 (2026-07-18): marking clause added to the authorship rule (§5) — from PRACTICE

<!-- 0.3.0 (2026-07-18): marking clause added to the authorship rule (§5) — from PRACTICE
     (test run o8-knot-v2-2026-07-17, again VOID for H1, but GATE 5/5 and a more precise finding):
     the authorship rule (0.2.0) repaired the rubric, not the runner; an unmarked rendering
     collapses at the output into one's own voice. Second clause: a rendering must be marked.
     MINOR: an existing rule extended by a necessary condition; no structure broken.
     [AI+] Claude Opus 4.8 on author commission; finding from the test run, not from prior knowledge.
     Evidence: test run o8-knot-v2 (internal test documentation) -->

<!-- 0.2.0 (2026-07-17): authorship rule for "no X" prohibitions entered (§5) + O8 profile corrected
     + screening of all 23 remaining operations for the same exposure (10 exposed, 4 high:
     O19/O12/O7/O9) + §8 extended by the status after the first material contact.
     MINOR: one condition was tightened, one rule + one candidate list were added;
     no structure broken, no profile re-cut.
     Provenance mixed, deliberately kept separate:
       - authorship rule + O8 correction = from PRACTICE (test run o8-knot-2026-07-17, VOID) —
         the only lines of this spec so far that do not derive from reading.
       - screening of the 23 = from READING. It exposes, it does not decide. Marked as a candidate
         list, expressly not as a finding.
     Evidence: test run o8-knot (internal test documentation)
     [AI+] Claude Opus 4.8 on author commission; finding from the test run, not from prior knowledge. -->


# Operations without Genealogy — Spec

> **Move 2026-07-17 (cut, not a copy).** This file previously sat as an
> internal methodology note in the
> internal work area and has been **moved** here; only a pointer remains there.
> Reason: as the tool's **operating basis** it
> belongs in the repo that carries it. A cut rather than a copy, so that no two versions drift.
>
> **Relation to the catalogue:** [`catalogue.md`](catalogue.md) holds the apparatus→operations map
> (which apparatus performs which move); this spec holds the **profiles** of the operations
> (what each requires of the material and of the analyst, what it produces, what it forbids) and derives
> conflict and interop from them **mechanically**. The catalogue is the inventory, the spec
> the mechanism. For the tool's selection logic the spec is the load-bearing file.

## 1. What for

24 operations, de-named from 21 prompt files. An operation is defined by: what it requires of the **material**, what it requires of the **analyst**, what it **produces**, what it **forbids**.

The apparatus level cannot do three things: (a) it indexes conflicts as framework × framework, while the real collisions are operation × analyst-state; (b) it knows no classes — a collision with ~27 instances appears twice; (c) for unary constraints (repeatability, circularity within one operation) it has no cell. The operations level produces conflict and interop **mechanically** from four fields, instead of declaring them.

---

## 2. The mechanism

Every profile carries four fields plus `repeatable`:

| Field | Content | Checkable on what |
|---|---|---|
| `requires_material` | states of the artefact before the run | on the artefact |
| `requires_analyst` | states of the analyst before the run | **on the finished output** — a condition that can only be formulated as a disposition ("readiness", "knowledge") is none |
| `produces` | states that obtain after the run and are transferable | on the output |
| `forbids` | what cannot run simultaneously, with hardness `hard` / `soft` | on the output |

**Interop falls out mechanically:** A → B exactly when an item from `A.produces` covers an item from `B.requires_*`. The edge is directed, the migrating state is nameable. No judgement, a match.

**Conflict falls out mechanically:** A × B exactly when an item from `A.requires_analyst` is the negation of an item from `B.requires_analyst`, or when `A.forbids` names a state that B establishes. Three types:

- **K1** — a state from A.requires is destroyed or pre-empted by B. Resolution: ordering.
- **K2** — the two analyst-states cannot be present in one person simultaneously. Resolution: separate passes.
- **K3** — A is not repeatable after its own performance. *Empty in the present stock* (see §8).

**Hardness:** `hard` = one of the two operations becomes invalid (its defining output can no longer be shown). `soft` = both remain executable, one is distorted or shortened.

The load-bearing test is not "can both be sequenced?" — that lets every state collision through. It is: **can the same analyst hold both states in the same pass?**

---

## 3. Conflict register

Only cases where simultaneity makes an operation invalid or distorts it. Prohibitions that the adversarial review discarded as a `blocker` are barred as a conflict source (O2.fb[4], O7.fb[2], O8.fb[4] incl. its `no-single-use`, O9.fb[0] recommendation clause, O16.ra[5], O21.fb[3]).

### 3.1 Undeclared — hard

| # | A × B | Type | Hardness | Resolution |
|---|---|---|---|---|
| U1 | **O8 × O22** — suspend / crossing of markers against a brought-along list | K2 | hard | O8→O22 |
| U2 | **O8 × O9** — suspend / hold a brought-along checklist | K2 | hard | O8→O9 |
| U3 | **O8 × O15** — suspend / assign a position set | K2 | hard | O8→O15 |
| U4 | **O8 × O12** — inside performance / interpretation-free outside classification | K2 | hard | O12→O8 (O12 is `only-before-others`) |
| U5 | **O8 × O5** (counter-concept/position variant) | K2 | hard | O8→O5 |
| U6 | **O7 × O10** — no part stands alone / person as the site of movability | K1+K2 | hard | **not by ordering** — both posit the attribution direction as their frame. Only separate passes with declared precedence |
| U7 | **O13 × O13** — first-person ranking / outside-classification ranking | K2 | hard | choose one version; the rankings are not additive |
| U8 | **O18 × O24** — version differentiation presupposes descent / the independence check determines it | K1 | hard | O24→O18, or O18 delivers the descent finding to O24 — not both in the same ring |
| U9 | **O16 × effect finding** — mode of address read back from observed effect | K1 (unary) | hard | carry the two effect magnitudes separately into the pass |
| U10 | **O18 × null-finding check** — the operation measures the difference set, cannot establish its absence | K1 (unary) | hard | none — the whether-question gets no outcome |
| U11 | **O18 × direction circle** — derive source/target from the difference list | K1 (unary) | hard | obtain direction knowledge externally (O12) |

**The common knot.** U1–U5 all lie on **O8**: the only operation that requires the *absence* of a brought-along grid. It collides mechanically with every grid-bearing operation (O1, O2, O5, O9, O11, O15, O22) and every outside-positioned one (O3, O12, O24) — ≈27 pair instances. The conflict is a property of the operation; the existing declarations are a property of the file neighbourhood. They do not coincide.

U9–U11 are **unary**: one operation collides with a state, not with a second operation. For this no notation slot exists in the legacy stock.

### 3.2 Declared — hard

| # | A × B | Type | Resolution |
|---|---|---|---|
| D1 | **O8 × O1** — suspend / expose as made | K2 | O8→O1 |
| ~~D2~~ | ~~**O8 × O2** — suspend / hold a compartment list~~ **→ EMPIRICALLY REFUTED 2026-07-19** (`o8-knot-v3`): no conflict. One agent carries both states in the same pass (A both 3/3, control C 3/3, GATE 6/6, AC1 1.0). The "conflict" was an artefact of the underdetermined O8 instruction, not of the operations. **First tested conflict of the register — it does not hold.** Details: §Tested conflicts below. | ~~K2~~ | — |
| D3 | **O8 × O11** — suspend / count out | K2 | O8→O11 |
| D4 | **O17 × O8** — log a preassumption / suspend a preassumption | K1 | **direction-forced O17→O8**: O8 destroys the quantity that O17 logs |
| D5 | **O12 × O1 / O16 / O17** — status before interpretation | K1 | O12→X |
| D6 | **O24 × O17** — check independence / carry along a preassumption | K1 | O24→O17 |
| D7 | **O11 × O20** — count out under the status "meaning-side not accessible" / sort binding | K1 | **not at all** — O20 requires a reconstructable meant; lifting the status forces a complete re-run |
| Governance decision | **O22 × O11** — crossing effect / count out single effects | K1 | **asymmetric: only O22→O11**. O22 also forbids the *already completed* decomposition |
| D9 | **O11 / O6 × O1** — count or cut / interpret in the same pass | K1 | O6/O11→O1 |
| D10 | **O7 × O19** — web of conditions / tip-over in the experiencer | K1 | O19→O7 |
| D11 | **O7 × O8** | K1 | O8→O7 |

### 3.3 Soft

| # | A × B | Resolution |
|---|---|---|
| W1 | **O10 × O1 / O22** — bipartition / producer finding from outside the situation | precedence declaration, which question governs |
| W2 | **O17 × O2 / O5 / O22** — preassumption shiftable / binding brought-along list | declaration, which side governs |
| W3 | **O3 × O8 / O10 / O19 / O23** — pole assignment from outside / inside position | declaration before merging |
| W4 | **O23 × O14** — locate counter-pressure / propose an intervention | declaration of the target direction |

### 3.4 Discarded (disagreement, not conflict)

O21 × O17/O8 (no analyst-state meets O21.fb[0]); O3 × O5 (O5 consumes O3's pair); O18 × O12; O15 × O3; O13 × O8 (O13's experiential version *is* the O8 state — not a second operation); O10 × O14 (feeding relation).

---

## 4. Interop register

### 4.1 Supply edges

Only edges where an output item of A covers a state of B that B **requires by name**.

| A → B | migrating state |
|---|---|
| O6 → O2 | segmentation = independently assignable units |
| O6 → O11 | delimitable, recognisable counting unit + countable element count |
| O6 → O5 | declared counting/analysis unit |
| O6 → O20 | individually delimitable carriers |
| O2 → O11 | fully assigned stock with kind-marking |
| O2 → O5 | closed distribution + grid against which absence is measured |
| O20 → O11 | kind assignment per carrier |
| O11 → O5 | distribution with declared zero cells |
| O11 → O1 | quantified distribution |
| O9 → O11 | count line per verdict |
| O3 → O5 | fixed pair of opposites (suppressed term) |
| O3 → O1 | fixed pair as a starting point |
| O12 → O4 | established material status |
| O12 → O17 | authenticity/provenance clarified before interpretation begins |
| O12 → O24 | authenticity status per piece of evidence |
| O12 → O18 | provenance/dating datum = direction knowledge source→target |
| O18 → O24 | descent finding of two concurring versions |
| O13 → O18 | channel inventory + ranking = capacity-limit inventory of the target carrier |
| **O24 → O12** | corrected evidence weight / status "uncontrolled" — **back edge** |
| O17 → O1 / O4 / O5 / O15 | logged standpoint note |
| O4 → O5 | centring/omission list |
| O4 → O1 | place finding |
| O15 → O5 | occupancy list + unoccupied positions = voices grid |
| O15 → O22 | named carriers/affected parties with positions |
| O16 → O9 | listing of the load-bearing orders = O9's authority frame |
| O19 → O7 | exposed background web |
| O19 → O1 | finding about the systematically un-noticed |
| O8 → O1 | background foil of the unthematised self-evidences = O1's point of attack |
| O7 → O23 | balancing loop + delay = application→counter-effect across two points in time |
| O7 → O14 | cycle map + ranking of intervention points |
| O23 → O14 | named spot + releasable surplus |
| O10 → O14 | marked approach side |
| O9 → O14 | self-contradiction proof / label-vs-performance list |
| O1 → O14 | divergence of value/performance + exclusion list |
| O5 → O14 | gap list |
| O14 → O21 | spelled-out proposal + competing hypotheses |
| O14 → O22 | named intervention — **weakest edge** (O22 requires an intervention *in* the artefact, not a produced one) |
| **O22 → O5** | gaps in the presentation stock — **back edge** |

**Anti-edge:** O6 → O3 drops out. O6 decomposes precisely the uncut whole that O3 requires.

### 4.2 Partial order

- **Stage 0 (entry points):** O3, O6, O8, O10, O12, O13, O16, O19
- **Stage 1:** O2, O7, O9, O17, O18, O20
- **Stage 2:** O4, O11, O15, O23, O24
- **Stage 3:** O5
- **Stage 4:** O1
- **Stage 5:** O14
- **Stage 6 (endpoint):** O21

O8 and O19 are necessarily stage 0: their preconditions are *negative* — any supply would be disqualifying. They are structurally unsuppliable, not undersupplied. O21 is the only sink: no profile requires a revision proviso or a null finding as input.

**Cycles (2):**

1. **O12 ↔ O24** — genuine. O24 requires an established authenticity status (O12); O12's reliability/robustness stage requires O24's output. At the operations level **not resolvable**; only at stage granularity: O12.authenticity → O24 → O12.reliability. Side finding: O12's robustness stage *is* O24 — the profiles overlap in the output.
2. **O5 → O14 → O22 → O5** — conditional. Holds only under a wide reading of O14→O22. Under a strict reading the edge drops, O22 moves up to stage 3.

**No orphan.** All 24 are connected. But accessibility is unequal: O19 costs nothing (entry), O21 costs five stages. O23 hangs on a single supplier (O7).

---

## 5. The operations table

| id | Operation | requires material | requires analyst | produces | forbids (hard) | rep. | Origin |
|---|---|---|---|---|---|---|---|
| **O1** | Expose what presents itself as self-evident as made | citable passage without justification; literal/connotative level separable | predecision "made" before the material; declared own position; external knowledge | localised passage; construction claim + beneficiary; exclusion list; counter-reading; **verdict only where positive** | suspending (O8); positionlessness; **use as a checking instance** | yes | semiotics, critical-theory, poststructuralism, postcolonial, feminist, systems, pragmatism, structuralism |
| **O2** | Hold a ready-made compartment list up to the material | >1 assignable unit; stock large enough for a distribution; genre homogeneity | ready-made closed list (definition + anchor + boundary rule per compartment); declared origin; **NO suspending** | distribution; gap list; remainder; assignment map; log | suspending (O8); mixing with a substantive conclusion | yes | content-analysis, structuralism, speech-act, phenomenology, existentialism, stoicism, form-linter, artifact-triage, asemic |
| **O3** | Extract the load-bearing pair of opposites | coherent whole; both poles evidenced in the material; attributions per pole | pair fixed as load-bearing; descriptive/evaluative decided in advance; outside position | pair with clusters; marked/unmarked; belonging/exclusion; middle positions | simultaneous destabilisation of the pair | only-before-others | structuralism, semiotics, poststructuralism, feminist, (systems: unevidenced) |
| **O4** | Trace a neutrally-presenting statement back to its place of production | statement with a neutrality claim; reconstructable production situation; an indication of interest | brought-along axis; context knowledge; **EITHER** declared own position **OR** declared non-identification | provenance attribution; suspended neutrality status; centring/omission list | carrying a position along AND claiming observer neutrality; positing the place as an effect of the discourse | yes | feminist, postcolonial, source-criticism, critical-theory, systems |
| **O5** | Register absence as a finding | *counted variant:* delimited whole + counting unit; *counter-concept variant:* a text | named grid; logged grid origin | gap list per grid; zero cells declared; unoccupied voice positions; suppressed term | suspending (O8); retroactive deletion of categories that stayed empty | yes | content-analysis, feminist, postcolonial, poststructuralism, semiotics, structuralism |
| **O6** | Cut into smallest self-contained parts | multi-part; fixed, citable version; surrounding context present | declared cutting unit + surrounding-context reach + reference quantity; **state-lean** | segmentation; cutting criterion; countable element count; ordering; remainder | rewriting the material; inferring in the same pass; simultaneous contesting of boundaries | yes | structuralism, semiotics, content-analysis, form-linter, asemic, critical-theory, feminist, hermeneutics, existentialism |
| **O7** | List the web of conditions; no part stands alone | named occurrence; >1 element; ≥1 effect relation; temporal course | positing "no element exists independently"; framing self-set + declared; no attribution of intent | list with a condition per element; reciprocal conditioning; declared boundary; contingency finding; *noted:* intervention ranking | positing an instance as an unconditioned starting point | yes | systems-theory, eastern-philosophy, pragmatism |
| **O8** | Suspend one's own categories; describe only | single concrete incident as a course; accessible from the position of the affected person; variable | **no** brought-along list; **no** fixed explanation **of the analyst**; inside position; no value judgement **of the analyst** — evaluations and explanations that **the source itself** carries may be rendered and do not violate the condition (see authorship rule below the table) | description without explanation **of the analyst**; foreground/background; temporal articulation; background foil; invariant features | compiling one's **own** list; carrying along one's **own** fixed explanation; outside position | **yes** (single-occurrence was a blocker) | phenomenology, eastern-philosophy |
| **O9** | Check whether the presentation is covered by the substance | presentation and performance separately determinable; producer; coverage claim; external reference point | brought-along checklist; contract/frame passage named; declared observer stance; verdict set with "undecidable" | coverage balance per occurrence; conditions balance; misfire/abuse bipartition; authority status; count line | repairing in the same pass; attribution of intent/being; gate decision at the lowest maturity level | yes | speech-act-theory, form-linter, eastern-philosophy |
| **O10** | Split the situation into fixed and influenceable | described single situation; >1 element; named carrier; reaction datum | cutting rule noted in advance; declared inferential figure | bipartition without remainder; misassignment list; marked approach side | two cutting rules at once; a third bin | yes | stoicism, existentialism |
| **O11** | Count the kinds; hold the distribution against chance | >1 countable unit; delimitable, stable counting unit; assigned stock | comparison model **in writing before** the run; output format with non-discard; saturation state | frequency distribution + ranking; test result (test statistic, df, p, decision); blanks; summary statistics; boundary statement | choosing the model after inspection; interpretation in the same pass; meaning attribution under the status "not accessible"; order test without a fixed sequence | yes | content-analysis, asemic-pattern-detection |
| **O12** | Fix the material's status before interpreting | single piece with determinable carrier form; provenance claim | **no** ongoing interpretation; **no** brought-along meaning explanation; outside position; period knowledge | material status (primary/secondary/fabrication/unclarified); authenticity note; credibility calibration; descent determination; licence statement | interpretation; exploitation before authenticity; perspective adoption; meaning from intent | only-before-others | artifact-triage, source-criticism |
| **O13** | Inventory the channels; state their ranking | artefact in its original version; centre/surrounding distinguishable; presented as **one** | no advance fixing of the load-bearing channel; a carried-along channel repertoire; **EITHER** interpretation-free-outside **OR** first-person | channel list incl. absent ones; ranking; switch finding single-/multi-channel; foreground/surrounding cut | ongoing interpretation; both versions as **one** ranking | only-before-others | multimodal-analysis, artifact-triage, phenomenology |
| **O14** | Propose an intervention | named gap; identifiable carrier; >1 point of leverage; declared purposes | **a finished external finding** (never the first step); brought-along criterion + origin datum; brought-along depth ranking; disposition attribution | ranked list of points of leverage; retractable proposal + carrier; consequence estimate; refutation condition; means-ends balance | operating without a brought-along criterion; incompatible remediability assumptions without precedence | yes | pragmatism, systems-theory, postcolonial, critical-theory, eastern, stoicism, existentialism |
| **O15** | Assign a person's position/role | identifiable person; attribution utterance→person; ≥2 fillable positions | **logged attribution decision** (person vs. system) before the assignment; **logged** observer stance; for a set: closed position list | occupancy list; unoccupied positions; marked/unmarked; authority status; attribution decision as an output line | person and system attribution at once; outside and inside mapping at once; deriving a position from prior constitution | yes | structuralism, feminist, existentialism, speech-act, semiotics |
| **O16** | Reconstruct the mode of address toward the addressee | readable addressing; the wording/presentation itself; a statable circumstantial frame | knowledge of the authority order; declared reading position; **declared governing addressee model**; effect "designed-in" and "occurred" kept separate | mode of address; gradient form/move; conditions list + failure kind; preferred reading + position; deviant readings; role assignment; load-bearing orders | both addressee models unexplained; effect finding as evidence for the mode of address | yes | semiotics, structuralism, critical-theory, speech-act |
| **O17** | Log one's own preassumption; track its shift | single piece with its own genesis situation; clarified material status; citable contradiction spots | an **existing** articulable expectation; written down **before** the first interpretive step; no treatment as a disturbance variable | dated before-note; shift log; list of contradicting spots; standpoint note | an already performed suspension; simultaneous outside checking of provenance | only-before-others | hermeneutics, feminist-theory |
| **O18** | Differentiate two renderings of the same content | both versions accessible simultaneously; distinguishing non-content feature; **direction datum**; material form of both | direction knowledge **independent** of the difference finding; capacity-limit inventory of the target carrier; assumption that the transformation was not lossless | difference list (missing/added/transformed); assignment to carrier limits (forced vs. chosen); chain with change points; break-point list; descent finding | null-finding check in parallel; deriving direction from the difference list; counting versions as independent pieces of evidence | yes | multimodal-analysis, source-criticism |
| **O19** | Locate the tip-over from unremarkable to remarkable | use **plus** user; temporal course with two states; concurrent references; **no context material** | no fixed cause/frequency explanation; internal position; no causal-statistical vocabulary | two-state segmentation with tip-over point; exposed background web; gaps of normal operation; typing (disruptive/obtrusive/resistant) | concurrent causal explanation; exclusion of the experiencer | yes (hedged) | phenomenology |
| **O20** | Sort sign-binding by similarity / contact / convention | ≥1 delimited carrier; **reconstructable meant**; per case a checkable connection or community | knowledge of the prevailing convention; **declared** arity of the positing; no binding judgement fixed in advance | typology per carrier; interplay for composite material; named community per convention case | two-place model without an explanation of which governs | yes | semiotics |
| **O21** | Check whether a dispute has stakes | spelled-out claim; ≥2 distinguishable outcomes; a nameable field of practice | knowledge of the field of practice (domain named in the output); revision proviso on the finding | stakes finding (difference **or** null finding); translation into the observable; culling; revision proviso; ranking of the versions | in advance: meaning does not resolve into consequences *(hardness disputed — see §8)* | yes | pragmatism |
| **O22** | Test the crossing of several belonging-markers for an effect that arises only there | ≥2 markers on the same cases; nameable affected parties; material conditions; material on three levels; named intervention; presentation stock | brought-along marker list (**open**, not exhaustive); dimension tripartition; level tripartition; partisanship to centre the perspective; **no blinding** | crossing effects; affectedness ranking; gaps in the presentation stock; three-level assignment; single-axis harm list; **no forecast** | single-effect decomposition (including a completed one); suspending (O8) | yes | feminist-theory |
| **O23** | Find the spot where pressing produces the counter-pressure | ongoing application of force with an author; counter-running effect **afterwards**; ≥2 points in time; not-operating conceivable | inside position; **no** fixed strong/weak assignment; no continuation commitment; access to the course | named spot (application→counter-effect); reversal assignment; counterfactual description; releasable surplus | a strong/weak assignment fixed in advance | yes (hedged — `no-single-use` unevidenced) | eastern-philosophy |
| **O24** | Check the independence of concurring pieces of evidence | ≥2 pieces of evidence with a point of agreement; overlap region; provenance datum per piece; predecessor nameable or determinable as not findable | knowledge of transmission paths (predecessor candidate named in the output); outside position; no commitment "agreement = confirmation" | independence classification (convergent/derived + predecessor); corrected evidence weight; divergence explanations; status "uncontrolled" / "formally impossible"; undecidable pairs | a performed meaning interpretation; perspective adoption | yes | source-criticism |

### Authorship rule for prohibitions of the form "no X"

*(Entered 2026-07-17 on a test finding — the only change to this spec that stems from practice and not from reading.)*

**Every prohibition of the form "no X" must name the author of X.** What is always meant: **X introduced by the analyst.** If the source itself carries X and the analyst renders it, the condition is **not violated** — **provided the rendering is marked as such** (quotation, paraphrase, "the source says…"). *An unmarked rendering violates the condition*, because at the output it cannot be distinguished from an X of one's own.

**Two clauses, both test-evidenced, both necessary:**
1. **Authorship clause** (from `o8-knot-2026-07-17`): the source's evaluation/explanation is permitted — the prohibition applies only to the analyst.
2. **Marking clause** (from `o8-knot-v2-2026-07-17`): the permitted rendering must be **marked**. Without marking it collapses at the output into one's own voice, and the checkability test (§2: "can a third party establish at the output whether the condition was met?") fails again — at exactly the spot that clause 1 does not reach.

**Why both (the v2 finding):** clause 1 alone repaired the *rubric* (the judge then distinguished marked-rendered from one's own explanation, GATE 5/5), but did **not** rescue the positive control (1/3): the runner melted the source's judgement *unmarked* into its own voice ("It is a negligent guard…" instead of "the report calls the guard negligent"). The existing cell and the constructed G5 baseline marked — and passed. The difference is the marking, not the occurrence. **Clause 1 is necessary, not sufficient; only both together make the condition followable AND checkable.**

**Why the rule is needed.** The first test of a derived claim of this spec (`o8-knot-2026-07-17`, K2 class O8 × O2) came out **VOID**: the positive control — O8 alone, without disturbance — carried its own item in **0 of 3** cells. The cause, quotation-evidenced in all three cells: the test material was a first-person report whose narrator interprets himself (*"Hunger and thirst are powerful antidotes to fear"*). The describers rendered such sentences **faithfully**; the blinded reviewers scored them as *explanation* or *value judgement*. **Both were right** — the profile did not distinguish whose evaluation is prohibited.

**The defect type.** On material that interprets itself, *the analyst evaluates* and *the analyst reports the source's evaluation* coincide at the output. Thus the condition does not pass this spec's **own checkability test** (§2: *"can a third party establish at the finished output whether it was met?"*) — it is neither followable nor checkable, and self-interpreting material is the normal case with reports and protocols, not the special case.

**Origin of the finding — and why it stands here:** the adversarial text review of this spec found **six** blocker prohibitions and overlooked this one. It becomes visible only on the material. That is the limit of reading as a generation procedure: it finds what stands wrong in the text, not what arises on the object.

**Applied:** O8 (§5, all four affected fields).

### Screening of the remaining 23 operations — candidates, not verdicts

*(Reading pass 2026-07-17. What reading can do: **expose**. What it cannot do: **decide** — that was the lesson of the run that forced it. Every line below is a test case, not a finding.)*

**The discriminator is not the form "no X", but who can perform X:**

- **Immune** — the prohibition names a **preparatory or procedural act** of the analyst ("choosing the model after inspection", "compiling a brought-along list", "no blinding", "two cutting rules at once"). A source cannot supply it; at the output the author is unambiguous.
- **Exposed** — the prohibition names a **content act** that the source too performs: *explain · evaluate · interpret · attribute intent · take a perspective · assign strong/weak*. If the analyst reports it faithfully, the output looks **identical** to a violation of one's own.

| Op | exposed spot | Why | Rank |
|---|---|---|---|
| **O19** | "no fixed cause/frequency explanation"; forbids "concurrent causal explanation" | **O8's twin** — the same inside position, the same defence against explanation. If the source explains causally, the import is unavoidable. At the same time a **solo operation** (carries discriminative power that no other provides). | **high** |
| **O12** | requires "no ongoing interpretation"; forbids "interpretation", "perspective adoption" | If the source interprets itself, its rendering is not distinguishable from "interpretation". **And O12 is `only-before-others`** — the entry gate. If it hangs, everything behind it hangs. | **high** |
| **O7** | "no attribution of intent" | If the source attributes an intent to someone (anchor case: *"which the captain had thoughtlessly strewn among them"*), the rendering is an attribution of intent verbatim. | **high** |
| **O9** | forbids "attribution of intent/being" | the same class as O7. | **high** |
| **O24** | forbids "a performed meaning interpretation; **perspective adoption**" | To *report* the source's perspective is hard to separate from its *adoption* at the output. | medium |
| **O23** | "**no** fixed strong/weak assignment" | If the source itself assigns, the rendering becomes an assignment. Inside position like O8. | medium |
| **O11** | forbids "interpretation in the same pass"; "meaning attribution under the status 'not accessible'" | If the analyst counts out units that the source already interprets, the interpretation migrates along. | medium |
| **O13** | forbids "ongoing interpretation" | like O12, but without gate position. | medium |
| **O15** | forbids "deriving a position from prior constitution" | If the source itself assigns positions, the rendering is hard to separate from the derivation. | medium |
| **O6** | forbids "inferring in the same pass" | If the source draws conclusions and the cut renders them — the same doubt, weaker. | low |

**Not exposed (13):** O1, O2, O3, O4, O5, O10, O14, O16, O17, O18, O20, O21, O22 — their prohibitions throughout name preparatory/procedural acts or simultaneity locks that only an analyst can trigger.

**Balance: 10 of 23 exposed, 4 of them high.** The authorship rule above applies **generically** to all — that is why it is formulated as a rule and not as an O8 special case. The ten lines are its test reserve, sorted by rank.

**Express limit of this screening:** it says where the defect **can occur**, not where it occurs. With O8 the exposure was likewise readable from the text — that it actually struck in **3 of 3** cells was shown only by the material. **O19 and O12 are the next tests**, not the next corrections.

**Evidence:** `test run o8-knot (internal test documentation)` — `phase-3` (adversarial review 4+5, GATE 4/4, AC1 0.901) · `phase-4` (Claim C-2) · `raw/arm-C*.md` (the cited spots). The test is thus **repeatable, but not yet repeated. (AC1 = Gwet coefficient of inter-rater agreement; 1.0 = perfect unanimous agreement.)**

> **Status after material contact: O19/O12 (2026-07-18/19).** The two "next tests" named above have run (`o19-o12-urheber-2026-07-18` + gnomic follow-up test `2026-07-19`). Result, two-tiered by material difficulty (easily-attributable with explicit "I believe" markers vs. gnomic, marker-free like the O8 test case):
>
> - **O19 — really reachable, probabilistic, not dominant.** On easily-attributable material: **0/3 collapse**, GATE 6/6, AC1 1.0 — the defect did not occur. On gnomic material, same runner, same operation, only the material difficulty changed: **1/3 unanimous collapse** (the source's causal sentence migrates unmarked into one's own description). The null finding of the easy tier was **material-dependent, not knot-dependent** — the "high" exposure is thereby **confirmed, not refuted**, but probabilistic instead of the 3/3 full collapse that O8 showed.
> - **O12 — more robust than its rank.** **0/3 collapse on both material tiers** (6/6 clean cells in total), despite an identical "high" rank to O19. The screening exposure is a possibility statement, not a collapse prediction — O12 shows that "high" must not be confused with "equally likely". Provisionally relieved (2 material instances, n=3/cell), the a-priori rank itself remains unrevised.
> - **Consequence for the balance above:** O19 remains on the high list, now with a test finding instead of a conjecture. O12 remains formally listed there, but is practically relieved.
> - **What remains open:** the mitigated cells (authorship rule actively demanded rather than spontaneously followed) have not yet been run (B19g/B12g) — next cheap step (gnomic-result.md phase 4). O7 and O9, the other two "high" cases, are still untested.
>
> **Evidence:** `test run o19-o12-urheber (internal test documentation) (`phase-0`…`phase-4`, `gnomic/gnomic-result.md`). [AI+] Claude, author commission as maintainer upkeep, drift-fix direct commission 2026-07-19; finding from the test run, not from prior knowledge.

---

## 6. Relation to the existing rule set

Here apparatus names are dropped — only here.

### 6.1 The numbers

| Quantity | Number |
|---|---|
| Prompt files with interop/conflicts | 20 of 21 (`translation.md` is a pointer stub) |
| Interop bullets (deduplicated) | 223 |
| Conflicts bullets (raw) | 159 |
| of which genuine inter-framework conflicts (after deducting note bullets) | **~87** |
| of which consequential by the apparatus's own sequence test | **3–4** |
| of which assignable to an operation collision (state test) | **~30** |
| **without any operative correspondence** | **~55 (≈ 63%)** |
| Cross-operational collisions in this spec | ~35 |
| **of which declared somewhere in the legacy stock** | **~27 (≈ 77%)** |
| of which declared **in the C-Row** | ~10 |
| undeclared (§3.1) | 11 |
| repeatability restrictions / declared | 7 / **0** |
| state-collision class (grid-holder × suspender): instances / declared | ~27 / **2 (7%)** |

### 6.2 What holds

**"Full of inconsequential enmities" — confirmed.** ~63% of the conflict declarations have no operative correspondence. The five with the sharpest language ("cannot run simultaneously") are without exception inconsequential: all expressly permit sequential execution, and the corpus says so itself — `semiotics.md`: "The two can complement each other operationally (L3) but not ontologically (L1)."

Two cases are sharper than inconsequential:

- **anattā × Phenomenology** — declared as "genuine ontological conflict about the nature of the experiencing subject". Both perform **O8**, with identical `requires_analyst` and identical `forbids`. Zero operative difference. The same file's own interop: "independent discoveries of the same methodological move."
- **Stoicism × Existentialism** — both perform **O10**. The same cut, the opposite conclusion. One file says "cannot run simultaneously", the other "can be run in parallel if the difference in tone … is declared". A self-contradiction in the stock.

**Structuralism × Existentialism** too (the sharpest L1 anchor) does not bite as ontology: O3 → oppositions map, then O10 → cut, two usable outputs. Where it bites is exclusively **O15**, hard — and there the L1 conflict is a **declaration parameter**: the file's remedy ("declaring which level takes priority") is literally the precondition of the operation.

The `SCHEMA.md` claim "Some conflicts are L1-level (ontological, **irresolvable by sequential use**)" is nowhere redeemed in the corpus.

### 6.3 What does not hold

**"The legacy stock lacks the real collisions" — false.** ~77% of the operative collisions appear somewhere in the legacy stock. Just not in the C-Row: they appear in interop lines, D2 notes, L2 classifications, and unnumbered prose. The material knowledge is good; the registry is not.

### 6.4 The defect: three addressing errors

1. **Wrong key.** The C-Row indexes framework × framework. The real constraints are operation × analyst-state. The same collision appears, depending on chance, under C, under D2, under L2, or in the interop.
2. **Instance instead of class.** The grid-holder-×-suspender class has ~27 instances and is entered twice (Content Analysis ↔ Hermeneutics; Feminist/Postcolonial ↔ Hermeneutics-monological). Not because 25 were overlooked — the notation knows no classes.
3. **Constraint types without a cell.** Repeatability (7/0). Unary circularities (U9–U11). State preconditions without a conflict partner (O11's comparison-model-before-the-run, O14's disposition question). The C-Row is binary-relational; these are unary.

A side finding: `feminist-theory.md` **recommends** Phenomenology positively in the interop — while O22 × O8 collides hard. The legacy stock declares at this spot the opposite of the finding.

**The consequence is not to delete the declarations.** It is re-indexing: ~55 drop out as neighbourhood notes, ~27 become state rules with class reach, 11 are newly added, 7 repeatability rules need a line of their own.

---

## 7. How to operate with it

No apparatus name needed. Four steps.

### Step 1 — Translate the question into a target state

Not "which method?", but: **which state should the output carry?** The `produces` column of the table is the catalogue. Examples: a gap list (O5), a quantified test against a chance model (O11), a material status (O12), a coverage balance (O9), a retractable proposal (O14).

### Step 2 — Run backward through `requires`

Take the target operation, read `requires_material` and `requires_analyst`. Every item that the artefact does not already carry becomes a query to the interop register (§4.1): **which operation produces it?** Recursive until all items are covered or externally obtainable. The result is the forward sequence.

### Step 3 — Hold the conflict register against the sequence

For each pair in the sequence, look it up in §3. For **hard**: keep the prescribed order or split the sequence. For **soft**: write a declaration into the output as to which side governs. For the back edges (O24→O12, O22→O5) and the cycles: plan two passes, not one.

### Step 4 — Stage check

Check the sequence against §4.2. A sequence that sets a stage-0 operation *after* a stage-2 operation has either a back edge (legitimate, two passes) or an error (the precondition is already destroyed).

---

### Worked example

**Artefact:** an institutional circular (text + layout) announcing a new regulation.
**Question:** Whose perspective does the letter carry, and whom does it exclude?

**Step 1 — target state.** What is sought is a *gap list of unoccupied voice positions* → **O5**, position variant.

**Step 2 — backward.**

O5 requires: (a) a named grid of possible occurrences; (b) logged grid origin; (c) for the position variant: one's own observer stance declared as a position, not as neutrality.

- (a) voices grid → interop register: **O15 → O5** delivers "occupancy list + unoccupied positions".
  O15 in turn requires: identifiable persons, attribution utterance→person, ≥2 fillable positions, **logged attribution decision** (person vs. system), logged observer stance.
  → The attribution decision is an analyst positing, not a supply. Here: **system** (the letter assigns positions). Noted.
- (c) standpoint note → **O17 → O5**.
  O17 requires: clarified material status before interpretation begins → **O12 → O17**.
  O12 requires: determinable carrier form, provenance claim. Both present on the circular. No further lead-in.
- Additionally: the letter is multi-channel (text + layout). **O13** gives the channel ranking and opens the gate — stage 0, costs nothing.

**Forward sequence (raw version):**
`O12 → O13 → O17 → O15 → O5`

**Step 3 — conflicts.**

| Pair | Register finding | Consequence |
|---|---|---|
| O12 × O17 | **D5, hard** — status before interpretation | O12→O17 ✓ (sequence is correct) |
| O12 × O13 | no entry; both `only-before-others`, both interpretation-free | both up front, uncritical |
| O17 × O15 | interop edge (standpoint note), no conflict | ✓ |
| O17 × O5 | **W2, soft** — preassumption shiftable vs. binding brought-along list | **declaration needed:** is O15's voices grid revisable (then O17 governs) or binding (then O5 governs)? Here: binding — the positions are fixed with the letter. Write it into the output. |
| O13 × O17 | O13 version choice relevant: **U7, hard** | choose O13's **interpretation-free outside version**, not the first-person version — otherwise it collides with O12's outside position (U4) |
| O5 × O8 | **U5, hard** | O8 does not run in this sequence. No problem — but: *if* someone proposes "just look at it without prejudice first", that is O8 and must lie **before** O12 or be dropped entirely. |

**Step 4 — stages.**
O12 (0) → O13 (0) → O17 (1) → O15 (2) → O5 (3). Monotonically increasing, no back edge, no cycle. The sequence holds.

**Final sequence:**

```
1. O12  Establish material status (interpretation-free)
2. O13  Inventory channels + ranking, outside version
3. O17  Write down the preassumption, BEFORE the first interpretive step
4. O15  Assign positions — attribution decision: system (logged)
5. O5   Carry unoccupied positions as gaps
        + declaration: grid binding, O5 governs against O17 (W2)
```

No apparatus was chosen. The sequence fell out of `requires`/`produces`.

---

## 8. What this spec does not evidence

**The derivation base is prompt text, not artefact practice.** All 24 profiles are read from 21 markdown files. No operation was performed on an artefact. The profiles are reconstructions of what the files *instruct* — not of what happens when running.

**All conflicts are hypotheses.** Including the "file-declared" ones: what is declared is that a file claims a conflict, not that it occurs.

> **Status after the first material contact (2026-07-17).** The two sentences above stand unchanged — they still hold. **One** test has run (`o8-knot-2026-07-17`, K2 class O8 × O2, the case most heavily loaded in §3.1: 11/11 undeclared hard conflicts, ~27 class instances). Its result:
>
> - **The question remained untested (VOID).** The positive control fell; the pre-registered instrument clause took effect. The K2 class is thereby **neither supported nor refuted** — the status is unchanged, not improved.
> - **The procedure "conflict = state negation" has remained unchecked.** Its test case did not run to completion.
> - **What the run yielded instead:** a **profile defect** that no reading would have found (→ §5, authorship rule). The adversarial text review of this spec found six blocker prohibitions and overlooked this one, because it arises only on the material.
> - **Consequence for §6.4:** the re-indexing proposal **still stands on an untested basis**. A run that ended VOID did not support it.
>
> **The lesson for the status of this spec:** a test on material checks two things — the hypothesis **and its formulability**. If the second fails, the first is unreachable. How many of the remaining profiles clear this hurdle is **not decidable by more reading**.

> **Status after three runs (2026-07-19) — first decided result.** After two VOID runs (v1: rubric authorship-blind; v2: runner renders unmarked → §5 rule extended by the marking clause) v3 (`o8-knot-v3`) did **not** come out VOID:
> - **O8 × O2 does NOT collide.** Positive control C 3/3 (v1→v2→v3 = 0→1→3, monotone with each clause), simultaneous arm A carries both items 3/3, GATE 6/6, AC1 1.0. As soon as the O8 instruction is complete (authorship + marking), **one** agent holds both states in the same pass. The "conflict" was an artefact of the underdetermined instruction.
> - **The first tested conflict of the register does not hold** — and it was a *declared* one (§3.2 D2). This supports the catalogue's own thesis "~63% of the conflict declarations operatively inconsequential" with a first data point.
> - **Consequence for §6.4:** the re-indexing proposal gets its **first** empirical evidence — in the direction "the declarations are too generous". **But:** one pair out of 11 O8 conflicts. The K2 class as a whole remains untested; the other 10 are different partners (O22/O9/O15/O12/O5) and unchecked.
> - **The procedure "conflict = state negation"** here *predicted a conflict that does not exist*. One pair is not a refutation of the procedure, but a warning signal: the derivation from pre-/postconditions overproduces conflicts that practice does not confirm.
>
> **Evidence:** `test run o8-knot-v3 (internal test documentation)` (phase-1-4, GATE 6/6, raw/).

### The decisive test per class

| Class | Claim | Decisive test |
|---|---|---|
| **K2 (state collision)** | An analyst cannot hold both states at once | Two runs on the same artefact: once both operations in the same pass, once sequenced. Does the simultaneous output carry both defining items? If yes, the conflict is refuted. |
| **K1 (state destruction)** | B destroys what A requires | Run after B, then A. Is A's `requires` item still determinable on the artefact? |
| **Hardness hard vs. soft** | With `hard` the output becomes invalid, not just weaker | Present the simultaneous output to a third party: can they still name the operation's defining item? No → hard. Yes, but shortened → soft. |
| **Interop edge** | A.produces covers B.requires | Run B with A's output as the sole input. Does B run through without the analyst supplying more? |
| **Stage order** | The partial order is material-independent | The same chain on three artefacts of different genre. Does the order hold? |
| **Cycle O12↔O24** | Not resolvable at the operations level | Attempt a linear sequence without stage-decomposition of O12. If it succeeds, O12 was wrongly cut as a single operation. |

### Blocker findings of the adversarial review

Six prohibitions were discarded as **invented** — not file-evidenced, not compelled by the operation's wording. They are barred here as a conflict source and their consequences withdrawn:

| Field | Finding | Consequence for this spec |
|---|---|---|
| **O2.fb[4]** — writing off the remainder into "Other" without a list check | The file offers revision **or** a remainder compartment as equivalent. The only evidence was a meta-critique of the file, not the file. The reason refutes itself ("The operation remains executable"). | no conflict entry; a check-value note, not a prohibition |
| **O7.fb[2]** — a completed single-cause assignment | Not a single piece of evidence. Not compelled by the wording ("no part stands alone" does not exclude a single cause, as long as it is itself conditioned). Not determinable at the output. | no conflict entry |
| **O8.fb[4]** — a second pass of the same operation | No file says anything about repetition. The nearest passage speaks **against** it ("every situation as if for the first time"). | **`repeatable` corrected to `yes`. K3 is thereby empty** — the only K3-like case (D4: O17→O8) rests not on single-occurrence but on state destruction. |
| **O9.fb[0]**, recommendation clause | What is evidenced is "never repair" for the *checked spot*. The extension to "action recommendation as a conclusion" annuls a file-mandated step of one of the three performances. | prohibition cut back to repair of the checked spot |
| **O16.ra[5]** — no brought-along commitment on the addressee model | Inverts the evidence: the files require the advance declaration, the profile forbade it. Unfulfillable in conjunction with its own `forbids`. | reversed into a **declaration obligation** (table §5) |
| **O21.fb[3]** — simultaneous rephrasing into the new vocabulary | Contradicts the operation's wording: the translation into the observation vocabulary **is** a mandatory step of O21 and stands as its own `produces` item. | no conflict entry |

### Further hedged spots

- **O23 `no-single-use`** — unevidenced (overstretch: a counting statement about the file was read as single-occurrence of performance). Carried here as `yes (hedged)`.
- **O19 `only-before-others`** — the evidence carries only "not in the same pass", no ordering. Carried here as `yes (hedged)`.
- **O3 `systems-theory`** as performer — among 24 pieces of evidence not one line from the file; the review found there a **pre-given** pair, not one won from the material. Marked in the table as "(systems: unevidenced)".
- **O21.fb[0]** — hardness disputed: the review holds "soft" to be covered, not "hard" (the commitment does not block an outcome, only the verbal-dispute conclusion from the null finding).
- **U6 (O7 × O10)** is the sharpest undeclared case and at the same time the most uncertain: the files carry it as an individualisation *warning* (soft), although the same L1 break is declared **hard** elsewhere. The classification "hard" here is a derivation from the analyst-states, not file coverage.
- **Edge O14 → O22** — the weakest edge of the register. O22 requires an intervention *in or on the artefact*, not a produced one. Under a strict reading it drops, and cycle 2 falls apart.

### What remains structurally open

- **The cut itself.** Whether 24 is the right number is untested. O12's robustness stage overlaps in the output with O24 ("uncontrolled" stands literally in both profiles) — at least one cut is negotiable.
- **The performance attribution.** Several profiles carry traditions as performers for which not a single piece of evidence stands in the field (O3/systems, O5/semiotics + structuralism, O14/stoicism + eastern + existentialism). These are evidence gaps, not miscuts — but a third party cannot verify the performance claim at these spots.
- **O21 as sink.** That no profile requires a revision proviso as input is a gap of the stock, not a finding about O21.
