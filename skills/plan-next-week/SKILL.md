---
name: plan-next-week
description: Sunday weekly setup — reflects on last week, takes a brain dump, and generates a structured weekly plan as an Obsidian note with checkboxes. Covers home tasks, appointments, meals, groceries, movement, and tracking metrics.
---

When planning next week:

## Steps

### Step 1: Weekly Reflection (before planning)
Before jumping into the new week, review the PREVIOUS week first.

1. Read the current `Week of *.md` file in the weekly notes folder (see config.md for path)
2. Scan all checkboxes and categorize:
   - **Completed** (`- [x]`): what got done
   - **Incomplete** (`- [ ]`): what didn't get done
3. Present a reflection summary to the user with these sections:

**What you crushed this week:**
- List completed items, grouped by category (home, appointments, movement, content, etc.)
- Call out wins — especially things that took effort or were new

**What didn't happen:**
- List incomplete items
- No judgment — just surface them clearly

**Patterns & observations:**
- Note any patterns (e.g. "Movement dropped off mid-week", "Meal prep consistency improving")
- Compare to the week's stated goal/theme if one exists

**Carry-forward items:**
- Ask which incomplete items should carry forward vs. drop entirely

4. Then ask the user:
   - "How do you feel about this week overall?"
   - "Anything you want to do differently next week?"
5. Use their answers to inform the new week's plan

Only AFTER the reflection conversation is done, move to Step 2.

### Step 2: Get the brain dump
- The user will paste or describe their weekly notes (messy is fine)
- If they don't provide notes, ask: "What's on your plate this week? Dump it all — home stuff, appointments, meals you're thinking about, anything."

### Step 3: Check the Meal Roster (if configured)
If the user has a meal roster file configured in config.md:

1. Read the Meal Roster file
2. Look at available meals and rotation history
3. Suggest meals that HAVEN'T been made recently to keep variety
4. If there are "New to Try" entries not yet tried, suggest one
5. If user doesn't specify meals, pick from the roster and confirm with them

If no meal roster is configured, ask the user what meals they're thinking about.

### Step 3b: Check if workouts need planning
- If the user mentions workouts are already planned, just add tracking checkboxes
- If workouts are NOT mentioned, ask: "Want me to help plan workouts for the week, or already handled?"
- Include a Movement section with checkboxes based on user's config

### Step 4: Ask quick clarifying questions (if needed)
Only ask if the brain dump is missing key info. Don't over-ask — if the brain dump covers it, just go.

### Step 5: Archive the previous week
1. Check for any existing `Week of *.md` file in the weekly notes folder
2. If one exists, MOVE it to the `History/` subfolder (create if needed)
3. This preserves checked-off checkboxes as a record

### Step 6: Build the weekly note
Calculate the week's starting date (use Sunday as week start by default). Name the file `Week of {Month} {Day}.md`.

Parse the brain dump and organize into sections. Save to the weekly notes path from config.md.

### Step 7: Update the Meal Roster (if configured)
Add a row to the rotation history table tracking what was planned this week.

### Step 8: Confirm with the user
Show a quick summary:
- File saved + location
- Meals at a glance
- Anything you assumed or defaulted

---

## Output Format

Use this structure for the Obsidian note (adjust sections based on config.md):

```markdown
> {User's stated goal or theme for the week}

---

## Home Tasks
- [ ] {task from brain dump}
- [ ] {task from brain dump}
{skip sections that don't apply this week}

---

## Appointments / Meetups
- [ ] {appointment 1}
- [ ] {appointment 2}

---

## Movement
- [ ] {workout or activity 1}
- [ ] {workout or activity 2}
- [ ] {weekend activity}
{Adjust based on user's movement preferences in config.md}

---

## Meals

| Meal | Mon | Tue | Wed | Thu | Fri | Sat | Sun |
|------|-----|-----|-----|-----|-----|-----|-----|
| Breakfast | {meal} | {meal} | {meal} | {meal} | {meal} | {meal} | {meal} |
| Lunch | {meal} | {meal} | {meal} | {meal} | {meal} | {meal} | {meal} |
| Snack | {snack} | {snack} | {snack} | {snack} | {snack} | {snack} | {snack} |
| Dinner | {meal} | {meal} | {meal} | {meal} | {meal} | {meal} | {meal} |

{Include protein estimates if health goals are configured}
{Adjust meal structure to match household in config.md}

---

## Grocery List

**Protein**
- [ ] {item}

**Produce**
- [ ] {item}

**Dairy**
- [ ] {item}

**Pantry**
- [ ] {item}

**Check Staples**
- [ ] {staple items from config}

{Skip grocery section on weeks with no cooking}

---

## Tracking

| Metric | This Week | Baseline |
|--------|-----------|----------|
| {metric from config} | | {value} |

{Only include metrics the user configured — this section is optional}
```

---

## Important Notes
- Keep checkboxes as `- [ ]` for Obsidian compatibility (tappable on phone)
- Grocery list gets checkboxes too (check items off while shopping)
- If user provides partial info, fill in reasonable defaults and FLAG what you assumed
- If a section doesn't apply this week, skip it entirely
- ONE file per week. Old weeks go to History/.
- Read config.md for all user-specific settings (paths, meals, health goals, household info)
