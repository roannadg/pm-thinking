# Opportunity Framing — AI in Allied Health (Azita Discovery)

Based on: interview with Azita Deljo, March 2026
Source: `Azita interview summary.md`

---

## Desired Outcome (for this discovery)

Understand where AI could meaningfully reduce practitioner burden in solo allied health practices — without replacing clinical judgement.

---

## Opportunity 1: Billing follow-up for failed payments

**Framing (customer's voice):**
"When automatic billing fails, I have to chase each case manually — Medicare, TAC, NDIS, private — and every case is different. So I put it off. Sometimes for two years."

**Why this is an opportunity:**
- 10% of billing fails automatic processing — not a tiny edge case
- Each failure requires individual diagnosis and follow-up (different payer, different reason)
- Azita is a psychologist — this task is cognitively mismatched with her skills and identity
- Real money delayed or written off as a result
- No current solution. Halaxy handles the 90% that works. The 10% that doesn't has nothing.

**Importance:** High — affects income and practice viability
**Satisfaction:** Very low — frequently put off, money lost
**Opportunity Score:** High

**What good looks like (Azita's words):**
"An AI equivalent of a bookkeeper — identifies what's unpaid, why, and what to do about it."

**What this is NOT:**
Not replacing a bookkeeper. Not re-doing Halaxy's auto-payment function. The gap is triage and next-step guidance on the failed cases.

**Key design constraints:**
- Must integrate with Halaxy or work alongside it
- Must handle multiple Australian payer types (Medicare, TAC, NDIS, private insurer)
- Trust framing: AI surfaces what to do, practitioner executes — not autonomous resolution

---

## Opportunity 2: EEG interpretation for neurofeedback

**Framing (customer's voice):**
"Session to session, I need to know whether the brain wave patterns are moving in the right direction. Right now I'm doing it by eye, or paying $200 an hour for a mentor."

**Why this is an opportunity:**
- Neurofeedback is a growing modality — Azita is transitioning her whole practice toward it
- No accessible AI tool exists for solo practitioners doing session-to-session EEG comparison
- Enterprise tools exist (expensive, clinic-grade) — solo practitioner gap is unserved
- Azita confirmed she will buy neurofeedback software (~$10,000) in 1-2 months and offered to collaborate directly — rare access to test with real clinical data

**Importance:** High — core clinical competency, directly affects treatment quality
**Satisfaction:** Very low — expensive workaround ($200/hour mentor), slow, no scalable solution
**Opportunity Score:** High — but longer time horizon than Opportunity 1

**What good looks like:**
AI reads session EEG data, compares to prior session, flags whether key markers are moving in the target direction, surfaces anomalies for clinician review. Clinician makes the call. AI removes the manual reading burden.

**Key design constraints:**
- Must work with the neurofeedback software she buys (need to identify what she purchases)
- Not autonomous interpretation — AI as pattern-surface layer, clinician as decision-maker
- Azita has 20+ years experience — tool needs to earn trust with a sophisticated user

---

## Prioritisation

| Opportunity | Importance | Satisfaction | Time horizon | Recommended next step |
|-------------|------------|--------------|--------------|----------------------|
| Billing follow-up | High | Very low | Near-term | Research Halaxy API + payer types. Interview 2-3 more practitioners to test generalisability. |
| EEG interpretation | High | Very low | Medium-term (dependent on her software purchase) | Follow up with Azita in ~2 months. Research existing QEEG AI tools to understand gap. |

**Near-term bet:** Billing follow-up. More generalisable across allied health (not specific to neurofeedback). Faster to prototype. Lower regulatory complexity.

**Longer bet:** EEG interpretation. Higher differentiation. Direct collaboration offer from Azita. Requires her to buy the software first.

---

## What's out of scope (for now)

**Report writing** — medium pain, medium satisfaction. Templates mostly solve this. AI report writing exists. Azita's specific constraint (Farsi notes) is addressable but not the biggest lever.

**AI report quality in the market** — Azita flagged junior practitioners signing AI-generated reports with errors. Real concern, but a training/policy problem, not a product problem for this discovery.

---

## Discovery next steps

| When | Action |
|------|--------|
| April 2026 | Research Halaxy API and feature set — what does it expose? What gaps exist? |
| April 2026 | Interview 2-3 younger practitioners — do they have the same billing pain? How do they handle it? |
| April 2026 | Research existing AI tools for QEEG interpretation — BrainDX, Neurosity, others |
| June 2026 (approx) | Follow up with Azita once she buys neurofeedback software — she offered direct access for testing |
