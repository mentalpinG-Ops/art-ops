---
name: O20-sign-binding
op_id: O20
variant: generic          # carries on images without translation (image plan §3: preconditions image-coverable)
version: 0.1.1
status: draft
last_changed: 2026-07-19
repeatable: yes
stage: 1
exposed: no
pins: {operations-spec: "0.5.1", operations-register: "0.2.2", opc: "OPC-README.md @ 0.1.1"}
requires_material:
  - {id: "O20.rm[0]", text: "≥1 delimited carrier", checkable_on: artefact, edge: "O6.pr[0] — segmentation supplies the carriers"}
  - {id: "O20.rm[1]", text: "reconstructable meant (what is meant)", checkable_on: artefact}
  - {id: "O20.rm[2]", text: "per case a checkable connection or community", checkable_on: output}
requires_analyst:
  - {id: "O20.ra[0]", text: "knowledge of the governing convention (for convention cases)", checkable_on: output}
  - {id: "O20.ra[1]", text: "declared arity of the framework", checkable_on: output}
  - {id: "O20.ra[2]", text: "no binding verdict fixed in advance", checkable_on: output, author: analyst}
produces:
  - {id: "O20.pr[0]", text: "typology per carrier (similarity / contact / convention)", checkable_on: output}
  - {id: "O20.pr[1]", text: "interplay for composite material", checkable_on: output}
  - {id: "O20.pr[2]", text: "named community per convention case", checkable_on: output}
forbids:
  - {id: "O20.fb[0]", text: "a two-place model without explaining which governs (arity must be declared — counterpart to O20.ra[1])", checkable_on: output}
declarations_from_plan: []
evidence: "Profile: reading. Solo operation (sole carrier of sign-binding sorting in the inventory)."
provenance: "[AI+] from operations.yaml@0.2.1 O20 profile; author brief step 3; [AI+] full EN translation per author decision 2026-07-19."
---

# O20 — sort sign-binding by similarity / contact / convention

**What this module does:** for each carrier, sort **by what** it means — the denotation level
as a hands-on move. Input is a segmentation (O6 output, referenced via RCC).

## Prompt (executable; input: image + O6 element list)

> You are given an image and a numbered element list (`[E<n> | location]`). For **each
> element**, sort by what it means — exactly one main binding, mixed cases named as such:
>
> - **Similarity:** the element means because it resembles what is meant (a depiction shows
>   what it shows).
> - **Contact/cause:** it means via a physical, causal or situational connection (a trace, a
>   place, a condition pointing to what brought it about).
> - **Convention:** it means by the convention of a nameable community (dress codes, gestures,
>   writing, emblems).
>
> Rules:
> 1. **Declare the checkable connection per case** — for contact: which connection; for
>    convention: **which community** carries it ("convention — which community?" is a
>    mandatory field; "generally customary" is not enough).
> 2. **No binding verdict fixed in advance:** decide at the element, not from a brought-along
>    expectation of what is "typically" a symbol.
> 3. **Declare arity:** say at the start whether you work two-place (carrier→meant) or
>    three-place (carrier→meant→for whom), and stay with it.
> 4. Reference exclusively via `[E<n>]` — do not introduce new, unreferenced elements. If an
>    element is missing, name the gap instead of filling it.
> 5. Authorship marking (generic): if the artefact itself carries text/writing/emblems with
>    valuations or explanations, reproduce them only marked ("the image says: '…'"), never in
>    your own voice — including when naming the community of a convention case.
>
> Output: table `[E<n>] | binding | checkable connection / community`, then a short paragraph
> on the **interplay** (which bindings dominate, where several attach to one element).

## Limits

- O20 is the denotation level: it says **by what** something means — not **what** it connotes
  or naturalises (that is O1, a separate pass).
