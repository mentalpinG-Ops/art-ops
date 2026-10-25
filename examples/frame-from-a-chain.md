---
name: "Application note — planning a declared frame from an operations chain"
modality: text (institutional circular), planning only
register_pinned: "operations.yaml@0.2.5 · operations-spec@0.5.5"
version: 0.1.0
status: draft
last_changed: 2026-10-25
provenance: "[AI+] application note, drafted by Claude (Sonnet 5.5) on the maintainer's commission, 2026-10-25; no sub-agent was used for the drafting, token total not recorded. Planning example only: the chain as a whole was not enacted on an artefact (of its operations only O12 has met material in a register test), and no service consumed the sketched frame. The sketch is a generic illustration, not the format of any particular service."
---

# Application note — planning a declared frame from an operations chain

The other examples run operations on an artefact. This note does the step before: an operator
who wants a **stateless analysis service** (one that keeps no state between calls) to apply a chain of operations plans the chain
first, then writes the result into a **frame declaration**: a versioned description of the lens,
the objects, the licensed operations, the observer position and the confidence discipline that
the service resolves per request. Nothing here is enforced by art-ops (the tool recommends and
declares), and a response of the kind sketched below carries no sign that the chain was
followed.

Terms used below: **pass** is one run of one analyst over the material (here: one service
call, by stipulation). **K1** is a conflict that ordering resolves; **K2** is a pair of analyst
states that one analyst cannot hold in the same pass. **W-class** conflicts are soft: both
operations stay valid, one side must be declared as governing. (K1, K2: spec §2; W-class:
spec §3.3.) **`reading`** is the register's evidence status for an entry derived from reading
the prompts and not tested on an artefact.

## Why planning instead of a mechanism

The register's conflicts are stated over analyst states: *can the same analyst hold both
states in one pass?* A stateless service keeps no state between calls, so a mechanism that
tracks analyst states across calls would be a new feature of the service. The operator can
instead do the work before the frame is pinned, and write the outcome into slots a frame
declaration of the sketched kind already has. This is the cheapest option. Run on real
artefacts it would also yield the material evidence the register lacks (spec §8); planning
alone yields none.

## The steps

The four steps of `operations-spec.md` §7, plus a fifth for provenance:

