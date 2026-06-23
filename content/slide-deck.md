---
title: "AI in Delivery"
subtitle: "Leading Projects That Ship"
author: "Dr. Michael Borck"
format:
  html:
    embed-resources: true
  pdf: default
  docx: default
  pptx: default
---


# Welcome

![](./images/opening-humans-ai-collaboration.png)

**AI in Delivery — Leading Projects That Ship**

::: {.notes}
- "Today is hands-on. You'll scope, staff, stress-test and decide on a real AI project — and you'll do it by talking to the people who'd actually make or break it."
- "You'll work hard, make uncomfortable calls, and leave with a project design, not a folder of notes."
:::

---

# The question you came in with

> *"Why is delivering an AI project any different from delivering any other project?"*

**That's the question we answer today — and then you go do it.**

::: {.notes}
- This is the hook. Most of the room is here because they sense AI is *different* but can't articulate how — and they're tired of being told "it's just change management."
- "By morning tea you'll have a clear, defensible answer. By the end of the day you'll have led one."
- Resist the urge to reassure with the old '80% of projects fail' stat. The point isn't that AI projects fail more — it's that they fail *differently*, and you have to lead for that difference.
:::

---

# Today's Journey

- 9:00–10:30 → **Why AI is different** (foundations + the trust tool)
- 10:30–11:00 → Morning Tea
- 11:00–12:30 → **Sprint 1: Scope it against reality**
- 12:30–1:15 → Lunch & Networking
- 1:15–2:30 → **Sprint 2: Stakeholders & human-in-the-loop**
- 2:30–3:00 → Afternoon Tea
- 3:00–4:00 → **Sprint 3: Roadmap, risk & the go/no-go call**
- 4:00–4:30 → **The edge that's left to humans + your action plan**

::: {.notes}
- "One project, carried all the way through. Each block hands you a piece of a real delivery design."
- "You'll spend the afternoon interviewing RetailFlow's leadership team — live — to build and defend your plan."
:::

---

# What you leave with

A **delivery design for a real AI project**:

- Scoped objectives, data requirements, and a defined "good enough"
- A delivery roadmap with milestones and go/no-go gates
- A stakeholder plan and a human-in-the-loop checkpoint design
- A risk register and a pilot-to-production path

::: {.notes}
- "Not a theory to apply later. A concrete design for a real scenario, stress-tested before you leave."
- Set expectations clearly (addresses prior feedback): "This is a leadership and delivery course. You'll *use* AI today, but the skill we're building is judgement — knowing where AI helps, where it quietly fails, and where you must stay in charge."
:::

---

# Why AI is different

![](./images/traditional-vs-ai-paths.png)

**Five things every project manager assumes — that AI breaks.**

::: {.notes}
- This is the new spine of the day. Walk the five contrasts that follow. Each one: the normal-project assumption → why AI breaks it → the leadership move it forces.
- Tie it together at the end with the summary slide. These five are the answer to the question they walked in with.
:::

---

# Difference 1 — "Done" can't be specified

**Normal projects:** you write acceptance criteria up front and test against them.

**AI:** output is *non-deterministic* and *doesn't reason*. Same input, different answer. Fluent and confident even when wrong. No spec pins the behaviour.

**The move:** you manage a **probability distribution of behaviour**, and "good enough" becomes a judgement you must define and defend — not a checkbox.

::: {.notes}
- Concrete: ask a model the same question twice, get two different answers. A normal QA team would file that as a bug. Here it's the nature of the material.
- "Doesn't reason" matters: it produces a convincing average of everything it has seen. That's brilliant for some tasks and quietly dangerous for others — which is exactly what the trust tool (next) helps you predict.
- Leadership implication: if you can't write a fixed spec, you have to define *fitness for purpose* before deployment, not discover it after.
:::

---

# Difference 2 — A working demo is a trap

**Normal projects:** a working demo means you're nearly there.

