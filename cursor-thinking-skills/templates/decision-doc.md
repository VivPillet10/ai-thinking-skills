# Decision Document Template

A lightweight template for capturing key decisions with enough structure to make the reasoning traceable, but not so much that it slows you down.

## When to Use

- A decision involves multiple stakeholders or teams
- There are real tradeoffs between options (not just "should we do it?")
- The decision is worth documenting because you might revisit it later
- Cross-team coordination requires alignment on a path forward

## How to Use This Template

1. Read the **Template Structure** section below -- this is the exact document skeleton to produce
2. Read the **Section-by-Section Guide** for rules on filling each section
3. Read the **Formatting Rules** for tone, length, and style constraints
4. Fill the template, present it for decision, then update the **Outcome** row and **Execution / Meeting Notes** section after the call

---

## Template Structure

Copy this skeleton verbatim as the starting point. Every section header, table, and structural element below must appear in the final document. Do not add, remove, or rename sections.

```markdown
# **Decision: [Short Decision Topic]**

# **Overview**

| Decision | [Frame the decision as a specific question to answer] |
| ----: | :---- |
| **Type** | [Type 1 - Hard to reverse / Type 2 - Easy to reverse] |
| **Decision maker** | [Name(s) with email links] |
| **Outcome** | [Option chosen + date, plus any conditions. Fill after decision is made.] |

# **Situation**

* [What's happening? Set the factual scene. 2-4 bullets.]
* [Include specific initiatives, timelines, or dependencies that create the context.]

# **Complication**

* [What creates tension or forces a decision now? 2-4 bullets.]
* [Name the competing priorities, resource constraints, or risks.]

# **Options**

|  | Hypothesis / Description | Why is this a good decision, and how will we know? | Why is this a bad decision, and how will we know? |
| :---- | :---- | :---- | :---- |
| **Option 1:** [Name] | [1-2 sentences: what this option means concretely] | [Upside + success signal] | [Downside + failure signal] |
| **Option 2:** [Name] | [1-2 sentences: what this option means concretely] | [Upside + success signal] | [Downside + failure signal] |
| **Option 3:** [Name] | [1-2 sentences: what this option means concretely] | [Upside + success signal] | [Downside + failure signal] |

# **Recommendation**

* **Go with Option [N]:** [1 sentence stating the recommended option and what it means.]
* **Why:** [1-2 sentences with the core reasoning. Reference the complication directly.]

# **Execution / Meeting Notes**

* [Capture decisions, conditions, follow-ups from the discussion. Fill after the meeting.]
```

---

## Section-by-Section Guide

### Title

- Format: `Decision: [Topic]`
- The topic should name the tension, not just the subject area. "Classifier Badge Conflict" is better than "Badge Discussion."

### Overview Table

**Purpose:** Give any reader the full picture in 5 seconds: what's being decided, who decides, and what was chosen.

**Rules:**
- **Decision** row: Frame as a specific, answerable question. "How should X and Y coordinate when both need Z?" is good. "What should we do about badges?" is too vague.
- **Type** row: Use Amazon's Type 1 / Type 2 framework.
  - **Type 1 (Hard to reverse):** One-way doors. High cost to undo. Warrants more deliberation.
  - **Type 2 (Easy to reverse):** Two-way doors. Can be undone with low cost. Bias to speed.
- **Decision maker** row: Name the people who have authority to make the call. Include email links. These are not "consulted" or "informed" parties -- they are the deciders.
- **Outcome** row: Leave blank in the draft. Fill after the decision is made with: the chosen option, the date, and any conditions or caveats agreed upon.

### Situation

**Purpose:** Set the factual context so the reader understands the landscape without needing prior knowledge.

**Rules:**
- 2-4 bullets. Factual, not interpretive.
- Name the specific initiatives, teams, experiments, or timelines involved.
- Include enough detail that someone outside the immediate context can follow. Mention team names and initiative names explicitly.
- No opinion here. Save that for Complication and Recommendation.

### Complication

**Purpose:** Explain why a decision is needed now. What creates tension between reasonable paths?

**Rules:**
- 2-4 bullets. This is where you name the conflict.
- Identify competing priorities and make each side's case briefly. Show that both options have real merit.
- Be specific about costs: coordination overhead, timeline delays, resource constraints, analytical complexity.
- If there's a forcing function (deadline, dependency, resource constraint), name it.

### Options Table

**Purpose:** Lay out the realistic options with honest pros and cons for each.

**Rules:**
- 2-4 options. Three is typical. Don't pad with options nobody would seriously consider.
- **Option name:** Short, descriptive label. Use verbs when possible ("Run at the same time", "Take turns", not "Concurrent approach").
- **Hypothesis / Description:** 1-2 sentences explaining what this option means concretely. What would the team actually do?
- **Why good:** State the upside AND what success looks like. "Success = [observable outcome]" is a useful format.
- **Why bad:** State the downside AND what failure looks like. "Bad = [observable outcome]" is a useful format.
- Every option should have a genuine case for and against. If an option has no real downside, it's not a real tradeoff and probably doesn't need a decision doc.

### Recommendation

**Purpose:** State your recommended option clearly and explain why.

**Rules:**
- Lead with the option number and a 1-sentence description.
- Follow with "Why:" that directly addresses the complication. The recommendation should resolve the tension named in the Complication section.
- Keep it to 2-3 sentences total. The Options table already laid out the detailed reasoning.
- If the recommendation has conditions ("do X, but keep Y in mind for Q3"), state them here.

### Execution / Meeting Notes

**Purpose:** Capture what actually happened when the decision was discussed.

**Rules:**
- Fill after the decision meeting.
- Include: the final decision (if it differs from the recommendation), any conditions or follow-ups agreed upon, and who is responsible for what.
- Keep it brief. This is a record, not meeting minutes.

---

## Formatting Rules

These apply to the entire document:

- **Bold** section headers and option names
- Overview table uses right-aligned label column (`----:`) and left-aligned value column (`:----`)
- Options table uses left-aligned columns (`:----`)
- Links use inline markdown format `[text](mailto:email)` for people
- No em dashes in prose (use commas, periods, or "and")
- Keep prose direct. No filler phrases.
- The document should fit on one page when printed. If it doesn't, you're overwriting.

---

## Quality Checklist

Before sharing the decision doc, verify:

- [ ] All 6 sections are present: Overview, Situation, Complication, Options, Recommendation, Execution
- [ ] Decision is framed as a specific, answerable question in the Overview table
- [ ] Type is classified as Type 1 or Type 2
- [ ] Decision makers are named with email links
- [ ] Situation is factual, not interpretive
- [ ] Complication names competing priorities with specifics
- [ ] Each option has both a genuine upside and downside with success/failure signals
- [ ] Recommendation directly resolves the complication
- [ ] No filler prose, no em dashes
- [ ] Document is concise enough to read in under 3 minutes