1. **Target state.** What should the output carry? Pick the operation whose `produces` names it.
2. **Backward through `requires`.** Each `requires` item the artefact does not carry becomes a
   query to the interop register (the register's supply edges between operations, spec §4.1).
   The result is the forward sequence.
3. **Conflict register against the sequence**, pair by pair. Hard conflicts keep the prescribed
   order or split the sequence; soft ones need a declaration of which side governs.
4. **Stage check** against §4.2.
5. **Provenance.** Name the register version in the frame. A register change that changes a
   decision is a new frame version, never an edit of a pinned one.

## Where each decision is written

| Decision from the plan | Slot in a frame declaration |
|---|---|
| Sequence of operations | the description of the licensed operations, in order |
| Hard conflict resolved by ordering (K1) | the same sequence |
| Hard conflict resolved only by separate passes (K2) | two frames, one per pass; "a pass is one call" is a stipulation, not a fact. The one K2 pair tested so far (O8 × O2) came out as no conflict, so the class rests on reading |
| Hard conflict with no resolution | a declared self-conflict; a service that treats it as blocking will refuse the frame, which is the true state |
| Soft conflict (W-class) | a declaration in the operations description naming which side governs |
| Evidence status of each register entry used | lines in the operations description: `basis: <id> · status: <status> · source: <spec@version §>` |
| Observer position the operations require | the observer slot |
| Hedge conditions (a status that stays unresolved) | the confidence slot |
| Operations whose material the service does not take | scope exclusions |

## Worked sketch — the §7 circular

**Artefact:** an institutional circular announcing a regulation, reduced to its text (the
circular of the spec's worked example also carries layout).
**Question:** whose perspective does the letter carry, and whom does it exclude?
**Chain** (spec §7, worked example): the spec's sequence is `O12 → O13 → O17 → O15 → O5`. Here
it runs as `O12 → O17 → O15 → O5`: O13 (channels) is dropped, because the service takes text,
so the layout channel is not given and not ranked. The operations are O12 (fix the material's
status before interpreting), O17 (log one's own preassumption), O15 (assign a position or
role), O5 (register absence as a finding). Conflicts held against the sequence:
D5 (O12 before O17, hard; the order is the resolution), W2 (O17 × O5, soft; declared below),
the authorship rule for prohibitions of the form "no X" (spec §5).

```yaml
# Illustration only. Not the format of any particular service; not validated against any schema.
frame: position-gap-circular
version: v1
register: operations-spec@0.5.5

declaration:
  lens: >-
    Voice-position gap analysis of an institutional text, planned as the chain
    O12 -> O17 -> O15 -> O5.
  objects: >-
    The utterances of the text, the persons or agents it names or addresses, and the voice
    positions those utterances open or leave unfilled.
  operations: >-
    (1) Fixes the status of the text before interpreting it; no interpretation in this step.
    (2) States the reader's preassumption in one sentence before any interpretive step.
    (3) Assigns the positions the text opens; attribution decision: system, reported as an
    output line. (4) Lists unfilled positions as gaps over the grid of step 3; empty categories
    are reported, not deleted.
    Declarations. Grid governance: the grid is binding for step 4 and is not revised by the
    preassumption (W2, soft). Intent: the issuer's stated purpose is rendered only as the
    text's own statement, marked "the text states"; the reading introduces no intent of its
    own (authorship rule, applied here to the prohibition on meaning from intent that the
    register lists under O12). Channels: text only; no claim about layout.
    Status. basis: D5 · status: reading, untested · source: operations-spec@0.5.5 §3.2.
    basis: W2 · status: reading, untested · source: operations-spec@0.5.5 §3.3.
    basis: authorship rule · status: practice-proven on operation O8 (a source that states
    its own evaluations; three runs of one test, the first two ended VOID on their positive
    control and the third passed its gate, the rule's two clauses stem from the first two),
    declared generic for all operations; its use on intent is not itself tested · source:
    operations-spec@0.5.5 §5 and operations.yaml (authorship_rule). The sequence as a whole
    has not been enacted on an artefact; of its operations only O12 has met material in a
    register test (authorship screening, 2026-07-18/19) · source: manifest.yaml and
    operations.yaml (evidence_global), as read 2026-10-25.
  observer: >-
    A reader outside the issuing institution, classifying the text from outside and stating
    that standpoint as a position, not as neutrality.
  confidence: >-
    An empty cell on the text's own grid is a finding, not an uncertainty. A position the
    reader adds beyond the grid is named as an addition, not listed as a gap. If issuer or
    date cannot be determined, the status stays unresolved and the reading carries a hedge.

scope:
  admits: "A single institutional text with an identifiable issuer, text only."
  excludes:
    - "layout, typography, imagery (no non-text channel is given)"
    - "what the issuer privately meant beyond what the text states"

self_conflicts: []
```

## What a frame declaration cannot carry here

Found while writing the sketch; each is a limit of a *declarative slot*, not of the register.

- **Sequence and status are prose.** In the sketched format nothing checks that the described
  order is the planned one, or that the status lines match the register.
- **Prohibitions of the form "no X".** The register requires that such a prohibition name its
  author and that a rendering of the source be marked. A lexical pattern list cannot tell the
  analyst's own statement from a marked quotation, so the sketch declares no patterns. The
  prohibition stands in the description only, unchecked.
- **Non-text operations.** O13 (channel inventory) has nothing to work on when the service
  takes text only, and the image module for O6 (`operations/O06-image-segmentation.md`) is
  unusable there. O6 itself is modality-neutral in the register (cut into smallest
  self-contained parts) and can be planned on text.
- **Hard conflicts across passes** are expressible only as separate frames; nothing links them.

## Status

Every register entry the sketch rests on is `reading`, except the authorship rule, which is
practice-proven on O8; the chain as a whole has not been enacted on an artefact, and of its
operations only O12 has met material in a register test. The sketch shows that the plan fits
a declarative frame, not that the reading it produces is sound. Enforcing any part of it
(refusing a request, compiling a frame from the register) would need a passed material test per operationalisation first; until then the
practice stays declarative.