**AI:** the gap from demo to production is wide and *deceptive*. Something that works 9 times out of 10 looks 90% done — and is maybe 10% done. All the cost lives in the last 10%: the edge cases, the confident hallucinations, the adversarial inputs.

**The move:** kill the instinct that says *"we have a working version, we're nearly there."* **Progress is illusory.**

::: {.notes}
- This is the single most expensive misread in AI delivery. Executives see the demo, assume it ships next month, and set a board date. You are now late before you start.
- The demo is the *beginning* of the hard work, not the end of it.
- This reframes how you sequence the plan and where you put your gates (Sprint 3).
:::

---

# Difference 3 — The data is the uncertainty, and you discover it

**Normal projects:** requirements are the uncertainty; you nail them down, then build.

**AI:** the *data* is the uncertainty — and its real quality and availability are **discovered, not specified**. Feasibility can collapse mid-flight when the data isn't what everyone assumed.

**The move:** run the project as a **discovery process about your own organisation**, with gates that expect to find out you were wrong.

::: {.notes}
- RetailFlow preview: their data is "fragmented across systems," online and store data siloed, store-level operational data inconsistent. Priya will tell your groups this in Sprint 1 — if they ask.
- The leadership skill is humility built into the plan: assume the data will surprise you, and design checkpoints to catch it early rather than at launch.
:::

---

# Difference 4 — Verification is the product

**Normal projects:** QA is a phase near the end.

**AI:** because the output is plausible-but-sometimes-wrong, deciding **where a human checks, who has the judgement to check, and how much checking is enough** is the core design work — continuous, not a phase.

**The move:** you're not shipping a tool. You're shipping a **division of labour between human judgement and machine output.** Design it deliberately.

