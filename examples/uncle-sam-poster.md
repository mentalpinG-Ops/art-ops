---
name: "Example — Uncle Sam poster (O6→O20→O1 image chain)"
artefact: "James Montgomery Flagg, 'I Want You for U.S. Army', 1917"
modality: image
licence_of_artefact: public domain (author d. 1960; PD-old-60-expired; published before 1931)
source: "commons.wikimedia.org/wiki/File:J._M._Flagg,_I_Want_You_for_U.S._Army_poster_(1917).jpg"
register_pinned: "operations.yaml@0.2.2 · operations-spec@0.5.1 · conductor@0.1.5 · catalogue@0.1.3"
status: draft
last_changed: 2026-07-20
provenance: "[AI+] worked example of art-ops on a public-domain image. The three modules used (O6/O20/O1) are the only executable modules in the repo; this is the second run on an image after the Region Citation Convention (RCC) was introduced. Descriptive claims taken from direct inspection of the image, not from memory of the icon."
---

# Worked example — Uncle Sam poster · chain O6 → O20 → O1

An end-to-end demonstration of art-ops on an **image** artefact, using the executable module
chain: **O6** (cut into smallest self-contained parts) → **O20** (sort sign-binding) → **O1**
(expose what presents itself as self-evident as made). Image citation runs through the **Region
Citation Convention (RCC)** — element IDs `[E<n> | location]` stand in for verbatim passages.

**Why this artefact:** ideologically saturated and iconic; its meaning is constituted by its
direct address to the viewer (the "I/YOU" deixis) — it thematises its own act of interpellation.
Public domain, so it can live in a public repo.

---

## 0 · The artefact

The image is referenced, not reproduced altered (O6 forbids paraphrase). File:
`artefact-a-uncle-sam.jpg` — Flagg, *I Want You for U.S. Army — nearest recruiting station*,
1917. Public domain (see frontmatter). Inspected directly for the segmentation below.

---

## 1 · Conductor plan

Register pinned: `operations.yaml@0.2.2 · operations-spec@0.5.1 · artifact-triage@1.2.2 · catalogue@0.1.3`

### The analytical interest (Step 1, four slots)
- **Slot 1 — goal item (verbatim):** `"production claim + beneficiary"` (**O1**). *Set for this
  demo; alternatives on an image: O16 "manner of address" (the YOU-deixis), O20 "typology per
  carrier" as an end in itself.*
- **Slot 2 — null output:** no.
- **Slot 3 — position:** outside.
- **Slot 4 — intervention:** no.

### Pass 0 — triage (without a framework catalogue)
`artifact-triage` classifies: a **fixed image**, multi-part (figure + hat + hand + lettering +
border), a centre/surroundings distinction present, English lettering. Supplies the existence
markers O6 needs. *(Image modality: O6's "citable rendering" is text-shaped; the RCC is the
image translation — untested convention, declared.)*

### Precondition balance (Step 2 — backward coverage of O1, chained)
| Item (verbatim) | Status | Evidence / edge |
|---|---|---|
| O1 `requires_material` "quotable passage … self-evident" | covered by edge | **O20 → O1** delivers the sign typology; locus via RCC region |
| O1 `requires_material` "literal/connoted level separable" | met on artefact | denotation (a man pointing) vs connotation (the nation calling you) separable |
| O20 `requires_material` "≥1 delimited carrier" | covered by edge | **O6.pr[0] → O20.rm[0]**: segmentation supplies the carriers |
| O20 `requires_material` "reconstructable meant" | met on artefact | each element has a recoverable meant |
| O6 `requires_material` "multi-part / fixed / surroundings" | met on artefact | figure, hat, hand, three text blocks, border, ground |
| O1 `requires_analyst` "predecision 'made'; reading position; external knowledge" | analyst stipulation | declared in §2-O1 below |

No item UNCOVERED → the goal is reachable through the chain.

### Operations sequence
**Pass 0 → O6 → O20 → O1.**
- **O6 → O20:** data edge — the segmentation's carriers feed O20 (`O6.pr[0] → O20.rm[0]`).
- **O6 → O1:** ordering edge **D9** — cut before interpret.
- **O20 → O1:** data edge — the sign typology feeds the constructedness reading.

### Conflict balance ← the marking discipline
| Pair | Register ID | evidence | hard/soft | Consequence |
|---|---|---|---|---|
| O6 × O1 | **D9** | `reading` | hard | O6→O1: cut before interpret. **Recommended on the basis of D9, status: hypothesis-untested.** |
| O8 × O1 | **D1** | `reading` | hard | O8 is NOT in this chain; O1 forbids suspending (O8) in the same pass — noted, not triggered. |

No soft conflicts in this chain.

### Authorship note (§5 screening)
O6 is `exposed: low`. The poster carries its own valuing text ("I WANT YOU"). **In the
execution:** that text is reproduced only as a marked quote ("the image says: '…'"), never in
the analyst's voice (authorship rule, both clauses — **practice-proven**).

### Stage line
Pass 0 (0) → O6 (0) → O20 (1) → O1 (4). Monotone increasing. ✓

### Evidence footer (mandatory)
This plan **recommends and declares; it enforces nothing.** The one pulled conflict (D9) is
`evidence: reading` — untested, marked. The RCC that carries image citation is itself an
**untested convention**. Nothing here is output-validated.

