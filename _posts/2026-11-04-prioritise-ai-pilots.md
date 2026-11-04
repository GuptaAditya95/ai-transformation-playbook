---
title: "Prioritise AI pilots: from a dozen to three"
module: "Lesson 3"
framework: "The Value–Feasibility–Risk Sort"
summary: "Score every pilot on value, feasibility and risk, avoid the clustering trap, and turn a ranked list into a portfolio you can defend."
tags: [strategy, prioritisation, portfolio]
---

This lesson continues [Build your AI leadership strategy]({{ '/lessons/build-your-ai-leadership-strategy/' | relative_url }}).
That lesson was about finding bets that serve the business. This one answers the question that comes next,
and that most AI leaders face early on: **you've inherited a dozen pilots and the board wants three. How do
you decide?**

## Key pointers

- **Weigh value, feasibility and risk together.** Looking at any one of them alone gives the wrong answer.
- **A matrix drawn from intuition is just advocacy with axes.** Weighted scoring makes prioritisation
  defensible: score each candidate on fixed criteria, weight each criterion to reflect what you value, and
  take the weighted average.
- **In regulated settings, risk may weigh far heavier, or act as a gate outright.**
- **Beware the clustering trap.** When everything is a priority, nothing is. It's what renders most
  prioritisation matrices useless.
- **High feasibility alone is never a reason to fund.** Easy isn't the same as valuable.
- **Value first.** Let feasibility and risk shape the sequence and the prerequisites, not override value in
  selection.

## The framework: The Value–Feasibility–Risk Sort

### The five moves

| Move | What you do | Why it matters |
|---|---|---|
| 1. **Normalise** | Put every candidate on a common canvas, described the same way. | You can't compare a vendor demo with a half-built prototype. |
| 2. **Agree criteria** | Fix the scoring criteria and their weights, set by strategy and risk appetite. | Weights decided up front stop people arguing backwards from their favourite. |
| 3. **Score independently** | Each evaluator scores alone, then the group discusses where scores diverge. | Divergence is information. Don't just average it away. |
| 4. **Read the quadrants** | Place candidates on value vs feasibility. Tie each survivor to a KPI, a baseline and a target. | A pilot without a measurable target isn't ready to be prioritised. |
| 5. **Defend the order** | Be able to tell the CFO why each one is first, second or parked. | If you can't explain the order, it isn't a decision yet. |

### The four quadrants

|  | **Lower feasibility** | **High feasibility** |
|---|---|---|
| **High value** | **Strategic bets.** Worth the investment, but need prerequisite work first: data readiness, capability building, resolving dependencies. | **Priority now.** These advance first, with no ceremony and no debate. |
| **Lower value** | **Kill or defer.** Stay out of the portfolio. | **Quick wins.** Build confidence and momentum, but time-box them so they don't crowd out higher-value work. |

### The clustering trap

Left to intuition, most proposals land in the top-right corner. Sponsors rate their own ideas as high value
and high feasibility, so the "winners" are only perceived ones. The clustered proposals then compete for
attention, there's no clear priority, and decisions stall. Sponsors also tend to favour safe picks.

A related bias is **central tendency**: scores bunch in the safe middle, avoiding the extremes that would
force real decisions.

Four facilitation habits fix clustering:

1. **Set boundaries at the median.** Quadrant lines go at the group's median score, so half the candidates
   are always "lower". It's relative, by design.
2. **Keep absolute gates.** Some criteria, like unacceptable regulatory risk, rule a candidate out
   regardless of its average.
3. **Use the full range.** Push evaluators to spread their scores and avoid the safe middle.
4. **Demand evidence.** Any top-right candidate must show proof, not optimism.

### From ranked list to portfolio

A ranked list isn't a portfolio yet. Turn it into one in three steps:

1. **Assign quadrants.**
2. **Fine-rank the high-value candidates** using their weighted scores.
3. **Order by dependency.** What has to be true before each one can start?

Then check the mix. A healthy portfolio balances three kinds of work:

| Type | Role |
|---|---|
| **Quick wins** | Early results that build credibility |
| **Strategic bets** | Core functions, longer horizons |
| **Moonshots** | Capabilities you don't have yet |

## Case study: Meridian Insurance inherits twelve pilots

*Meridian is the fictional insurer used throughout this playbook. The numbers are illustrative.*

Meridian has just acquired a smaller insurer, and with it came twelve AI pilots in various states of
progress. The board gives the COO one quarter and funding for three.

