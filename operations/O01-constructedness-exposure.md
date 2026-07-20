---
name: O1-constructedness-exposure
op_id: O1
variant: generic-with-image-note   # locus on images = RCC region instead of a verbatim passage (image plan §3 gap translation)
version: 0.1.1
status: draft
last_changed: 2026-07-19
repeatable: yes
stage: 4
exposed: no
pins: {operations-spec: "0.5.1", operations-register: "0.2.2", opc: "OPC-README.md @ 0.1.1"}
requires_material:
  - {id: "O1.rm[0]", text: "quotable passage without justification — on images: an RCC region that presents itself as self-evident/given", checkable_on: artefact, gap_note: "spec item is text-shaped; RCC translation untested"}
  - {id: "O1.rm[1]", text: "literal/connoted level separable", checkable_on: artefact}
requires_analyst:
  - {id: "O1.ra[0]", text: "predecision 'made' brought to the material (declared working hypothesis, not a finding)", checkable_on: output, author: analyst}
  - {id: "O1.ra[1]", text: "declared own position", checkable_on: output, author: analyst}
  - {id: "O1.ra[2]", text: "external knowledge (cultural/historical context, declared as such)", checkable_on: output}
produces:
  - {id: "O1.pr[0]", text: "located passage(s) (RCC reference)", checkable_on: output}
  - {id: "O1.pr[1]", text: "making claim + beneficiary", checkable_on: output}
  - {id: "O1.pr[2]", text: "exclusion list (what the naturalised reading renders invisible)", checkable_on: output}
  - {id: "O1.pr[3]", text: "counter-reading", checkable_on: output}
  - {id: "O1.pr[4]", text: "verdict only where positive (where nothing naturalised is found: say so, do not force it)", checkable_on: output}
forbids:
  - {id: "O1.fb[0]", text: "suspending (O8) — D1: declared hard conflict, O8→O1 as ordering", checkable_on: output, evidence: reading}
  - {id: "O1.fb[1]", text: "positionlessness (counterpart to O1.ra[1]: one's own position must be declared)", checkable_on: output}
  - {id: "O1.fb[2]", text: "use as a checking instance (the operation judges constructively, it does not verify — not a verdict instrument)", checkable_on: output}
declarations_from_plan: []
evidence: "Profile: reading. No hard falsifier of the core operation — inference from operations-spec §5/§8 (produces item 'verdict only where positive' + the apparatus entries performing O1 spread across classes B and C in catalogue.yaml; a direct 'O1 = class C' entry does NOT exist — classes there are apparatus-, not operation-scoped). Hence the verdict-only-where-positive duty as the honesty valve. D9 (O6 before O1): reading."
provenance: "[AI+] from operations.yaml@0.2.1 O1 profile; author brief step 3 (image sequence); [AI+] full EN translation per author decision 2026-07-19."
---

# O1 — expose what presents itself as self-evident as made

**What this module does:** expose the meanings that present themselves as natural/given as
culturally made — the myth level as a hands-on move. Runs **after** O6 (D9: cut before
interpreting) and typically after O20; a separate pass.

## Prompt (executable; input: image + O6 element list + optionally O20 typology)

> You are given an image, an element list (`[E<n> | location]`) and possibly a sign typology.
> Your task is the second level of meaning: **what presents itself here as self-evident,
> natural or given — and is in truth made?**
>
> Declare at the start (mandatory, one sentence each):
> 1. **Working hypothesis:** you are looking for making — that is a brought-along predecision,
>    not a finding. Say so.
> 2. **Your reading position:** from where you read (cultural location, distance to the milieu
>    of the image).
> 3. **External knowledge:** which cultural/historical context knowledge you draw on — marked
>    as analyst knowledge, not as an image finding.
>
> Then, per finding:
> - **Locus:** `[E<n>]` or element combination (RCC) — where does the meaning that presents
>   itself as self-evident sit?
> - **Making claim:** what is presented as given that is a cultural/social setting — and **who
>   benefits** from the naturalisation (beneficiary, named concretely or honestly "not
>   determinable")?
> - **Exclusion list:** what does this reading render invisible (what would one have to see if
>   one did not share it)?
> - **Counter-reading:** at least one reading that does not go along with the naturalisation.
>
> Rules: **verdict only where positive** — where you find nothing naturalised, say so
> explicitly; do not force a finding (the operation has no hard falsifier; your non-finding is
> the only honesty valve). Authorship marking: if the image itself carries valuing
> writing/symbols, reproduce them only marked. No statements about real depicted persons as
> individuals — the object is the **construction of meaning**, not biography.

## Limits

- A constructive operation without a hard falsifier (class C) — the output is a justified
  reading, not a checkable measurement. Hence the mandatory declarations + verdict only where
  positive.
- On images, the locus rests on the RCC (untested convention) and the O6 element list
  (descriptive-accuracy chain).
