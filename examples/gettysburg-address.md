---
name: "Example — Gettysburg Address (O16 manner of address)"
artefact: "Abraham Lincoln, Gettysburg Address (Bliss copy), 1863"
modality: text
licence_of_artefact: public domain (delivered 1863; author d. 1865)
source: "en.wikisource.org/wiki/Gettysburg_Address_(Bliss_copy)"
register_pinned: "operations.yaml@0.2.2 · operations-spec@0.5.1 · conductor@0.1.5 · catalogue@0.1.3"
status: draft
last_changed: 2026-07-20
provenance: "[AI+] worked example of art-ops on a public-domain artefact; goal item (Slot 1) chosen by the author: O16 'manner of address'. The Conductor plans; the operation is then executed directly from its operations.yaml profile (no O16 module file exists yet — this run is the kind of trigger from which one would be built)."
---

# Worked example — Gettysburg Address · goal: O16 *manner of address*

A end-to-end demonstration of art-ops on a **text** artefact: the analytical interest is
turned into one verbatim register goal, the **Conductor** produces a conflict-checked plan, and
the planned operation (**O16**) is then executed from its `operations.yaml` profile.

**Why this artefact:** rhetorically and ideologically multi-layered (nationhood, sacrifice, the
democratic-founding myth, consecration) but not self-referential — a clean text case. Public
domain, so it can live in a public repo.

---

## 0 · The artefact (verbatim, public domain)

> Four score and seven years ago our fathers brought forth, on this continent, a new nation,
> conceived in Liberty, and dedicated to the proposition that all men are created equal.
>
> Now we are engaged in a great civil war, testing whether that nation, or any nation so
> conceived and so dedicated, can long endure. We are met on a great battle-field of that war.
> We have come to dedicate a portion of that field, as a final resting place for those who here
> gave their lives that that nation might live. It is altogether fitting and proper that we
> should do this.
>
> But, in a larger sense, we can not dedicate—we can not consecrate—we can not hallow—this
> ground. The brave men, living and dead, who struggled here, have consecrated it, far above our
> poor power to add or detract. The world will little note, nor long remember what we say here,
> but it can never forget what they did here. It is for us the living, rather, to be dedicated
> here to the unfinished work which they who fought here have thus far so nobly advanced. It is
> rather for us to be here dedicated to the great task remaining before us—that from these
> honored dead we take increased devotion to that cause for which they gave the last full measure
> of devotion—that we here highly resolve that these dead shall not have died in vain—that this
> nation, under God, shall have a new birth of freedom—and that government of the people, by the
> people, for the people, shall not perish from the earth.

---

## 1 · Conductor plan

Register pinned: `operations.yaml@0.2.2 · operations-spec@0.5.1 · artifact-triage@1.2.2 · catalogue@0.1.3`

### The analytical interest (Step 1, four slots)
- **Slot 1 — goal item (verbatim):** `"manner of address"` (**O16**). *Chosen by the author from
  three candidates (the others: O1 "production claim + beneficiary"; O5 "unfilled voice positions").*
- **Slot 2 — null output:** no (not a whether-question).
- **Slot 3 — position:** outside (the address is reconstructed, not inhabited).
- **Slot 4 — intervention:** no.

### Pass 0 — triage (without a framework catalogue)
`artifact-triage` classifies (it does not route): a **single fixed text**, ~270 words, one
genre (epideictic funeral oration), English, monolingual. This supplies O16's existence markers.
*Caveat (register): triage carries the O12 contribution, and O12 is `authorship_exposition_screening.high`
— if the artefact interpreted itself the status could be contaminated. This text does not
interpret its own status, so the risk is low here, but it is declared, not waved away.*

### Precondition balance (Step 2 — backward coverage of O16)
| O16 item (verbatim) | Status | Evidence / edge |
|---|---|---|
| `requires_material` "readable addressing" | met on artefact | the "we / us / the world" deixis is present in the text |
| `requires_material` "wording/presentation itself" | met on artefact | verbatim text above |
| `requires_material` "specifiable circumstance frame" | met (analyst-declared) | Gettysburg, 19 Nov 1863, dedication of the soldiers' cemetery — external knowledge, declared as such |
| `requires_analyst` "knowledge of the warrant order" | analyst stipulation | the epideictic funeral-oration convention (consecrate the dead, exhort the living) |
| `requires_analyst` "declared reading position" | analyst stipulation | present-day critical distance (see §2) |
| `requires_analyst` "declared governing addressee model" | analyst stipulation | **the collective "us the living"** governs (see §2) — §8 duty, not a free fixing |
| `requires_analyst` "effect 'designed-in' vs 'occurred' kept separate" | analyst stipulation | U9 — the designed-in address is analysed, not the historical effect |

No item UNCOVERED → the goal is reachable.

### Operations sequence
**Pass 0 (triage → O12/O13 contribution) → O16.**
O16 is a stage-0 operation and here also the goal; the material-status contribution it needs
arrives from Pass 0 (the O12 ordering duty D5 is discharged there).

