---
name: OPC-contract-stub
version: 0.1.3
status: draft
last_changed: 2026-07-20
pins:
  operations-spec: "operations-spec.md @ 0.5.1"
  operations-register: "operations.yaml @ 0.2.2"
provenance: "[AI+] Author brief 'build step 3, working toward the target output'. LEAN cut of a broader modules draft down to the actually triggered sequence of one image analysis (O6→O20→O1); verdict repairs incorporated, see below; [AI+] full EN translation per author decision 2026-07-19; [AI+] RCC rule 1 sharpened (object-anchor preference) from a blinded single-reader pilot 2026-07-20 — a pilot, not a test; status stays untested; [AI+] rcc-mr-2026-07-20 finding entered per pre-registered NO-branch consequence."
---

# OPC — Operations Profile Contract (stub, LEAN version)

Modules are **executable single prompts** per operation, in `operations/`. Each carries its
spec profile machine-readably in the frontmatter (items with stable IDs) and a prompt body.
**Composition comes from a Conductor plan**, never from the module itself — conflict/interop
registers are not copied into modules and are not mechanically derived here either.

## Why this cut (repairs from the adversarial review of the original modules draft)

| Draft defect (verdict/critic) | Treatment here |
|---|---|
| K1 matcher deviated from spec §2 | **no matcher/composer built** — the Conductor plan supplies the checked sequence; modules execute, they do not compose |
| Soft register (W1–W4) with no place of production in the frontmatter | field `declarations_from_plan` — the plan passes mandatory declaration lines in; the module writes them into the output |
| Pilot conflated a format test with an authorship test | runs are **application, not testing** (applying ≠ testing); a test needs its own pre-registration under the test regime |
| Mandatory coupling to a not-yet-adopted schema field of the source collection | **dropped** — de-named operations carry no tradition on which that field would hang; to be revisited if the schema introduces it |
| `states.yaml` without a consumer (YAGNI) | **dropped** — states as plain text in the frontmatter; a states vocabulary only once a composer reads it |
| `checkable_on` only on `produces` | **every item** carries `checkable_on: artefact|output` |
| Authorship marking only for "exposed" operations; O8 (the documented case) would fall out | the authorship-marking convention applies **generically** to every module whose operation can touch source utterances; the `exposed` field informs, it does not gate |

## Frontmatter fields (per module)

`name · op_id · variant · version · status · last_changed · repeatable · stage · exposed ·
pins (spec/register) · requires_material[] · requires_analyst[] · produces[] · forbids[] ·
declarations_from_plan (empty if the plan passes nothing in) · evidence (status of the
load-bearing register statements: practice-proven | reading | falsified)`

Each item: `{id, text, checkable_on}` — IDs stable (`O6.rm[0]` form); for `requires_analyst`
additionally `author: analyst` where applicable (two-clause rule, practice-proven).

## Authorship-marking convention (practice-proven, o8-knot v1–v3)

Valuations/explanations/interpretations that **the source itself** carries may be reproduced —
**but only marked** ("the source says: '…'"). Unmarked adoption into one's own voice counts as
analyst-authored and violates "no X" conditions. Applies in every module output.

## Region Citation Convention (RCC) — for image artefacts

**The occasion for this stub:** the spec items "quotable rendering" (O6) and "quotable
passage" (O1) are text-shaped; an image satisfies them only via a region convention. It reads:

1. **Element ID + region reference:** every segmented element receives `[E<n> | <location>]`,
   where `<location>` is a nameable image region — a grid reference (e.g. "upper third,
   left"), a relational reference ("between E2 and E4") or an object anchor ("on the table,
   centre"). **When the target is an object, prefer the object anchor** (name the object
   type): in a busy surround, a grid or relational reference alone can leave several
   candidates in the region.
2. **Quotation = element reference:** where a text operation demands "quote the passage",
   `[E<n>]` takes the place of the verbatim quote. The finding thereby remains checkable by
   third parties against the image — that is the purpose of quoting, not the text form.
3. **No interpretation in the region reference:** the location says where — never what it
   means.

**Status: convention, untested — now with a first pre-registered finding
(`rcc-mr-2026-07-20`, single artefact).** A blinded three-reader run with a constructed
gold key and a judge GATE (all judges 4/4, unanimity, AC1 1.0) split the convention's claim
in two:
- **What held (18/18, incl. rejection of all constructed false claims):** *claim checking*
  over full RCC references (location + carrier naming) — the purpose of citing.
- **What did not hold (14/24 resolved):** *location-alone resolution*. Errors cluster in
  three known limit classes: **(1) zone grids over multi-element zones** (readers name the
  stack, not the element), **(2) lexical collision** of the location wording with features
  of other elements (a "band" location resolving to a striped border — once *confidently
  wrong*, the most dangerous form), **(3) small elements with imprecise fine-position.**
  Object anchors resolved best (0.833), grids worst (0.333) — supporting the anchor
  preference in rule 1.
The status stays **untested** overall (the pre-registered H1 threshold was missed; n=1
artefact): cite with location + carrier naming, do not rely on location alone.

## Limits

- Executing modules ≠ Conductor run mode. The orchestrator stays in plan mode; here the
  **user** (or a session started by the user) executes individual modules along a plan.
- Three modules exist (O6 image, O20, O1) — those of the actually triggered image-analysis
  sequence. Further ones only on real demand — a module comes into being when a concrete
  analysis plan calls for it, not on stock.
- The register remains mostly hypothesis; every module carries the evidence status of its
  load-bearing statements in the frontmatter.
