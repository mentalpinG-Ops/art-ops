# CLAUDE.md — art-ops

Context for AI assistants working in this repository.

## Purpose

A register of **analytical operations** for cultural artefacts + a planning tool derived from
it, which — per artefact — selects the operations that support the user's analytical interest.
The working level is the **operation** (a hands-on move on the material), not the
**apparatus** (the named tradition that justifies it). Details: [`README.md`](README.md).

## Ground rules for changes

1. **Prose is authoritative.** `operations-spec.md` and `catalogue.md` carry justifications,
   caveats and evidence states; the YAML files are derived from them. Where they disagree, the
   prose governs. YAML is re-derived from prose, never the other way round — a YAML edit
   without prose coverage is drift.
2. **Evidence honesty is a construction principle.** The register consistently distinguishes
   empirically tested statements from reading-derived hypotheses. No edit may present a
   hypothesis as validated; every recommendation of the planner carries its evidence status.
   The tool recommends and declares; it enforces nothing.
3. **Versioning:** every load-bearing file carries `version`/`status`/`last_changed` in its
   header; substantive changes bump the version and record the origin of the change.
4. **Provenance discipline:** this repo is produced largely AI-assisted. AI-introduced content
   is marked as such (the `[AI]` marker family), not silently counted as prior knowledge;
   findings from test runs are cited as such, not as prior knowledge.

## Material boundaries (non-negotiable)

- **No** employer, client, or institutional material — in any form.
- **No person-related artefacts or analyses of them** in this repo: runs on real private
  artefacts (e.g. photographs) stay outside; the `.gitignore` net (`plans/`) protects against
  accidental inclusion. Check before every commit.
- No naming of employers, institutions, or private individuals in files, commits, issues.
- When in doubt: **do not write it** — clarify first.

## Licence

Proprietary, all rights reserved, commercial licensing by arrangement — see
[`LICENSE`](LICENSE). The referenced prompt schema of the source collection lives separately
under its own licence and is referenced by field name only, never embedded. Content from
share-alike-licensed sources does not migrate here by copy (licence incompatibility);
adoptions are declared re-writes with a provenance note.

## Current state

- [`catalogue.md`](catalogue.md) — functional catalogue: 24 operations, distilled de-named.
- [`operations-spec.md`](operations-spec.md) — profiles, conflict register, interop graph.
- [`orchestrator/conductor.md`](orchestrator/conductor.md) — planner (plan mode; run mode
  deliberately deferred until the register is more broadly validated).
- [`operations/`](operations/) — executable modules (so far those of the first real image
  analysis) + Region Citation Convention.

**Both core documents are `draft` and rest mostly on reading, not on practice** — their §8
say so themselves. The evidence state (what is tested, what is hypothesis) is consolidated in
[`manifest.yaml`](manifest.yaml) and must be updated there **and** in the affected files in
sync whenever new test findings arrive — operating files of the same repo must not contradict
each other.
