---
name: weekly-workout
description: Picks the next workouts from your plan and formats them as a markdown checklist. Tracks progress across weeks so you always know where you left off.
---

When generating the weekly workout plan:

## Steps

1. **Figure out where the user left off**:
   - Check if a current `Week of *.md` file exists in the workouts folder (see config.md for path)
   - If it exists, read it and find the last workout day number mentioned. That's the last day assigned.
   - If no note exists, fall back to reading the tracker file (`workout_tracker.json` in the workouts folder) and use `last_completed_day`.
   - The next workouts should start AFTER this last day number.

2. **Read the workout source file** (path in config.md).

3. **Identify the next N workouts** (default: 3) starting after `last_completed_day`.
   - Use the workout types defined in config.md to determine which workout days to include vs. skip
   - For example, if config says "strength only", skip cardio/interval days

4. **Archive the previous week's note** before creating the new one:
   - Check if any `Week of *.md` file exists in the workouts folder
   - If it exists, MOVE it to the `History/` subfolder (create if needed)
   - This preserves the user's checked-off boxes as a progress log

5. **Calculate the week name**: Find the closest upcoming Sunday (or today if Sunday). Name the file `Week of {Month} {Day}.md`.

6. **Format output as Obsidian-compatible markdown** with `- [ ]` checkboxes:

```
**Workout 1 — Day {N} ({Type})**
- [ ] Warm Up: {warmup details}
- [ ] A1: {exercise} {reps}x{sets}
- [ ] A2: {exercise} {reps}x{sets}
- [ ] B1: {exercise} {reps}x{sets}
- [ ] B2: {exercise} {reps}x{sets}
- [ ] C: {finisher}
- [ ] Cool Down: {cooldown details}

---

(repeat for each workout)
```

7. **Save the file** to the workouts folder path from config.md.

8. **Update the tracker** — After generating workouts, update `workout_tracker.json`:
   - Set `last_completed_day` to the day number of the LAST workout picked
   - Update `last_updated` to today's date

## Important Notes
- Use clean, concise exercise names
- Include reps and sets in format like `12x3` or `10/side x3`
- Group supersets together (A1/A2, B1/B2)
- Always include warm up and cool down
- Tell the user which days were picked and which were skipped (and why)
- If the plan wraps around (all days completed), start from Day 1

## Folder Structure
```
Workouts/
  Week of Feb 1.md        ← current week (only 1 file here)
  workout_tracker.json    ← tracks last completed day
  History/
    Week of Jan 25.md     ← archived with checkboxes preserved
    ...
```
