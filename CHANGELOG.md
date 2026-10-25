# Changelog

All notable changes to art-ops are documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/), and the
versioning follows the per-artefact scheme this family of repos adopted in May 2026: **entries
cite the artefact and its new version**, so a consumer can pin a known-good state of a single
file rather than a whole repo. Repo-level versioning is independent of artefact versions —
art-ops carries no repo version and tags no releases, so the dated sections below mark the
states the repository actually went through.

**What gets an entry.** Every version bump of a load-bearing artefact: the register
(`operations.yaml`, `catalogue.yaml`), the prose authority (`operations-spec.md`,
`catalogue.md`), the Conductor, and the operation modules. `manifest.yaml` moves with them as
the index and is cited alongside rather than carrying an entry of its own — unless the index
itself was the defect, as below.

**Bump rules.** *Patch* — wording clarification, output behaviour unchanged. *Minor* — additive
change: a new analytical move, expanded scope, a new option; backwards-compatible. *Major* —
output structure changed, an analytical move removed, or a framework reframed; consumers may
need to adapt.

## [Unreleased]

### Added

- **`examples/frame-from-a-chain.md` (0.1.0, draft)** — an application note on planning an
  operations chain and writing it into a declared frame for a stateless analysis service, with
  one sketched frame for the §7 circular. Planning only: no operation of its chain was enacted
  on an artefact, every register entry it rests on is `reading`. Indexed in `manifest.yaml`
  0.2.13 → 0.2.14 (**patch**: index entry added, no artefact version changed) and in
  `examples/README.md`.

## 2026-08-13

### Changed

- **`orchestrator/conductor.md` (0.1.8 → 0.1.10) — four repairs, each traced to a defect that
  surfaced in one real run.** Slot 1 candidates now carry the operation's `label` verbatim and a
  **negative statement**: which part of the user's question this candidate does *not* answer.
  Quoting the `produces` item made the choice auditable, but not the gloss offered alongside it
  — and the gloss is what steers the choice; in the run, O9 was glossed as "validity in the
  narrower sense" against a question asking for arguments *and* their validity, and half the
  question went unanswered. Externally supplied items now need a **proof pass** before use.
  Where the goal operation sits on the authorship screening's `high`/`medium` list, the plan
  writes out a concrete **countermeasure** and the run's stipulations must answer it — adopted,
  or rejected with a reason; an unanswered proposal is a defect of the run record. That last one
  is a maintainer decision and compels a statement about a measure, not the measure itself: the
  reading of the governance rule it rests on is recorded in the section, as is the limit that
  the screening is a candidate list and not a finding (O12 came out clean across 9 cells at the
  same rank as the confirmed O19). No process step was removed and no evidence field changed.

  *Versioning note.* These are additive analytical moves and warranted a **minor** bump to
  `0.2.0` under the rules above; they were released as two patch bumps. Recorded rather than
  rewritten — the versions are already committed, and a consumer who pinned `0.1.10` should find
  it where it was published. The series is corrected **forward** instead: the next bump of this
  file goes to `0.2.0`, not `0.1.11`.

### Fixed

- **O9 removed from the whether-question blocked list** (`orchestrator/conductor.md`, part of
  the same 0.1.8 → 0.1.10 bump). Its
  "verdict set with 'undecidable'" is `O9.requires_analyst[3]` — something the analyst brings,
  not something the operation produces; `O9.produces` carries no decision or null item. The
  error was found when a run followed the list and could not locate the item under `produces`.

- **The evidence section's own date stamp** (`manifest.yaml` 0.2.12 → 0.2.13). The section was
  headed *as of 2026-07-26*, although the 2026-08-10 upkeep changed eight of its lines — and the
  stamp matched no commit that ever touched the file. Corrected to 2026-08-10, read off the
  commit history rather than assumed. It was corrected and not removed because it carries what
  the header cannot: when the evidence was last re-examined, as against when the file was last
  edited.

- **The version record the repairs were missing** (`manifest.yaml` 0.2.10 → 0.2.11).
  `manifest.yaml` still carried the Conductor at `0.1.9` after the file had moved to `0.1.10`,
  and the `provenance` header carried no entry for either version. Both numbers looked plausible
  on their own, which is why nothing surfaced the drift. `0.1.9` therefore exists as a version
  number but never as a commit.

## 2026-08-10

### Changed

- **Register upkeep across the conflict register** — `operations-spec.md` (0.5.2 → 0.5.5),
  `operations.yaml` (0.2.2 → 0.2.5), `orchestrator/conductor.md` (0.1.7 → 0.1.8),
  `manifest.yaml` (0.2.7 → 0.2.10). Drift fixes and register-internal defects found while
  working through the register entry by entry. Four entries were recorded as **under-specified
  transcription rather than repaired** — explicitly not as evidence of overproduction, because
  supplying an anchor would mean inventing a derivation that may never have been made. No
  conflict was decided and no evidence field changed.

## 2026-07-20

### Added

- **Initial public release** — `operations-spec.md` (0.5.2), `operations.yaml` (0.2.2),
  `catalogue.md` (0.1.4), `catalogue.yaml` (0.1.3), `orchestrator/conductor.md` (0.1.7),
  `manifest.yaml` (0.2.7). The 24-operation register with its prose authority, the Conductor in
  plan mode, the OPC modules of the first image analysis with the Region Citation Convention,
  worked examples across three modalities (text / image / dialogue), and the GitHub Pages
  showcase. Relicensed to CC BY-SA 4.0 on the same day, matching the source collection the
  register was distilled from.

---

Licence: CC BY-SA 4.0 — see [`LICENSE`](LICENSE).
