---
title: "Build the AI transformation roadmap"
module: "Lesson 4"
framework: "The Absorption and Momentum Tests"
summary: "Turn a ranked list of AI initiatives into a phased roadmap by asking what the organisation can actually absorb, and sequencing for momentum, not speed."
tags: [strategy, roadmap, change]
---

This lesson continues [Prioritise AI pilots]({{ '/lessons/prioritise-ai-pilots/' | relative_url }}). By now you
have a ranked list. The board doesn't approve a ranked list, though. It approves a **phased roadmap**.

**Ranked list → phased roadmap → executive approval**

The ranking told you *what* is worth doing. The roadmap decides *when*, and that depends less on what's
technically ready than on what the organisation can actually take on.

## Key pointers

- **A roadmap is not a project plan.** An AI transformation roadmap is a phased, milestone-driven plan that
  takes AI investments from assessment through production and scale, tied to specific business outcomes. It
  treats strategy, data readiness, governance and organisational design as *interdependent workstreams*, not
  a task list.
- **Absorption is usually the binding constraint.** Once value and AI fit are established, what decides
  what goes in a phase is the organisation's capacity to adopt it, not the technology.
- **People work goes first, not last.** Training, process redesign and ownership take longer than building
  the model, so they have to start early.
- **Sequence for momentum, not speed.** Visible early wins create the confidence and executive commitment
  that later, larger bets need. Each funded phase should earn the capital for the next.
- **The sequence has to be defensible.** A sceptical stakeholder should be able to challenge its logic on
  the merits, and the logic should hold.

## The framework: The Absorption and Momentum Tests

### Four habits of good sequencing

| Habit | What you do |
|---|---|
| 1. **Map dependencies** | Identify the data, governance and process dependencies behind each initiative. |
| 2. **Assess absorption capacity** | Ask what the organisation can actually absorb in a given phase, not just what's technically ready. |
| 3. **Place people work early** | Schedule people and process work first, not as a final "change management" step. |
| 4. **Build a defensible sequence** | Produce an order whose logic a sceptic can challenge on its merits. |

### The absorption test: Phase One or Phase Two?

Ask of every initiative: **can this organisation absorb this initiative in this phase?** Check four
conditions:

| Condition | The question |
|---|---|
| **Data pipeline** | Is the information the initiative needs already connected and usable? |
| **Governance** | Is someone authorised to approve it, monitor it and take responsibility for it? |
| **Team capacity** | Do the people who'd run and manage it have the time and training to do so? |
| **Integration dependency** | Is there a connection to an existing system or workflow that has to be built or confirmed first? |

Give each condition a quick read:

- 🟢 **Green:** ready.
- 🟡 **Yellow:** a gap, but a manageable one.
- 🔴 **Red:** not ready. A blocking dependency.

An initiative that clears the bar goes in **Phase One**, the work started now. One that doesn't goes in
**Phase Two**, held back until the missing foundation is built. And the red conditions don't just delay the
initiative: they become Phase One *foundation work* in their own right.

### The momentum test: the tiebreaker

When a placement is unclear, ask: **if this succeeds in Phase One, does it create enough confidence and
evidence to fund Phase Two?** If yes, it belongs in Phase One. If it still needs Phase Two groundwork first,
it waits.

## Case study: Meridian Insurance builds its roadmap

*Meridian is the fictional insurer used throughout this playbook. The numbers are illustrative.*

At the end of [lesson 3]({{ '/lessons/prioritise-ai-pilots/' | relative_url }}), Meridian's COO had a ranked
list. Now the COO has to turn it into an 18-month roadmap the board will approve. The obvious plan is to start
the most valuable work first: fraud flagging and claims triage. The absorption test tells a different story.

**Step 1: Map dependencies.** For each initiative, the team lists what it relies on:

| Initiative | Depends on |
|---|---|
| Agent call summaries | Call recordings in the contact centre platform; agent training |
| Policy wording search | Policy library (already digital); staff access rules |
| Home claims triage | A home claims data owner; a connector to the home claims system; trained adjusters |
| Subrogation recovery | Claims history; the recoveries team's time |
| Fraud flagging | Consolidated fraud data from three systems; the claims data pipeline built for triage |

**Step 2: Run the absorption test.**

