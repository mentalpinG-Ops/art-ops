---
name: O6-image-segmentation
op_id: O6
variant: image            # image instance of O6 — the actually triggered module (image plan 2026-07-19)
version: 0.1.1
status: draft
last_changed: 2026-07-19
repeatable: yes
stage: 0
exposed: low              # screening §5; informs, does not gate
pins: {operations-spec: "0.5.1", operations-register: "0.2.1", opc: "OPC-README.md @ 0.1.1"}
requires_material:
  - {id: "O6.rm[0]", text: "multi-part (several distinguishable elements)", checkable_on: artefact}
  - {id: "O6.rm[1]", text: "fixed rendering; quotability via RCC instead of a verbatim passage", checkable_on: artefact, gap_note: "spec item is text-shaped; RCC is the image translation, untested"}
  - {id: "O6.rm[2]", text: "surroundings present (centre/surroundings distinguishable)", checkable_on: artefact}
requires_analyst:
  - {id: "O6.ra[0]", text: "declared cutting unit + reach of surroundings + reference size (fixed before cutting, declared in the output as the cutting criterion)", checkable_on: output}
  - {id: "O6.ra[1]", text: "state-lean (no interpretive/expectational load carried while cutting)", checkable_on: output}
produces:
  - {id: "O6.pr[0]", text: "segmentation: numbered elements with RCC region references", checkable_on: output}
  - {id: "O6.pr[1]", text: "cutting criterion (declared: what the cut followed)", checkable_on: output}
  - {id: "O6.pr[2]", text: "countable total (element count)", checkable_on: output}
  - {id: "O6.pr[3]", text: "order/arrangement of the elements", checkable_on: output}
  - {id: "O6.pr[4]", text: "remainder (what escapes the segmentation, named)", checkable_on: output}
forbids:
  - {id: "O6.fb[0]", text: "paraphrasing the material (the image is referenced, never reproduced altered)", checkable_on: output}
  - {id: "O6.fb[1]", text: "concluding within the same pass (D9: cut before interpreting)", checkable_on: output, evidence: reading}
  - {id: "O6.fb[2]", text: "simultaneous boundary contestation (do not contest one's own cutting boundaries within the same pass)", checkable_on: output}
declarations_from_plan: []   # image plan 2026-07-19: no soft conflicts in the sequence
evidence: "Profile: reading. D9 ordering (O6 before O1): reading/hypothesis. RCC: untested convention."
provenance: "[AI+] from operations.yaml@0.2.1 O6 profile, image variant via RCC; author brief step 3; [AI+] full EN translation per author decision 2026-07-19."
---

# O6 (image) — cut into smallest self-contained parts

**What this module does:** decompose an image into its smallest self-contained elements and
make each referenceable via the Region Citation Convention (RCC, see `OPC-README.md`).
**Cut only — do not interpret** (D9: interpretation is a later, separate pass).

## Prompt (executable; input: one image)

> You are given an image. Decompose it into its smallest self-contained elements — persons,
> objects, parts of the surroundings and visible arrangement relations. **Describe only what
> is visible; do not interpret, do not explain, do not evaluate** — interpretation is
> explicitly not your task.
>
> Output:
> 1. **Element list:** one line per element, `[E<n> | <location>] <interpretation-free name>`.
>    `<location>` is a nameable image region: a grid reference ("upper third, left"), a
>    relational reference ("between E2 and E4") or an object anchor ("on the bench, centre").
>    The location says **where** — never what it means.
> 2. **Cutting criterion:** one sentence — what your cut followed (e.g. "each independently
>    nameable person/object/surroundings zone plus visible relations").
> 3. **Total:** the element count.
> 4. **Arrangement:** how the elements lie relative to each other (foreground/background,
>    left/right, overlaps) — purely spatial.
> 5. **Remainder:** what escapes the segmentation (blurs, occlusions, not safely nameable) —
>    **name it rather than guess**. Uncertain items are marked as uncertain
>    ("[E7 | lower right] object, not safely identifiable"), never resolved.
>
> Authorship marking (generic): if the image itself contains text/writing carrying valuations,
> reproduce them only marked ("the image says: '…'"), never in your own voice.

## Limits

- **Descriptive accuracy:** the element list is the input truth of all subsequent operations —
  errors here propagate. Keep uncertainties open (remainder field), do not smooth them.
- The RCC is an untested convention; whether a third party can actually check findings against
  the image via `[E<n>]` is only shown by a third-party-reader run.
