# Thinking Skills for Cursor

Three Socratic dialogue skills for AI-assisted decision-making and analysis. Built for [Cursor](https://cursor.com) Agent Skills.

These skills turn your AI assistant into a sparring partner that challenges your thinking through structured back-and-forth, then helps you produce clean artifacts. They don't summarize, don't lecture, and don't decide for you.

## The Skills

### Absorb

Process new intel (research decks, strategy memos, experiment readouts) through dialogue. The AI reads the material, loads whatever project context it can find, then opens with the sharpest tension between the new intel and your existing assumptions. One question at a time until the key threads are covered, then helps you externalize insights into artifacts.

**Trigger phrases:** "absorb this", "let's process this", "new intel", "help me think through this"

### Harden

Stress-test an argument before the real audience sees it. The AI finds the biggest weaknesses in your case, pushes back on assumptions presented as evidence, and either helps you structure the argument for maximum impact or tells you it's not ready yet. Outputs a structured recommendation with conditions for success and the weakest link called out honestly.

**Trigger phrases:** "harden this", "stress test this", "challenge this argument", "help me build this case"

### Choose

Guide a tricky decision through dialogue, then produce a structured decision doc. Classifies decisions as Type 1 (hard to reverse, worth deliberating) or Type 2 (easy to reverse, bias to speed). Maps options with honest pros/cons, finds the user's lean, stress-tests it, then generates a full decision document.

**Trigger phrases:** "help me decide", "I need to make a call on", "stuck between", "tradeoff"

## Installation

1. Copy the skill folders into `.cursor/skills/` in any project:

```
your-project/
  .cursor/
    skills/
      thinking/
        absorb/SKILL.md
        harden/SKILL.md
        choose/SKILL.md
      ...
```

2. Copy the `templates/` folder somewhere in your project. The skills reference these when producing artifacts:
   - `decision-doc.md` -- used by `choose` and `harden` when structuring decisions
   - `insights.md` -- used by `absorb` when externalizing findings from research or analysis

3. That's it. The skills will show up in Cursor's agent skills and activate on the trigger phrases above.

## Making These Even Better

These skills work out of the box as dialogue frameworks. But they get significantly sharper when your AI can load real project context during the conversation.

Every skill has a "context loading" step where it looks for strategy docs, open questions, experiment results, and project history. Out of the box, it will work with whatever files are in your workspace. But the more structured your context is, the better the challenges become.

What this looks like in practice:

- **Without context:** "Do you have evidence for that?" (generic)
- **With context:** "Your v1 experiment showed a 3% conversion lift but only in mobile. This proposal assumes desktop parity. What changed?" (grounded)

If you want to go deeper, consider organizing your project knowledge in a way the AI can navigate: strategy docs, experiment results, key insights, open questions. The skills will automatically pick up whatever's available and use it to make challenges more specific and grounded.

## Dialogue Principles

All three skills share core constraints:

- **One question at a time.** No lists of questions. Ask, wait, build on the answer.
- **Build on their words.** Reference what the user just said. Conversation, not questionnaire.
- **Never summarize what they already read.** The user has the material. They need a thinking partner, not a recap.
- **Push for speed.** Most decisions are two-way doors. Call it when someone is overthinking a reversible choice.
- **Never decide for them.** Frame, probe, challenge, steelman. The final call is theirs.
