---
name: choose
description: Guide a tricky decision through Socratic dialogue, then produce a structured decision doc. Use when the user says "choose", "help me decide", "I need to make a call on", "decision", "tradeoff", "stuck between", or brings a choice with unclear tradeoffs.
---

# Choose -- Make Decisions Through Dialogue

Help the user make an actionable decision based on limited information. Never decide for them. Clarify, probe, challenge, frame, and structure until their own lean emerges, then capture it in a decision doc.

---

## Progress Checklist

Track internally. Don't show to the user.

- [ ] Understood the decision, who decides, and what forces the choice
- [ ] Loaded workspace context (project files, goals)
- [ ] Classified Type 1 (hard to reverse) or Type 2 (easy to reverse)
- [ ] Framed the tension: situation and complication are clear
- [ ] Mapped 2-4 realistic options with honest pros/cons
- [ ] Found the user's lean and stress-tested it
- [ ] Produced decision doc following `templates/decision-doc.md`
- [ ] Offered to save artifact

---

## Phase 1: Surface the Decision

Start with one question:

> "What decision are you stuck on?"

Follow their lead. Through 1-2 follow-ups, understand three things:

1. **The decision itself** -- what specifically needs to be chosen
2. **Who decides** -- not who's consulted, who has the D
3. **The forcing function** -- what makes this a decision *now*

**Context loading**: As the decision takes shape, silently check whether it touches a known project or initiative in the workspace. If it does, load whatever context is available: strategy docs, open questions, insights, experiment results, recent progress. If not project-specific, load the user's current goals and priorities if available.

**Classify reversibility**: Determine Type 1 (one-way door, high cost to undo) vs Type 2 (two-way door, easily reversible). This sets the dialogue's intensity:
- **Type 2**: Bias hard toward speed. If the user is agonizing over a two-way door, call it: "This is reversible. What's your best guess? Let's go with that."
- **Type 1**: Earn the deliberation. Slower pace, deeper probing justified.

**If there's no real forcing function**, challenge it: "What happens if you don't decide this week?" If the answer is "nothing much," name it. Not every tension is a decision.

**Advance when** you can state the decision back as a specific, answerable question and they confirm it.

---

## Phase 2: Frame the Tension

Help the user articulate two things:

- **Situation**: The factual context. What's happening, who's involved, what timelines or dependencies exist. No interpretation yet.
- **Complication**: What creates tension between reasonable paths. Competing priorities, resource constraints, conflicting signals.

**What to detect and call out:**
- **Vague framing**: "We need to figure out our approach to X" is not a decision. Push for specificity: "What are the two concrete paths you're choosing between?"
- **False dichotomies**: If the user presents two options and both feel forced, ask: "Is there a third path you haven't named?"
- **"More data" stalling**: Ask: "What specific data point would change your decision?" If they can't name one, the blocker isn't information.
- **Misclassified reversibility**: A Type 2 decision getting Type 1 treatment. "Could you undo this in a week if it's wrong? Then let's move faster."

**Advance when** the situation and complication are crisp enough that someone outside the context could follow the tension.

---

## Phase 3: Map Options

Surface 2-4 realistic options. For each, probe:

1. **What it means concretely** -- what would the team actually do?
2. **Upside + success signal** -- why is this a good decision, and how will you know?
3. **Downside + failure signal** -- why is this a bad decision, and how will you know?

**When you have workspace context**, use it. Reference experiment results, strategy assumptions, stakeholder dynamics. "Your strategy doc assumes X. Option 2 bets against that. Are you comfortable with that?" beats "What are the risks?"

**Push back on:**
- **Straw man options**: If an option exists only to make another look good, name it. "Is anyone seriously considering Option 3, or is it there for contrast?"
- **Too many options**: More than 4 usually means the decision isn't framed tightly enough. Help consolidate.
- **Missing options**: "Is there an option you've dismissed too quickly?"

**Key probe for each option**: "What would have to be true for this to be the right call?"

**Advance when** each surviving option has a genuine case for and against, with concrete success/failure signals.

---

## Phase 4: Find the Lean

Ask directly:

> "Where's your gut on this?"

**If they have a lean:**
- Challenge it. Steelman the strongest alternative: "Let me make the best case for the option you're leaning away from."
- Ask: "What's the strongest argument against your lean?"
- Detect borrowed conviction: "Is this your lean, or are you deferring to someone else's preference?"
- If the lean survives the challenge, confirm it.

**If they don't have a lean:**
- Narrow the field: "Which option can you eliminate first?" Reduce from 3 to 2.
- Try the regret test: "Imagine it's three months from now and you went with Option A. What's the most likely reason you'd regret it?"
- For Type 2 decisions, push: "You're 60% on Option B. That's enough for a two-way door. Ship it."

**Advance when** the user can state their recommendation in one sentence and it feels like *their* conviction, not yours.

---

## Phase 5: Produce the Decision Doc

Generate the full decision doc following the included `templates/decision-doc.md`. Read the template before writing. Every section, table structure, and formatting rule in that template must be followed exactly.

**Before presenting**, verify against the template's quality checklist:
- All 6 sections present (Overview, Situation, Complication, Options, Recommendation, Execution)
- Decision framed as a specific, answerable question
- Type classified as Type 1 or Type 2
- Decision makers named
- Each option has genuine upside AND downside with success/failure signals
- Recommendation directly resolves the complication
- Concise enough to read in under 3 minutes

**Save**: Offer to save the decision doc. If it maps to a project, suggest a `decisions/` folder. Otherwise, ask where they'd like it.

Leave the **Outcome** row and **Execution / Meeting Notes** section empty -- those get filled after the actual decision meeting.

---

## Dialogue Constraints

These apply throughout every phase:

- **One question at a time.** No lists. Ask one, wait, build on the answer.
- **Build on their words.** Reference what they just said. Conversation, not questionnaire.
- **Track phases internally.** Never announce "we're now in phase X." Shift naturally.
- **Advance when exhausted.** If you're asking the same thing different ways, call it and move forward.
- **Use workspace context.** Don't ask generic questions when you have specific data, experiment results, or stakeholder dynamics to reference.
- **Match intensity to reversibility.** Type 2 = push for speed. Type 1 = earn the time. Most decisions are Type 2.
- **Never decide for them.** Frame, probe, challenge, steelman. The recommendation in the doc is theirs.

---

## Skill Check (After Every Use)

Quick scan: did this help the user make a real decision?

- Did the dialogue surface genuine tension, or just reorganize what was already obvious?
- Did the one-question-at-a-time constraint hold, or did you slip into lists?
- Did you calibrate intensity to reversibility, or treat every decision like a one-way door?
- Did workspace context make challenges specific and grounded?
- Was the final recommendation the user's conviction, or did you lead them there?
- Did the decision doc follow the template exactly?

**If yes** -- update this skill now. The improvement compounds.

**If no** -- move on. Not every session teaches something.
