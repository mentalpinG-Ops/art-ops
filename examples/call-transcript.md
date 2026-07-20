---
name: "Example — call transcript (O13 channels + O16 manner of address)"
artefact: "Synthetic call-centre transcript — IVR-bot → live-agent booking"
modality: transcript (dialogue)
licence_of_artefact: "CC0 1.0 (dedicated to the public domain by the rights-holder)"
source: "Written for art-ops; a synthetic, sanitised benchmark dialogue (see provenance). Not a real call; no real persons."
register_pinned: "operations.yaml@0.2.2 · operations-spec@0.5.1 · conductor@0.1.5 · catalogue@0.1.3"
status: draft
last_changed: 2026-07-20
provenance: "[AI+] worked example of art-ops on a dialogue artefact. The transcript is a synthetic role-play scenario the rights-holder dedicates to the public domain under CC0. Sanitised for public release: real-brand tokens replaced with fictional equivalents, and the example e-mail set to the RFC-2606 reserved domain (@example.com). All names, brands and contact details are fictional; any resemblance to real persons or entities is coincidental."
---

# Worked example — call transcript · O13 (channels) + O16 (manner of address)

An end-to-end demonstration of art-ops on a **dialogue** artefact. Two operations are run — but,
unlike the image example, **not as a chain**: the register carries no interop edge O13→O16, so
these are **two complementary stage-0 passes** on the same material, each declared in its own
right.

**Why this artefact:** a single call with two live channels (an IVR bot that fails, a human
agent that repairs) plus a written follow-up — real turn-taking, a motivated channel switch, and
a sharp contrast of address between bot and agent. Synthetic and CC0, so it can live in a public
repo.

---

## 0 · The artefact (verbatim, CC0 — synthetic, all details fictional)

> `[0:02] BOT:` Hello and welcome to Redwood Health bookings. I'm Ava, your virtual assistant. I can help you book an appointment from a referral. To begin, please say your full name.
> `[0:12] CUSTOMER:` Uh, hi. It's Tomasz Wiśniewski.
> `[0:18] BOT:` I'm sorry, I didn't catch that. Please say your full name clearly after the tone.
> `[0:26] CUSTOMER:` Tomasz. Wiś-niew-ski.
> `[0:33] BOT:` Thank you, Thomas. Now, please say your date of birth in the format day, month, year.
> `[0:43] CUSTOMER:` The fourteenth of March, nineteen seventy-one.
> `[0:49] BOT:` I'm sorry, I didn't understand. Please enter your date of birth using your keypad: two digits for the day, two for the month, four for the year.
> `[1:00] CUSTOMER:` Oh, for— fine. Hold on.
> `[1:09] BOT:` Thank you. Now, please say or enter your referral number.
> `[1:14] CUSTOMER:` Look, can I just talk to a person? This is doing my head in.
> `[1:20] BOT:` I can help you book your appointment. Please say or enter your referral number.
> `[1:27] CUSTOMER:` No. Agent. Customer service. A human being. Please.
> `[1:33] BOT:` Okay. I'll transfer you to an advisor now. Please hold.
> `[2:18] AGENT:` Hello, good afternoon, you're through to bookings, my name is Rahul. Thank you so much for holding. How may I help you today, sir?
> `[2:27] CUSTOMER:` Oh — oh thank god, a real person. Hello. Sorry. Yes. I've got a referral I just want to book, and your robot and I really weren't getting on.
> `[2:37] AGENT:` Not a problem at all, sir, I completely understand. May I have your good name, please?
> `[2:43] CUSTOMER:` Tomasz Wiśniewski.
> `[2:48] AGENT:` Thank you, Mr Wiśniewski. And you are having a referral — for which procedure, kindly?
> `[2:55] CUSTOMER:` A colonoscopy. I've got the letter here, there's a referral number on it if you need it.
> `[3:04] AGENT:` Most kind. Yes, please read it to me... thank you. One moment... yes, I have located it. So we will get this booked for you. First, kindly tell me — which area are you in, and do you have a preferred medical facility?
> `[3:20] CUSTOMER:` I'm in town. I don't really have a preference, just somewhere close. Whatever's nearest.
> `[3:27] AGENT:` Of course. So I am seeing a few options near you. There is one on Brindley Road, one on Calder Street, and one on Featherstone Way. Which of these is most convenient for you?
> `[3:42] CUSTOMER:` I... honestly, none of those mean anything to me. I've no idea where any of those are.
> `[3:49] AGENT:` No problem at all, sir, take your time. They are all within a few miles, if that helps.
> `[3:57] CUSTOMER:` It doesn't, really — I don't drive, so "a few miles" could be anywhere.
> `[4:05] AGENT:` I understand, I understand. Kindly bear with me one moment—
> `[4:11] CUSTOMER:` —Hang on, actually. Is there one near the old library? The big red-brick building by the bus station, on the high street. People go there for blood tests.
> `[4:23] AGENT:` The old library... let me just check this for you. One moment, I am searching the maps now.
> `[5:06] CUSTOMER:` ...Are you finding it? It's quite well known round here.
> `[5:12] AGENT:` Yes, yes, I am just looking — a few results are coming up. Is it Stephenson Street? There is a clinic on Stephenson Street.
> `[5:21] CUSTOMER:` I don't know the street name, do I. It's just — by the bus station. The big red-brick one.
> `[5:29] AGENT:` Bear with me, sir, the map is loading... Ah. I think I have it. Is it near a bakery and a betting shop?
> `[5:39] CUSTOMER:` ...Yes. Yes, that's the one. That's it exactly.
> `[5:44] AGENT:` Wonderful. So that facility is on Stephenson Street, and they do have colonoscopy slots. The earliest is two weeks on Thursday. Shall I book that for you?
> `[5:55] CUSTOMER:` Yes. Please. That one.
> `[5:59] AGENT:` Booked. You are confirmed, Mr Wiśniewski.
> `[6:05] AGENT:` Now, very important, sir — for the colonoscopy there is the preparation you must follow. Three days before, you move to a low-fibre diet, no seeds, no nuts, no skins. The day before, you take the bowel preparation — there are two sachets, the first at midday and the second in the evening, each mixed with one litre of water, and after that clear fluids only, nothing red or purple, and no solid food from—
> `[6:31] CUSTOMER:` —Sorry, sorry. Wait. Hang on.
> `[6:34] AGENT:` Yes, sir?
> `[6:36] CUSTOMER:` Is there any chance you could just email me all that? I'm not going to remember half of it. The diet, the sachets, the timings — I'll get it wrong.
> `[6:46] AGENT:` Of course, of course, that is no problem at all. We will do one thing: I will send the full preparation instructions to your email, so you have everything in writing. May I confirm your email address?
> `[6:57] CUSTOMER:` It's t.wisniewski@example.com.
> `[7:03] AGENT:` Thank you. I am sending it across to you now. You will have it all in writing, so there is nothing you need to remember from the call.
> `[7:12] CUSTOMER:` That's brilliant, thank you. And sorry — I was a bit short earlier. The robot just got me wound up. You've been really helpful.
> `[7:20] AGENT:` Not at all, sir. I am very happy we got there in the end. We sorted it out together, no?
> `[7:26] CUSTOMER:` We did, yeah. We got there. Thanks, Rahul.
> `[7:30] AGENT:` Most welcome, Mr Wiśniewski. Take care, and all the best for the appointment. Goodbye.
> `[7:35] CUSTOMER:` Cheers. Bye.

