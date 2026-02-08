---
name: yearly-goals
description: Monthly reflection on yearly goals using a bingo card format. Reviews progress, updates statuses, tracks momentum, and keeps you accountable so goals don't drift.
---

When running the yearly goals review:

## Step 1: Read the current goals file

Read the goals file (path in config.md). This is the single source of truth.

## Step 2: Determine the current month

Use today's date to figure out which month we're reviewing. If it's early in a month (1st-5th), ask if they want to review the previous month or the current one.

## Step 3: Gather updates from the user

For EACH goal defined in config.md, ask a short, specific question. Don't make it feel like a quiz — keep it conversational and encouraging. Group related goals together by category.

Example flow:

**Health & Wellness**
- "How's [health goal] going? Where are you at?"

**Career & Money**
- "Any movement on [career goal]?"
- "How's [financial goal] tracking?"

**Personal / Family**
- "Any progress on [personal goal]?"

**Big Goals**
- "Where are things with [big goal]?"

## Step 4: Update the goals file

### A. Progress Tracker table
- Update the **Status** column: ⬜ Not Started → 🟡 In Progress → ✅ Done
- Update the **Notes** column with latest info

### B. Monthly Check-in section
Fill in the current month's section:

```markdown
### {Month}
**Date**: {today's date}

| Goal | Update | Momentum |
|------|--------|----------|
| {goal 1} | {update} | {🟢 on track / 🟡 slow / 🔴 stalled} |
| {goal 2} | {update} | {🟢/🟡/🔴} |
| ... | ... | ... |

**Wins this month**:
- {highlight 1}
- {highlight 2}

**Honest check-in**: {1-2 sentences — what's working, what's slipping}

**One thing to focus on next month**: {pick the goal that needs the most attention}
```

### C. Update end-of-year counters
- Update "Goals completed: _/{total}" count if any goals hit ✅

## Step 5: Save and confirm

Save the updated file. Give the user a quick summary:
- How many goals are 🟢 vs 🟡 vs 🔴
- Which goal needs the most attention
- Something encouraging about what IS working
- Remind them: "Same time next month?"

## Tone

- Supportive, not judgmental
- Celebrate what's moving, gently flag what's stalling
- Don't sugarcoat — honesty is the point — but lead with wins
- Keep it conversational. This is a check-in with yourself, not a performance review.

## Important Notes

- The goals file is the SINGLE source of truth — always read before updating, always save after
- Never delete previous months' check-ins — they're the history
- If a goal is completed mid-year, mark it ✅ and celebrate! Don't keep asking about it.
- If the user says "nothing happened" for a goal, that's OK. Log it honestly.
