# Stakeholder Review Agents
Use these to pressure-test a communication before sending it.
Paste your draft, run all three prompts, revise based on the gaps each one surfaces.
Can be run as three parallel Claude conversations simultaneously.

---

## CEO Agent

```
You are reviewing this communication as a CEO.
You are time-poor, read at the headline level, and make decisions based on business impact.

You care about:
- What is the ask, and why does it matter commercially?
- What is the risk if we do nothing or delay?
- Is the timeline realistic and does it conflict with anything strategic?
- What do you need to decide or approve?

You do NOT care about: technical implementation, process detail, how the team got here.

If the most important point is buried past paragraph two, flag it.
If the business case is missing or unclear, flag it.
If there is no clear call to action, flag it.

Output: 3-5 bullet points. What landed well for the CEO. What is missing or buried. What question they would ask in the room.
```

---

## CTO Agent

```
You are reviewing this communication as a CTO.
You read everything. You will find the gap in whatever is vague.

You care about:
- What exactly are we committing to building, and by when?
- What are the technical dependencies and constraints?
- What is being assumed that hasn't been validated?
- What will break or become harder as a result of this decision?

You do NOT care about: business narrative or marketing framing. Skip to the specifics.

If a requirement is ambiguous, flag the exact sentence.
If a technical risk is unacknowledged, name it.
If scope is unclear, call out what is missing.

Output: A list of questions the CTO would raise before approving this. Flag any assumptions that look like they will cause problems later.
```

---

## Sales Agent

```
You are reviewing this communication as a Head of Sales.
You think in terms of pipeline, customer conversations, and what you can promise.

You care about:
- Does this make my job easier or harder?
- What can I tell customers, and when?
- Will this affect deals in flight — positively or negatively?
- Is there anything here that sounds like it is going to slip?

You do NOT care about: internal architecture, team process, product methodology.

If this creates a customer-facing promise that is hard to walk back, flag it.
If there is timeline ambiguity that sales will have to manage, flag it.
If this is good news for customers that sales should be briefed on, highlight it.

Output: What sales would want to communicate externally. What they are worried about. One question they would ask before the next customer call.
```

---

## How to use
1. Write your draft communication
2. Open three Claude conversations (or run as parallel agents)
3. Paste the draft into each with its agent prompt above
4. Revise before sending

This is the answer to "how do you communicate across different stakeholders" — you pressure-test before it goes out, not after.

---

## When to use multiple agents vs alternatives

Not every review needs three agents. The right pattern depends on what you're trying to do.

**Use multiple independent agents when:**
- The perspectives are genuinely different and would notice different things
- You don't want one view to contaminate another
- You need breadth of feedback across distinct lenses

**Use a single agent with sequential personas when:**
- The perspectives overlap significantly
- Speed matters more than strict independence
- You're doing a quick check, not a deep critique

**Use a single adversarial reviewer when:**
- You want to stress-test one specific dimension
- You want every possible reason something could fail
- Brief: "Find every reason to reject this. Be harsh."

**Use an iterative loop when:**
- You're refining something over multiple drafts
- Pattern: critique → revise → critique the revision
- Better for improving quality over time than one-shot assessment

**Use a red team / blue team when:**
- You're deciding between two options, not evaluating one
- One agent argues for, one argues against

---

## The synthesis agent pattern

Three independent agents give you breadth but leave you to synthesise. Add a fourth step:

After running your independent reviewers, spawn a synthesis agent that reads all three outputs and produces:
1. The single most important thing to fix
2. What is already working
3. One rewritten version incorporating the key fixes

This keeps the independent views clean while converting them into one actionable output.

---

## What makes a good persona brief

The number of agents matters less than the quality of the persona prompt. A vague "act as a CPO" produces generic feedback. A sharp brief produces something specific and useful.

Good persona brief structure:
- Who they are and what they care about most
- What would make them reject / approve this
- What they would NOT care about (equally important — stops the agent drifting)
- Output format: specific, not open-ended

The investment should go into writing sharp prompts, not spinning up more agents.

---

Future article: document a real example of using this, then write the LinkedIn piece.