**Normalise and agree criteria.** Each pilot gets a one-page summary in the same format: the problem, the KPI
it would move, the data it needs, and the evidence so far. The leadership team agrees the criteria and
weights before seeing any scores: **value 50%, feasibility 30%, risk 20%** (scored so that 5 means low
risk). Because Meridian is regulated, they add an **absolute gate**: anything scoring 1 on risk is out,
whatever its average.

**The first round falls into the clustering trap.** Five sponsors score their own pilots, and ten of the
twelve land between 3 and 4 on everything. Every pilot looks like a priority. The COO resets the exercise:
three evaluators score independently, they must use the full 1–5 range, and any 4 or 5 on value needs
evidence such as a KPI baseline or pilot results.

**Score independently and discuss divergences.** The biggest disagreement is on fraud flagging: claims scores
value at 5, IT scores feasibility at 2 because the fraud data sits in three systems. The discussion settles
on a feasibility of 3, with data consolidation named as a prerequisite.

**The results**, with quadrant lines at the median (3.5 on both value and feasibility):

| Pilot | Value | Feasibility | Risk | Weighted | Quadrant |
|---|---|---|---|---|---|
| Agent call summaries | 4 | 5 | 5 | 4.5 | Priority now |
| Automated claims triage (home) | 4 | 4 | 4 | 4.0 | Priority now |
| Fraud flagging on new claims | 5 | 3 | 3 | 4.0 | Strategic bet |
| Subrogation recovery prediction | 4 | 3 | 4 | 3.7 | Strategic bet |
| Underwriting assistant for commercial property | 5 | 2 | 3 | 3.7 | Strategic bet |
| Policy wording search for staff | 3 | 4 | 5 | 3.7 | Quick win |
| Dynamic renewal pricing | 5 | 3 | **1** | 3.6 | **Gated out** |
| Broker email drafting | 2 | 5 | 4 | 3.3 | Quick win |
| Invoice matching in finance | 2 | 4 | 4 | 3.0 | Quick win |
| Marketing image generation | 1 | 5 | 3 | 2.6 | Quick win |
| Customer FAQ chatbot | 2 | 3 | 3 | 2.5 | Kill or defer |
| CV screening for hiring | 2 | 3 | **1** | 2.1 | **Gated out** |

The gate does real work here. Dynamic renewal pricing has a higher weighted score than four other pilots,
but it fails the risk gate because of fairness rules on pricing, so it's out regardless.

**From ranked list to portfolio.** Following *value first*, the COO fine-ranks the high-value pilots and
then orders them by dependency:

| Order | Pilot | Type | Why it's here | KPI, baseline → target |
|---|---|---|---|---|
| 1st | Agent call summaries | Quick win | Ready now; builds credibility in the first 8 weeks | Average call handling time: 9.5 → 8 minutes |
| 2nd | Automated claims triage (home) | Strategic bet | Core claims function; starts once home claims data has an owner (see [lesson 2]({{ '/lessons/ai-literacy-for-business-leaders/' | relative_url }})) | Home claim cycle time: 15 → 11 days |
| 3rd | Fraud flagging on new claims | Strategic bet | Highest value; depends on triage's claims data pipeline and on consolidating fraud data | Fraud losses detected before payout: 22% → 35% |

**What happens to the rest.** The underwriting assistant is labelled a **moonshot**: high value, but Meridian
doesn't have the capability yet, so it gets a small research budget, not a pilot. Subrogation is first in
line for next quarter. The quick wins with lower value (broker email, invoice matching, marketing images)
are parked; policy wording search may run as a time-boxed six-week trial if the call summaries team has
capacity. The chatbot is stopped. Pricing and CV screening are closed on risk grounds.

**Defending the order to the CFO** takes three sentences: call summaries first because they're ready and
prove the approach; triage second because it's core to the claims KPI but needs its data owner; fraud third
because it's the most valuable but depends on the first two. That's the test: the order is explainable.

## Putting it to work

1. **List every pilot you've inherited** and write each one up on the same one-page canvas.
2. **Agree criteria and weights before anyone scores.** Decide whether any risk acts as an absolute gate.
3. **Score independently**, then spend the meeting on the divergences, not the averages.
4. **Set quadrant lines at the median** and require evidence for anything in the top right.
5. **Fine-rank high-value candidates, then order by dependency.** Check the mix of quick wins, strategic bets
   and moonshots.
6. **Tie each survivor to a KPI, a baseline and a target**, and write the one-sentence reason for its place
   in the order.

**Watch out for:**
- Letting sponsors score their own proposals.
- Scores bunching in the middle, so nothing stands out.
- Funding something only because it's easy.
- Letting feasibility override value in *selection*. It should shape *sequence*.
- Averaging away a serious risk that should have been a gate.