---

## 1 · Conductor plan

Register pinned: `operations.yaml@0.2.2 · operations-spec@0.5.1 · artifact-triage@1.2.2 · catalogue@0.1.3`

### The analytical interest (Step 1, four slots)
- **Slot 1 — goal item (verbatim):** `"manner of address"` (**O16**) — same operation as the
  Gettysburg example, on a different modality. *Complementary pass: O13 `"switch finding
  single-/multi-channel"` — run alongside, not chained (see below).*
- **Slot 2 — null output:** no.
- **Slot 3 — position:** outside (interpretation-free), fixed for **both** operations (O13
  requires EITHER outside OR first-person — U7).
- **Slot 4 — intervention:** no.

### Pass 0 — triage (without a framework catalogue)
`artifact-triage` classifies: a **fixed transcript**, multi-party (bot / customer / agent),
timestamped, English. It is *presented as ONE* call (O13 precondition) with a centre (the
spoken exchange) and surround (hold music, transfer, the e-mail follow-up).

### Two complementary passes — NOT a chain
The register carries **no interop edge O13→O16** (O13's only documented out-edge is O13→O18).
So this is not a pipeline. O13 and O16 are **both stage-0**, run independently on the same
artefact; neither supplies a precondition of the other. Declaring this honestly is the point —
an analysis is not always a chain.

### Precondition balance (Step 2)
| Op | Item (verbatim) | Status | Evidence |
|---|---|---|---|
| O16 | "readable addressing" | met on artefact | bot and agent both address the caller explicitly |
| O16 | "wording/presentation itself" | met on artefact | verbatim transcript above |
| O16 | "declared governing addressee model" | analyst stipulation | the caller-as-addressee, read per channel (see §2) |
| O13 | "artefact in original version / presented as ONE" | met on artefact | one continuous call |
| O13 | "EITHER outside OR first-person" | analyst stipulation | **outside, interpretation-free** chosen (U7) |

No item UNCOVERED for either operation.

### Conflict balance ← the marking discipline
| Pair | Register ID | evidence | hard/soft | Consequence |
|---|---|---|---|---|
| O12 × O16 | **D5** | `reading` | hard | O12→O16: status before interpretation (discharged in Pass 0). **hypothesis-untested.** |
| O16 × effect finding | **U9** (unary) | `reading` | hard | designed-in address analysed; the *occurred* effect (caller's frustration/relief) carried separately. **hypothesis-untested.** |
| O13 × O13 | **U7** | `reading` | hard | choose ONE ranking version (outside); do not add a first-person ranking to it. **hypothesis-untested.** |

No soft conflicts.

### Authorship note (§5 screening)
Neither operation is on the high-exposure list, but both touch the speakers' own words. **In the
execution:** the speakers' valuations ("your robot and I really weren't getting on"; "we sorted
it out together") are reproduced only as marked quotes (authorship rule, both clauses —
**practice-proven**).

### Stage line
Pass 0 (0) → O13 (0) ∥ O16 (0). Both stage 0, parallel — no ordering claim between them. ✓

### Evidence footer (mandatory)
This plan **recommends and declares; it enforces nothing.** All three conflicts (D5, U9, U7)
are `evidence: reading` — untested, marked. Nothing here is output-validated.

---

## 2 · Execution

### O13 — inventory the channels; state their ranking (outside, interpretation-free)

**Channel list (incl. absent ones):**
1. **Automated voice (IVR bot "Ava")** — scripted speech recognition; the opening channel.
2. **Keypad / DTMF** — offered by the bot ("enter … using your keypad") as a fallback the caller never adopts.
3. **Live human voice (agent "Rahul")** — real-time, adaptive; the repairing channel.
4. **Written follow-up (e-mail)** — the persistence channel the agent adds at the end.
- *Absent / declined:* the keypad channel is offered but refused; no visual/self-service channel is present.

**Ranking (outside version):** structurally, the bot channel is **imposed first** (the system
front-loads it) but is **functionally lowest** — it fails on its own terms. The **live-agent
channel is functionally dominant** (it completes the task). The **e-mail channel** ranks as the
**persistence layer** (repeatable, not memory-bound: "so there is nothing you need to remember
from the call").

**Switch finding (single-/multi-channel):** **multi-channel** — one call, three spoken/keyed
modes plus a written coda. The switch bot→agent is **motivated**, not incidental: it is triggered
by the caller's explicit escalation after the bot ignores it twice.

**Foreground / surrounding cut:** foreground = the spoken exchange; surround = the system
infrastructure (the "please hold", the transfer gap `[1:33]→[2:18]`, the silent map search).

*`forbids_hard` respected:* no running interpretation (channels named, not yet read for
meaning); one ranking only (U7).

### O16 — reconstruct the manner of address (per channel)

**Mandatory declarations:** reading position — present-day, outside. Governing addressee model —
**the caller as the addressee**, read separately in each channel. designed-in vs occurred kept
separate (U9): the *designed* address is analysed, not the caller's felt reaction.

**Findings (`produces`):**
- **Manner of address — bot channel:** **directive and system-centred**. The bot addresses the
  caller as an *input source*: "please say your full name", "enter … using your keypad", "I can
  help you book" (its capability, not the caller's need). It mis-hears the name and asserts a
  wrong one back ("Thank you, **Thomas**") — the address does not track the addressee.
- **Manner of address — agent channel:** **deferential and person-centred**. "May I have your
  **good name**, please?", "**Mr Wiśniewski**", "Not a problem at all, sir", "We sorted it out
  together, **no**?" The agent addresses the caller as a *person in a situation*, and repairs the
  name the bot got wrong.
- **Gradient (form/pull):** the bot's pull is **conditional** — cooperation is offered only if
  the caller supplies input in the required format; on format-failure the address loops
  ("Please say or enter your referral number" — repeated verbatim). The agent's pull is
  **accommodating** — it bends to the caller's frame ("the old library", "near a bakery").
- **Preferred reading + position / role assignment:** bot → caller as *defective input*; agent →
  caller as *co-participant* ("we sorted it out together"). The channel switch is itself an
  **address switch** — from "you are a mis-formatted input" to "you are a gentleman in need".
- **Condition list + failure type:** the bot's address **fails** exactly where the caller falls
  outside its input schema (a spoken date, an unrecognised name, an escalation request) —
  failure type: **schema-exclusion**. The agent's address holds by abandoning the schema.
- **Load-bearing orders:** the bot rests on a **transactional script** (fixed slots, fixed
  order); the agent rests on a **service-courtesy convention** (deference, repair, shared
  resolution).

*`forbids_hard` respected:* both addressee-model readings are declared (per channel), not left
unexplained; no effect finding used as evidence (U9) — the caller's relief is not cited as proof
of the agent's address.

---

## 3 · What this example shows (and its limits)

- **Shows:** a dialogue artefact read by two operations that are **complementary, not chained** —
  O13 ranks the channels and finds the motivated switch; O16 reads the address in each channel
  and finds the switch is an address-switch. The two findings meet at the same seam (the
  bot→agent handover) without any register edge forcing them together.
- **The teaching point:** not every operation set is a pipeline. Uncle Sam was a real chain
  (O6→O20→O1, documented edges); this is two independent stage-0 passes. Register-honesty means
  showing that, not inventing an edge.
- **Limit — the register is hypothesis.** All three conflicts (D5, U9, U7) are `reading`, marked.
- **Limit — synthetic artefact.** This is a written role-play, not a recorded call; findings
  about *this* transcript do not generalise to real call data (which, for boundary reasons, is
  out of scope for this public repo).
