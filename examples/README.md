# Examples — art-ops on real artefacts

Three worked examples of the art-ops workflow across three modalities. Each shows the same
end-to-end shape: **one analytical interest → one verbatim register goal → a Conductor plan
(operations, conflicts marked by evidence status, stages) → the operation(s) executed → limits
laid open.**

| File | Modality | Artefact | Operation(s) | Artefact licence |
|---|---|---|---|---|
| [`gettysburg-address.md`](gettysburg-address.md) | text | Lincoln, Gettysburg Address (1863) | **O16** manner of address | public domain |
| [`uncle-sam-poster.md`](uncle-sam-poster.md) | image | Flagg, "I Want You" poster (1917) | **O6 → O20 → O1** (chain) | public domain |
| [`call-transcript.md`](call-transcript.md) | dialogue | synthetic IVR-bot → agent booking call | **O13 + O16** (complementary passes) | CC0 (synthetic) |

## What the set is meant to show

- **The operation, not the tradition, is the unit.** The same operation **O16** ("manner of
  address") is run on a speech *and* on a call transcript — the tool asks "which move do you lay
  on the material", not "which theory school applies". De-naming in practice.
- **Not every operation set is a pipeline.** Uncle Sam is a real **chain** (O6→O20→O1, with
  documented data/ordering edges in the register). The transcript is **two complementary
  stage-0 passes** (O13, O16) with *no* edge between them — shown honestly rather than forced
  into a chain.
- **Evidence honesty is carried through.** Every conflict a plan pulls (D5, U9, U7, D9 …) is
  cited with its `evidence` status — here all `reading`, i.e. untested hypotheses, marked as
  such. The plans **recommend and declare; they enforce nothing.**
- **Image citation is a declared convention.** The image example cites regions via the Region
  Citation Convention (RCC, `[E<n> | location]`) — an untested convention, declared as such.

## Provenance & boundaries

- Gettysburg and Uncle Sam are **public-domain** artefacts (verified source pages; see each file's
  frontmatter). The Gettysburg text and the poster are the canonical test artefacts A/B of the
  source collection.
- The call transcript is **synthetic** and dedicated **CC0** by the rights-holder — written for
  this repo, sanitised for public release (fictional names/brands, RFC-2606 example e-mail). It
  is **not** a recording of a real call; findings about it do not generalise to real call data,
  which is out of scope for this public repo.

See [`../README.md`](../README.md) for the tool, and [`../orchestrator/conductor.md`](../orchestrator/conductor.md)
for the planner these examples exercise.