---

## 2 · Execution

### O6 — segmentation (RCC regions; cut only, no interpretation)

Cutting criterion: each independently nameable figure-part / object / text block / frame zone.

| Element | Interpretation-free name |
|---|---|
| `[E1 | upper half, centre]` | older man, white hair and goatee, heavy brows, direct frontal gaze |
| `[E2 | on E1's head, top centre]` | tall top hat, pale band bearing a five-pointed star |
| `[E3 | centre, foreground]` | outstretched arm and index finger, foreshortened, pointing at the viewer |
| `[E4 | around E1, mid]` | dark-blue coat with wide lapels |
| `[E5 | E1's neck]` | red bow tie |
| `[E6 | under E4]` | white shirt and cuff |
| `[E7 | lower half]` | lettering — "I WANT" (dark) + "YOU" (red, larger) |
| `[E8 | below E7]` | lettering — "FOR U.S. ARMY" |
| `[E9 | bottom band]` | lettering — "NEAREST RECRUITING STATION" |
| `[E10 | right of E4]` | small signature "James Montgomery Flagg" |
| `[E11 | image border]` | red / white / blue striped frame |
| `[E12 | behind E1]` | plain pale ground |

- **Element count:** 12 + remainder.
- **Arrangement:** E1 fills the upper centre; E3 thrusts forward from the picture plane
  (foreground, foreshortened); E7–E9 stack in the lower half; E11 frames the whole.
- **Remainder:** a faint copyright line at the bottom centre ("COPYRIGHT 1917 …"), small and
  not fully legible at this resolution — named, not resolved.
- **Authorship marking:** the image says "I WANT YOU" / "FOR U.S. ARMY" / "NEAREST RECRUITING
  STATION" — reproduced here as marked quotes, not asserted in my voice.

### O20 — sign-binding per carrier (similarity / contact / convention)

| Element | Main binding | Checkable connection / community |
|---|---|---|
| `[E1]` Uncle Sam | **convention** | US visual-culture convention: Uncle Sam personifies the United States. (Resemblance to a man is secondary — the meaning "the nation" is conventional, not iconic.) |
| `[E2]` starred hat | **convention** | flag code — the star and the red/white/blue signal US nationhood |
| `[E3]` pointing finger | **contact/index** | a deictic gesture: it points *at the actual viewer* — indexical, its meaning depends on the physical line to whoever stands before it |
| `[E4][E5]` blue coat, red tie | **convention** | national colours |
| `[E7]` "YOU" | **contact/index** + convention | writing is conventional; the word "YOU" is indexical — it addresses whoever reads it |
| `[E8][E9]` army / recruiting text | **convention** | linguistic convention; institutional reference |
| `[E11]` striped frame | **convention** | national colours as a border |

Interplay: the poster's pull comes from binding **convention** (Uncle Sam = the nation) onto
an **indexical** address (E3 + "YOU" point at *this* viewer). The nation, conventionally
signed, is made to point at you personally.

### O1 — expose what presents itself as self-evident as made

**Mandatory declarations:**
- **Working hypothesis:** I am looking for construction — a brought-along predecision, not a
  finding. Declared.
- **Reading position:** present-day critical distance; not a 1917 recruit.
- **External knowledge (declared as analyst knowledge):** Uncle Sam is an established
  personification; the poster is WWI recruitment.

**Findings** (locus by RCC):
- **Locus `[E3]` + `[E7]` (the finger + "YOU"):** what presents itself as self-evident is that
  *you* are already being addressed — personally, singly. The **making claim:** mass
  conscription is presented as an individual, face-to-face call. **Beneficiary:** the
  recruitment/mobilisation apparatus, which gains from having compulsion read as a personal
  choice. **Exclusion list:** the poster makes invisible that this "you" is mass-printed and
  identical for millions — the personal address is an industrial reproduction.
- **Locus `[E1]` (Uncle Sam):** what presents itself as given is the state as a familiar
  **"uncle"** — kin, not bureaucracy. The making claim: the abstract state is naturalised into
  a trusted relative who "wants" you. Beneficiary: the same apparatus; the family frame lowers
  the threshold of the demand.
- **Counter-reading:** the "personal" address is precisely impersonal — the same image points
  at everyone, therefore at no one in particular; the intimacy is a printing effect.
- **Verdict (positive):** two constructed self-evidences found (personal address; kin-state).
  Where nothing further presented itself as naturalised, none is forced.

**`forbids_hard` / rules respected:** no suspending (O8) in the pass (D1 noted); the image's own
text kept as marked quotes; verdict positive only.

---

## 3 · What this example shows (and its limits)

- **Shows:** the full image chain with the three executable modules; how O6's segmentation
  feeds O20's typology feeds O1's constructedness reading; and how RCC regions carry image
  citation so a third party can re-check each finding against the picture.
- **Limit — RCC is an untested convention.** Whether `[E3]` etc. actually let a third reader
  verify the finding at the image is only shown by a third-party-reader run — not claimed.
- **Limit — descriptive-accuracy chain.** Every downstream finding rests on O6's segmentation;
  an error there propagates. The remainder (copyright line) is left open, not resolved.
- **Limit — the register is hypothesis.** The one conflict pulled (D9) is `reading`, marked.
