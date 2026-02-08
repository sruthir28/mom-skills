# Mom Skills

Claude skills for running the small org with zero budget, no direct reports, and constant scope creep.

It's called home.

---

## What are these?

[Claude skills](https://docs.anthropic.com/en/docs/claude-code/skills) are reusable instructions that live in `~/.claude/skills/` and teach Claude how to do specific tasks for you. Think of them as SOPs for your AI assistant.

These skills were built for the operational side of life — meal planning, weekly planning, workout tracking, goal accountability. The same kind of systems you'd build at work, applied to the chaos of running a household.

## Skills included

| Skill | What it does | Complexity |
|-------|-------------|------------|
| [**plan-next-week**](skills/plan-next-week/) | Sunday brain dump → structured weekly plan with meals, groceries, appointments, movement | Customizable template |
| [**weekly-workout**](skills/weekly-workout/) | Picks next workouts from your plan, formats as checkable list, tracks progress | Bring your own workout plan |
| [**yearly-goals**](skills/yearly-goals/) | Bingo-card style yearly goals with monthly check-ins and momentum tracking | Define your own goals |
| [**weekly-report**](skills/weekly-report/) | Raw notes → clean weekly status report | Ready to use |
| [**practical-ai-skills**](skills/practical-ai-skills/) | Consulting & PM frameworks (SCPR, Issue Trees, Storylines, RICE) | Ready to use |

## Quick start

### 1. Install a skill

Copy any skill folder into your Claude skills directory:

```bash
# Copy a single skill
cp -r skills/plan-next-week ~/.claude/skills/

# Or copy all of them
cp -r skills/* ~/.claude/skills/
```

### 2. Customize it

Most skills have a `config.md` file where you fill in your own details — your meals, your schedule, your goals. The `SKILL.md` file is the logic; `config.md` is your data.

### 3. Use it

Open Claude Code and the skills activate automatically based on context, or reference them directly:

```
"Plan my week — here's my brain dump: ..."
"Pull my next 3 workouts"
"Run my monthly goal check-in"
```

## Skill details

### plan-next-week

The big one. Sunday evening ritual:
1. Reflects on what got done (and didn't) last week
2. Takes your messy brain dump
3. Builds a structured weekly note with: home tasks, appointments, movement plan, meal plan (with protein targets), grocery list, and tracking metrics
4. Saves as an Obsidian note you can check off on your phone all week

**Setup**: Edit `config.md` with your household size, meal preferences, health goals, prep schedule, and weekly rhythm.

### weekly-workout

Tracks your position in any multi-week workout plan and serves up the next batch:
1. Figures out where you left off
2. Picks the next N workouts from your plan
3. Formats with checkboxes for Obsidian
4. Archives last week's completed workouts

**Setup**: Add your workout plan to `config.md` and adjust the workout types and structure.

### yearly-goals

Bingo card approach to annual goals — because a 3x3 grid is more fun than a list:
1. Monthly check-in on each goal
2. Tracks momentum (on track / slow / stalled)
3. Logs wins and honest assessments
4. Keeps a running history so you can see the arc

**Setup**: Define your 9 goals in `config.md` with targets and categories.

### weekly-report

No config needed. Give it your messy notes, meeting summaries, or stream of consciousness and it outputs a clean report: accomplishments, in-progress, blockers, next week priorities.

### practical-ai-skills

Consulting and PM frameworks, ready to use:
- **SCPR**: Situation-Complication-Problem-Recommendation
- **Issue Trees**: MECE problem decomposition
- **Storyline Builder**: Presentation decks where each line = one slide title
- **PM Prioritization**: RICE, Impact/Effort, Value/Complexity, Weighted Scoring

No config needed. Just ask Claude to apply any framework to your problem.

## How skills work

```
~/.claude/skills/
  plan-next-week/
    SKILL.md        ← the instructions Claude follows
    config.md       ← your personal settings (meals, schedule, goals)
  weekly-workout/
    SKILL.md
    config.md
  ...
```

Claude reads `SKILL.md` to know *what to do* and `config.md` to know *your specifics*. The skill logic is generic; your config makes it personal.

## Designed for Obsidian

These skills output Obsidian-compatible markdown with `- [ ]` checkboxes. If you use Obsidian synced to your phone (via iCloud, Obsidian Sync, etc.), you get tappable checklists wherever you go.

Not using Obsidian? The output is standard markdown — works with any notes app.

## Contributing

Found a way to make these better? Open a PR. Have a skill that helps you run your household or your work? I'd love to see it.

## Origin story

My husband called these "Mom Skills" — Claude skills... for moms. He's proud of that one.

Turns out the operational rigor we bring to work? Many of us learned it at home first.

---

*Built with [Claude Code](https://claude.ai/claude-code)*
