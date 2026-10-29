---
title: "AI literacy for business leaders"
module: "Lesson 2"
date: 2026-10-29 12:00:00 +0000
framework: "AI Readiness and Responsible AI"
summary: "Check whether your organisation can really scale AI across six readiness dimensions, and build responsibility into the whole AI lifecycle."
tags: [readiness, data, responsible-ai, governance]
---

Running AI pilots feels like progress. This lesson is about the two things that decide whether that progress
survives contact with the rest of the organisation: **readiness** to scale, and **responsibility** in how AI
is built and run.

## Key pointers

- **Using AI is not the same as being ready to scale AI.** Activity isn't capability.
- **Pilots don't prove readiness.** A pilot can hide three problems:
  - *Data gaps:* the data turns out to be unsuitable for AI.
  - *Context dependency:* the pilot succeeds in one unit and fails in another.
  - *Hidden differences:* the underlying data, processes, governance and skills vary across the business.
- **Everyone sees readiness through their own lens.** The business points to use cases, the data team
  emphasises reporting, technology highlights infrastructure, and governance references policies. Each view
  is partial.
- **Data is the most misunderstood dimension.** Data that feeds your dashboards may not be AI-ready.
- **Responsible AI is a lifecycle practice, not a one-time review.** It's guided by a small set of widely
  accepted principles, and spotting bias needs no technical expertise.

## The framework, part 1: AI readiness

The real question is: **does the organisation have the capabilities to execute its AI strategy, consistently
and at scale?** Readiness is multidimensional. Assess all six dimensions, not just the one your own function
cares about.

**Strategy · Data · Governance · Infrastructure · Talent · Culture**

### What AI-ready data looks like

| Quality | What it means |
|---|---|
| **Reliable** | Consistent and accurate |
| **Governed** | Clear ownership |
| **Secure** | Protected and compliant |
| **Accessible** | Available to the right systems |
| **Fit for purpose** | Appropriate for the specific use case |

## The framework, part 2: Responsible AI

Responsible AI rests on four core ideas.

### 1. It's a lifecycle practice

Responsibility applies at every stage, not just a sign-off before launch.

| Stage | What responsible looks like |
|---|---|
| **Propose** | Define goals and risks |
| **Collect data** | Gather representative data |
| **Develop** | Train with governance |
| **Deploy** | Release with safeguards |
| **Monitor** | Track performance and bias |

### 2. It's guided by five core values

- **Fairness:** the system must not create unjustified disadvantages for particular groups.
- **Transparency:** people can understand how the system is built, what data it uses and how it decides.
- **Accountability:** a named team owns the outcomes.
- **Privacy** and **Security:** two values with one aim, to protect the information that powers the system, and the people affected by it.

### 3. Bias is identifiable

You don't need to be technical to ask where bias could come from. It can arise in three places:

1. **Training data**
2. **Model design**
3. **Human interpretation** of the outputs

### 4. Governance defines roles and responsibilities

Good AI governance does five things:

- Defines standards
- Reviews high-risk cases
- Assigns ownership
- Requires evidence
- Creates escalation paths

## Case study: Meridian Insurance tries to scale a pilot

*Meridian is the fictional insurer from [lesson 1]({{ '/lessons/build-your-ai-leadership-strategy/' | relative_url }}).
The numbers are illustrative.*

Meridian's claims triage pilot on **motor** claims hit its gate: cycle time fell by 3 days and reopened claims
stayed at 2.6%. The board asks to roll it out to **home** claims next quarter. Before agreeing, the COO runs
a readiness check.

**What the pilot hid.**
- *Data gap:* home claims descriptions are free-text notes from loss adjusters, while motor claims use a
  structured online form. The model was trained only on the structured data.
- *Context dependency:* motor claims are mostly similar in size. Home claims range from a broken window to a
  flooded house, so a routing mistake costs far more.
- *Hidden differences:* the home claims team uses a different system, has no data owner, and has never
  worked alongside an AI tool.

**Each function's lens.** Asked "are we ready?", the business head says yes (the use case is proven), the
data team says yes (their dashboards cover home claims), IT says yes (the platform can scale), and
governance says yes (the AI policy is signed). Each answer is true, and together they miss the problem.

**The six-dimension check** (1 = weak, 5 = strong):

| Dimension | Score | Evidence |
|---|---|---|
| Strategy | 5 | Tied to the cycle time KPI and sponsored by the COO |
| Data | 2 | Home claims data fails the AI-ready test (below) |
| Governance | 3 | Policy exists, but nobody owns home claims data |
| Infrastructure | 4 | Platform scales; needs a connector to the home claims system |
| Talent | 3 | Motor team trained; home team not yet |
| Culture | 2 | Home adjusters see triage as a threat to their judgement |

**Is the home claims data AI-ready?**

| Quality | Finding |
|---|---|
| Reliable | Partly. Claim categories are coded inconsistently between regions |
| Governed | No. There's no named owner |
| Secure | Yes. Stored in the compliant claims platform |
| Accessible | No. The triage model can't reach the home claims system yet |
| Fit for purpose | No. Free-text notes need extraction before triage can use them |

The data feeds a perfectly good weekly dashboard, and still isn't ready for AI.

**Building in responsible AI.** Meridian maps the rollout onto the lifecycle:

| Stage | What Meridian does |
|---|---|
| Propose | Names the risk: a severe claim routed to the slow queue harms a vulnerable customer |
| Collect data | Samples claims from every region and property type, not just the regions with clean data |
| Develop | Training and test results are reviewed by the AI governance group before release |
| Deploy | Every claim over £20,000 still gets a human check; adjusters can override any routing |
| Monitor | Monthly report on cycle time, override rate and outcomes by region and customer age group |

At the bias review, a claims manager with no technical background asks the three questions. *Training data:*
older customers are more likely to report by phone, so they're under-represented in the digital records.
*Model design:* postcode is an input, which can act as a proxy for income. *Human interpretation:* adjusters
may treat a "low priority" label as a judgement on the customer. All three get a mitigation before launch.

**Governance in practice:** the governance group sets the standard (the £20,000 human-check rule), reviews
the case as high-risk, assigns a home claims data owner, requires the monitoring report as evidence, and gives
adjusters an escalation path when they think the model is wrong.

**The decision:** the rollout is delayed by one quarter to fix data ownership and accessibility and to
train the home claims team. The pilot was a success; the organisation wasn't ready for it yet.

## Putting it to work

1. **Run a six-dimension readiness check.** Score strategy, data, governance, infrastructure, talent and
   culture. Get each function's view, since each sees only part of the picture.
2. **Test your data against the five qualities** for each priority use case, not in general. Data can be
   fit for one use case and not another.
3. **Before scaling a pilot, look for what it hid.** Would the data, processes, governance and skills hold
   up in the next unit?
4. **Map responsibility onto the lifecycle.** For each AI initiative, name what happens at propose,
   collect, develop, deploy and monitor, and who owns each stage.
5. **Ask the three bias questions** at every review: what's in the training data, how is the model
   designed, and how will people interpret the output?

**Watch out for:**
- Treating a successful pilot as proof the organisation is ready.
- Assuming data that's good enough for dashboards is good enough for AI.
- Running one responsible AI review at launch and never revisiting it.
- Leaving bias to the technical team when anyone can spot where it might arise.
