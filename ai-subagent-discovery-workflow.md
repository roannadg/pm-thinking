# LinkedIn Article Draft — Subagent Discovery Workflow
Status: Draft. Needs refinement before publishing.

Notes before publishing:
- Decide whether to name Mohit Mamoria or just reference "an article I came across" — tagging him would get more reach
- Add a specific example with numbers (10 interviews, 3 data sources, X themes) to make it more concrete
- Length is ~550 words — good for LinkedIn

---

**I stopped using AI to summarise my customer research. Here's what I do instead.**

For a while, my AI workflow looked like this: finish a batch of customer interviews, paste the transcripts in, ask for a summary, get a tidy list of themes back.

It felt efficient. It was not.

The summaries were coherent and well-organised and almost completely useless. AI groups by surface language. Two customers saying "the reporting is frustrating" get filed under the same theme. But one of them meant the data takes too long to load. The other meant they can't share it with their manager. Different problems. Different fixes. Filed together.

I was getting polished output on questions I hadn't actually asked yet.

---

I came across an article by Mohit Mamoria about running parallel AI agents on research — treating Claude as a team rather than a single assistant. The idea is that instead of feeding data in sequentially and asking for a summary at the end, you run multiple agents simultaneously across different data sources: interviews, support tickets, surveys. Each one extracts raw problems. Then you bring the outputs together.

I tried it on a discovery sprint covering about ten percent of our customer base.

The extraction step — pulling raw problems from each source — took under an hour. What used to take two days of manual synthesis.

But here's the part that matters: the clustering is still yours.

I took the extracted problems and grouped them myself. Not by category. By what I thought was actually happening underneath. That's where the AI falls short — it doesn't know that two complaints with different words are the same root cause, or that two complaints with identical words are completely different problems that need different solutions.

After clustering, I used AI again to build what I now call a feature signal matrix. Themes on one axis, data sources on the other. It shows you where a theme appears across interviews AND support tickets AND surveys (strong signal) versus where it only showed up once in a single conversation (weak signal, probably don't act on it yet).

Then I sized the themes commercially. Frequency times impact times dissatisfaction. AI will weight by frequency every time. But the most frequently mentioned problem is rarely the most commercially important one. That call is yours.

The output was the clearest discovery brief I'd produced. Not because the AI was smarter. Because I was faster to the point where my judgment actually mattered.

---

The one-liner I keep coming back to: AI is good at the extraction. I'm good at the prioritisation. I use it to surface what's there, not to decide what matters.

If you're using AI to summarise your research, you're outsourcing the wrong step. The synthesis is where the insight lives. That's the job.

---

*What does your AI-in-discovery workflow actually look like? Genuinely curious what's working.*