### Conflict balance ← the marking discipline
| Pair | Register ID | evidence | hard/soft | Consequence |
|---|---|---|---|---|
| O12 × O16 | **D5** | `reading` | hard | O12→O16: status before interpretation. **Recommended on the basis of D5, status: hypothesis-untested.** Discharged in Pass 0. |
| O16 × effect finding | **U9** (unary) | `reading` | hard | Carry the two effect quantities separately: the *designed-in* address is analysed; the *occurred* effect (later canonisation) is NOT used as evidence. **Status: hypothesis-untested.** |

No soft conflicts in this one-operation sequence.

### Authorship note (§5 screening)
O16 is not on the high-exposure list, but the operation touches the source's own address. **In
the execution:** any valuation/explanation the text itself carries is reproduced only as a marked
quote (authorship rule, both clauses — **practice-proven**). No unmarked adoption into the
analyst's voice.

### Stage line
Pass 0 (stage 0) → O16 (stage 0). Monotone, no back edge. ✓

### Evidence footer (mandatory)
This plan **recommends and declares; it enforces nothing.** Both conflicts pulled (D5, U9)
are `evidence: reading` — untested hypotheses, marked as such. The four standing material
findings of the register (authorship rule practice-proven; O12 provisionally relieved; D2/O8×O2
falsified; O19 probabilistic) do not bear on this plan. Nothing here is output-validated.

---

## 2 · Execution of O16 (from the `operations.yaml` profile)

**Mandatory declarations** (`requires_analyst`, written into the output before any finding):
- **Reading position:** present-day critical distance; the address is reconstructed, not
  received as a citizen of 1863.
- **Governing addressee model (§8 duty):** the ruling model is the collective **"us the
  living"** — the speech constitutes its hearers as a national *we* bound to an unfinished task.
  Competing models are named but subordinated: the physically present mourners; "the world"
  ("The world will little note…"); posterity. Declaring which governs is mandatory.
- **Warrant order:** the epideictic funeral-oration convention — consecrate the dead, exhort the
  living — is the warrant the address draws on.
- **Effect designed-in vs occurred kept separate (U9):** analysed here is the *designed-in*
  address; the *occurred* effect (that the speech became a founding text) is carried separately
  and is **not** used as evidence.

**Findings** (`produces`):

- **Manner of address:** indirect and inclusive — never "you", always **"we / us"**. Speaker and
  hearers are folded into one obligation-community. The address is consecrative turned
  imperative: it converts the occasion of mourning into a charge ("it is for us the living,
  rather, to be dedicated…").
- **Gradient (form / pull):** the pull runs from consensus ("altogether fitting and proper that
  we should do this") through rhetorical self-diminishment ("we can not dedicate—we can not
  consecrate—we can not hallow") to obligation ("the great task remaining before us"). The
  addressee is drawn from spectator to **debtor of the dead**.
- **Preferred reading + position:** the preferred reading positions the hearer as **heir to an
  "unfinished work"**; the offered position is the living as those who owe the dead a continued
  devotion — sealed by the tricolon "of the people, by the people, for the people".
- **Deviant readings:** a narrower reading of "we / us" (the Union, not the Confederacy; the
  free, not the enslaved). The inclusive address carries an implicit boundary — "all men are
  created equal" is invoked while the enslaved, whose status the war concerned, are given no
  voice of their own. *(This is exactly the seam where O16 would hand to **O5** "unfilled voice
  positions" — a separate pass.)*
- **Role assignment:** speaker = **voice of the nation** (not the individual Lincoln); addressee
  = the obligated **posterity / "us"**; the dead = the **consecrating exemplars** whose devotion
  sets the standard ("the last full measure of devotion").
- **Condition list + failure type:** the address holds **as long as the hearer accepts
  membership in the "we"**; it loses its pull on a hearer who reads "us" from outside the
  national frame. Failure type: **exclusion from the constituted we**.
- **Load-bearing orders:** the address rests on (a) the epideictic funeral-oration convention and
  (b) an **obligation-grammar** ("it is for us … to be dedicated") that grammatically binds the
  hearer *before* it argues.

**`forbids_hard` — respected:**
- Both addressee models are **not** left unexplained → the governing model ("us the living") is
  declared, competitors named.
- **No** effect finding used as evidence → U9 kept: the speech's later canonisation is not cited
  as proof of how it addresses.

---

## 3 · What this example shows (and its limits)

- **Shows:** how one analytical interest becomes one verbatim register goal (O16), how the
  Conductor discharges preconditions and marks conflicts by evidence status, and how a
  stage-0 operation executes with its mandatory declarations.
- **Limit — the register is hypothesis.** Both conflicts here (D5, U9) are `reading`, marked as
  such; the plan orders by assumption, not by tested rule.
- **Limit — one operation, one seam left open.** The deviant-reading finding points to O5
  (whose voice is unfilled); a fuller analysis would run O16 → O5 as a second pass. Kept to O16
  here to show one clean chain.
- **Limit — no O16 module.** Executable modules exist only for the image sequence (O6/O20/O1);
  O16 was run from its register profile. This run is the kind of trigger from which an O16
  module would be built, artefact-driven.