::: {.notes}
- This is the heart of "human-in-the-loop": not a compliance box, a design decision about *where judgement lives*.
- Sprint 2 is built on this. The two inserts (evaluator's advantage / apprenticeship pipeline) sharpen *who* the right human is and what it costs to build that judgement.
- "If you can't say where a human must stay in the loop and why, you haven't finished designing the system."
:::

---

# Difference 5 — Generic competence is now the baseline

**Normal projects:** more throughput = more value.

**AI:** when everyone runs the same models, **generically high-quality output with no variation is the baseline — not an edge.** If the AI is good at running your company, it's good at running every company.

**The move:** protect and inject the **human variation, judgement and taste** a competitor's identical model can't produce.

::: {.notes}
- This is a preview — we return to it as the closing frame of the day.
- "The whole organisation built to deliver the product matters less; the taste of the people inside it matters more."
- For a delivery lead this is sharp: 'done' isn't 'it works' — it's 'it carries judgement a rival running the same model can't get.'
:::

---

# The five differences

1. **"Done" can't be specified** → manage a distribution, define "good enough"
2. **The demo is a trap** → progress is illusory
3. **Data is discovered, not specified** → run it as organisational discovery
4. **Verification is the product** → design where judgement lives
5. **Generic is the baseline** → protect the human variation

**Every PM tool you know still applies — but each one bends under these five forces. Today you learn the bend.**

::: {.notes}
- This is the slide to photograph. It's the whole intellectual spine on one page.
- Make the meta-point explicit: "You already know roadmaps, risk registers, stakeholder maps. We're not replacing them. We're showing how AI distorts each one — and how to lead anyway."
:::

---

# A tool for the hardest call: when to trust AI

<!-- NEW VISUAL NEEDED: 2x2 trust-tool matrix — axes: Average↔Precise (x), Small↔Large stakes/scope (y) -->

**Average vs. Precise × Small vs. Large**

- AI excels at **average** answers over **small**, low-stakes work.
- It gets dangerous on **precise** answers and **large**, high-stakes work.

::: {.notes}
- This is the trust tool from *Conversation, Not Delegation* (the free companion resource for the whole series). It is the AI-specific lens that makes Difference 1 and Difference 4 actionable.
- "AI produces a convincing average. Where 'about right' is fine, lean in. Where exactly-right and high-stakes meet, a human stays in the loop."
- Groups will apply this to *their own* initiative in Sprint 1: which parts of the work are average-and-safe to automate, which are precise-and-high-stakes and must keep a human.
- michael-borck.github.io/conversation-not-delegation — point them here for "go deeper."
:::

---

# Live: meet RetailFlow's staff — and watch one fail

<!-- LIVE DEMO slide. Instructor talks to a RetailFlow virtual-staff chatbot on screen. -->

**Watch what happens when I ask it something it doesn't actually know.**

::: {.notes}
- THE WOW MOMENT. On screen, open a RetailFlow virtual-staff chatbot. Ask something reasonable, then ask for a specific policy/number it can't know (e.g. "what's RetailFlow's exact returns window for sale items?"). Let it confidently invent an answer.
- "That's Difference 1 and Difference 2 in your hand. It's fluent. It's confident. It's wrong. Now imagine that in front of a customer — or in your board pack."
- Then reframe: "This afternoon, these same staff are your information source and your stress-test. They disagree with each other. Your job is to lead anyway."
- Fallback if bots aren't live: use a screenshot/recording of the same exchange, or do it on any public model with a RetailFlow-style question.
:::

---

# Meet RetailFlow

50 stores • $150M revenue • 2,000 people • Australia

**The board has funded ONE AI initiative. You are the delivery lead. Ship it — without the predictable failures.**

::: {.notes}
- Realistic, fictional Australian fashion & homewares retailer. We use it all day.
- Shift from the old framing: this is not "should we invest?" (that's the Strategy course). The money is committed. Your job is delivery.
- Each group will take a *different* funded initiative, so no two designs look alike: customer-service chatbot, dynamic pricing, inventory optimisation, or fraud detection.
- "Your stakeholders are down the hall — Emma the Managing Director, Marcus the CIO, Priya in data, David in finance, Tom in customer service. You'll talk to them this afternoon."
:::

---

# Sprint 1 — Scope it against reality

![](./images/pilot-program.png)

**Interview Priya (Data) and Marcus (CIO). Reconcile "move fast" with "the data isn't ready."**

::: {.notes}
- Each group gets its assigned initiative card.
- Task: produce scoped objectives, data requirements, and a defined "good enough" — applying the trust tool to *this* project (what's average-and-safe vs precise-and-high-stakes).
- The deliberate tension: Marcus pushes speed and ambition; Priya gives realistic, data-grounded timelines. Your scope is the reconciliation.
- Live bots: groups interview Marcus and Priya. Text-persona fallback: hand out their profiles as briefing cards and have groups interrogate them on paper.
- 60 min work + debrief. Use a visible timer (prior feedback: tighten pacing).
:::

---

# Sprint 2 — Stakeholders & human-in-the-loop

![](./images/speed-dating.png)

**Interview Emma (Managing Director), Tom (Customer Service), David (CFO). Decide where a human must stay in the loop.**

::: {.notes}
- This is Difference 4 made concrete. Output: a stakeholder plan + a human-in-the-loop checkpoint design.
- Emma = board pressure and the promise made. Tom = the frontline team that gets automated. David = ROI and the go/no-go criteria.
- The two inserts (next slides) land right here, on Tom's team.
- Add the design prompt: for each checkpoint, name who actually has the expertise to evaluate the output — and whether that checkpoint *builds* that expertise or just *consumes* it.
:::

---

# Your experienced people are your AI advantage

- The myth: "digital natives" are "AI natives." Delivery reality is closer to the opposite.
- Juniors often become **conduits** — passing on fluent, polished AI output without the context to know it's wrong.
- Experienced staff have the **evaluator's advantage**: they spot the confident hallucination instantly, because they know what right looks like.
- **So:** human-in-the-loop is a *judgement* role — and judgement is unevenly distributed across your team. Staff your checkpoints accordingly.

::: {.notes}
- (Friday insert A.) This defuses AI anxiety: most of the room is experienced, and their experience is the asset, not the liability.
- It sets up the afternoon design decision: the checkpoints you build need the *right* humans on them, not just any human.
:::

---

# The second-order cost of the productivity win

- Experts were forged through **grunt work** — the repetitive tasks delegated to juniors. That work was where judgement got built.
- AI makes it cheaper to give that work to a machine than to a "slow, flawed" junior. Rational in the moment.
- But the grunt work was **how the next evaluator got made.** Automate all of it and you erode the pipeline that produces the experienced people you just said you depend on.
- A genuine **Catch-22**: short-term delivery speed vs. long-term team capability.

::: {.notes}
- (Friday insert B.) The "I hadn't thought of that" moment for a delivery audience.
- What a delivery lead can actually do: decide *deliberately* which work stays human for development reasons, not just quality; use AI-assisted work as a chance for juniors to *critique and verify* output (an evaluator skill) rather than just consume it; make it an explicit team-design choice in the plan.
- Tie to the workshop: when groups design checkpoints, mark which ones also build capability.
- Delivery note: keep this conceptual. Don't quote model versions or precise study figures from memory; if citing, name OpenAI's GDPval and say "recent studies suggest."
:::

---

# Sprint 3 — Roadmap, risk & the go/no-go call

![](./images/scale-pivot-kill-decision-tree.png)

**Build the roadmap. Then the staff push back, and a crisis hits. Defend your plan — or change it.**

::: {.notes}
- Output: delivery roadmap with go/no-go gates, a risk register, and a pilot-to-production path.
- Stress-test 1: the bots push back ("you promised the board this by Q3"). Stress-test 2: inject a crisis (data-quality / team-resistance / executive-pressure) and have them respond with DDCD — Diagnose → Decide → Communicate → Document.
- At the first gate, force the call: SCALE / PIVOT / KILL, defended with evidence. Reinforce: killing a bad project early is success, not failure.
- This is where the demo-to-production gap (Difference 2) bites — the gates exist because progress is illusory.
:::

---

# DDCD — leading through the inevitable crisis

**Diagnose → Decide → Communicate → Document**

- Is this a *technical*, *people*, *leadership*, or *ethical* crisis? They need different responses.
- Decide under uncertainty. Communicate to the right stakeholder. Document the call and why.

::: {.notes}
- Keep the proven crisis framework — it works. The change is that they apply it to *their own* plan, not a generic scenario.
- The four crisis types map back to the stakeholders they've met: data-quality (Priya), team-resistance (Tom), executive-pressure (Emma/David), ethical (everyone).
:::

---

# The edge that's left to humans

> *"If the AI is good at running your company, it's good at running every company. Generically high quality, with no variation, means no competitive edge. Humans bring the edge by providing variation — you start to care more about the taste of the person than the whole organisation built to deliver the product."*

**Where in your delivery did you protect the judgement a competitor's identical model can't get?**

::: {.notes}
- The closing frame. Return to Difference 5 and make it personal to the plan they just built.
- "Notice how generic your AI-assisted first draft was. That sameness *is* the lesson. What made a plan good was your judgement — where you kept a human, what you refused to automate, the taste you protected."
- This threads the whole series together: individual capability (Practice) → investment judgement (Strategy) → delivering judgement that lasts (Delivery).
:::

---

# Your Action Plan

![](./images/action-plan-growth-trajectory.png)

**This week** — one thing you'll do differently.
**This month** — one thing you'll change.
**This quarter** — one thing you'll transform.

::: {.notes}
- Make it personal and small. One concrete commitment with a defined "what good looks like."
- Required for CRL — have them complete it thoughtfully before they leave.
- Companion resource for going deeper: michael-borck.github.io/conversation-not-delegation
:::

---

![](./images/QR-Code-Feedback.png)

**Lead with humans in the loop. Protect the judgement only you bring.**

Dr. Michael Borck — michael.borck@curtin.edu.au

::: {.notes}
- "AI in Strategy is the sister course on *choosing* where to invest; AI in Practice builds the individual fluency underneath both."
- "Please take 3–4 minutes for feedback — it genuinely shapes the next iteration."
:::
