# art-ops

**A toolkit for the analysis of cultural artefacts** — texts, images, documents, practices.
Instead of routing questions through theory schools ("what would school X say?"), art-ops
decomposes analysis into **operations**: single, nameable moves performed on the material,
which can be combined — and whose reliability is declared item by item.

---

## The idea in three sentences

1. Analytical traditions contradict each other in their **justifications** — but many of their
   **moves** are identical or combinable. art-ops works at the level of the move.
2. Every operation is described as a profile: what it needs from the **material**, what it
   demands of the **analyst**, what it **produces**, what it **forbids**. From these profiles,
   analysis sequences can be planned mechanically — including the conflicts between operations.
3. **Honesty is a construction principle:** the register consistently distinguishes which
   statements are empirically tested and which are (still) reading-derived hypotheses — and
   every generated analysis plan declares this line by line.

## What's inside

| File | Content |
|---|---|
| [`catalogue.md`](catalogue.md) / [`catalogue.yaml`](catalogue.yaml) | **Inventory:** 24 operations, distilled from 21 analysis prompts of a curated collection — which traditions perform which move, where they overlap, how checkable their core claims are |
| [`operations-spec.md`](operations-spec.md) / [`operations.yaml`](operations.yaml) | **Mechanism:** the 24 operation profiles, the conflict register (which operations exclude each other within the same pass) and the interop graph (which feed into each other) |
| [`orchestrator/conductor.md`](orchestrator/conductor.md) | **Planner:** takes an artefact + an analytical interest and produces an ordered, conflict-checked operations plan — with an evidence status attached to every recommendation. It plans; it does not execute. |
| [`operations/`](operations/) | **Modules:** executable single prompts per operation (so far the three of one real image analysis), plus a Region Citation Convention for images |
| [`manifest.yaml`](manifest.yaml) | **Machine-readable index:** artefacts, versions, derivation relations, evidence state |

**How to read:** the prose files are authoritative (they carry justifications and caveats);
the YAML files are the machine-readable derivation. Where they disagree, the prose governs.

## What it can do

- Translate an analysis question into an **ordered sequence of moves** instead of a theory
  label ("first segment, then sort sign-bindings, then expose naturalisations" — rather than
  "do a semiotic analysis").
- **Make conflicts visible** before they spoil the analysis: which moves demand mutually
  exclusive stances from the analyst, which orderings are forced.
- **Analyse images**, although the underlying prompts are text-shaped — via a Region Citation
  Convention that translates "quote the passage" for image regions.
- Declare every recommendation with its **evidence status**: empirically supported · refuted ·
  reading-derived hypothesis.

## What it cannot do (yet) — the limits, laid open

- **The register is mostly hypothesis.** The profiles and conflicts are derived from the
  wording of the source prompts, not tested against material. Only a few statements are
  empirically tested so far — among them the most remarkable finding: **the first conflict of
  the register ever put to a test did not hold** (two operations that, per derivation, ought to
  collide demonstrably run within the same pass — the "conflict" was an artefact of an
  underdetermined instruction). Consequence: the tool **recommends and declares; it enforces
  nothing**.
- **The planner does not execute.** A run mode is deliberately deferred until the register is
  more broadly validated — nothing should harden untested hypotheses into a hard gate.
- **Interpretive operations remain interpretation.** Operations like the naturalisation
  exposure have no hard falsifier; their outputs are justified readings with a mandatory
  counter-reading, not measurements. The tool makes this visible instead of hiding it.
- **Modality gaps:** sound, moving image, numerical data and code are not covered by the
  inventory; image analysis rests on the (itself still untested) region convention.

## Origin and method

The register is a **reading distillate**: from 21 analysis-prompt files of a curated
collection, the operations were extracted "de-named" — as verb + object, without theory brand
names (those appear only where they are themselves the object of analysis). No prompt text was
copied; this is a re-description at the level of the move, not a fork.

The empirical findings come from pre-registered test runs with blinded judging instances and
constructed gold standards; the test identifiers are attached to the respective findings. The
full test documentation is not part of this repo.

## Status & licence

Under development (`draft`); API and register content may change.
**Licence:** proprietary, all rights reserved — reading and scrutiny welcome, reuse by
arrangement (commercial licensing by arrangement), see [`LICENSE`](LICENSE).

No employer, client, or person-related materials: analyses of real private artefacts
(e.g. photographs) remain outside this repo as a rule; a `.gitignore` net prevents accidental
inclusion.