| Initiative | Data pipeline | Governance | Team capacity | Integration | Placement |
|---|---|---|---|---|---|
| Agent call summaries | 🟢 | 🟢 | 🟡 Peak season in Q1 | 🟢 | **Phase One** |
| Policy wording search | 🟢 | 🟢 | 🟢 | 🟢 | **Phase One** |
| Home claims triage | 🔴 Not connected | 🟡 Owner newly named | 🟡 Adjusters untrained | 🔴 Connector needed | **Phase Two** |
| Subrogation recovery | 🟡 | 🟢 | 🟡 | 🟡 | Unclear → momentum test |
| Fraud flagging | 🔴 Three systems | 🟡 | 🟡 | 🔴 Needs triage pipeline | **Phase Two, later** |

Triage, the initiative everyone wanted first, has two reds. Starting it now would mean building on a missing
foundation. It moves to Phase Two, and its reds become Phase One work.

**Step 3: Apply the momentum test to subrogation.** No reds, but four yellows. Would a win here fund Phase
Two? Recovered money goes straight to the P&L, so the CFO would notice. But the recoveries team sits inside
claims, and claims is also preparing for triage. The team can't absorb both at once, and triage is worth
more. Subrogation waits for Phase Two. The binding constraint isn't technology, it's the claims team's
capacity.

Policy wording search is the opposite case. It's lower value, but it's all green, visible to every staff
member, and done in six weeks. It stays in Phase One as a time-boxed quick win because it builds momentum.

**Step 4: Place people work early.** Meridian's first draft put adjuster training in month 10, just before
triage launched. The final roadmap moves it to month 2. Training, revised claims workflows and the new data
owner's role start in Phase One, so the people are ready before the technology is.

**The roadmap**, as four interdependent workstreams:

| Workstream | Phase One (months 1–6): prove and prepare | Phase Two (months 7–12): scale the core | Phase Three (months 13–18): expand |
|---|---|---|---|
| **Initiatives** | Call summaries live; policy search (6-week trial) | Home claims triage live; subrogation pilot | Fraud flagging pilot |
| **Data** | Build home claims connector; start consolidating fraud data | Claims data pipeline in production | Fraud data consolidated |
| **Governance** | Home claims data owner named; triage risk review | Monitoring report for triage (cycle time, overrides, fairness) | Fraud model review and escalation paths |
| **People & org** | Adjuster training; redesign claims intake workflow | Recoveries team capacity freed up; triage champions in each region | Fraud investigators trained to work with model flags |
| **Milestone to unlock the next phase** | Call handling time down ≥1 min; connector tested | Home cycle time down ≥3 days with accuracy held | Fraud detection rate up ≥10 pts |

**Step 5: Defend the sequence.** At the board meeting the CFO pushes back: "Fraud is the most valuable item.
Why is it last?" The COO's answer holds up: fraud flagging depends on the claims data pipeline that triage
builds, and on data from three systems that isn't consolidated yet. Starting it now would mean paying for that
foundation twice. Meanwhile call summaries will show savings within six months, which is the evidence the
board needs to fund Phase Two.

**The outcome:** the board approves Phase One in full and Phase Two in principle, with funding released when
Phase One's milestone is met. The roadmap sequences for momentum, not speed, and every phase earns the next.

## Putting it to work

1. **Start from your ranked list** and write down the dependencies behind each initiative: data,
   governance, process and systems.
2. **Run the absorption test** with the people who'd actually run each initiative, not only the sponsors.
   Rate each condition green, yellow or red.
3. **Turn every red into Phase One foundation work** with an owner and a date.
4. **Use the momentum test** for anything that's unclear. Put quick, visible wins early.
5. **Schedule people work first.** Training, workflow changes and new roles should start before the
   technology arrives.
6. **Lay the roadmap out as workstreams** (initiatives, data, governance, people) with a milestone that
   unlocks each phase.
7. **Rehearse the sceptic's questions.** For each placement, can you say in one sentence why it's there?

**Watch out for:**
- Sequencing by value or technical readiness alone, and ignoring absorption.
- Treating change management as the last step.
- Overloading one team by putting several initiatives that depend on it in the same phase.
- Funding all phases up front, so there's no milestone that earns the next.
- A roadmap that's really a task list, with no link between workstreams.
