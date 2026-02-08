# Weekly Workout — Config

Fill in your details below. The skill reads this file to know your workout plan and preferences.

---

## File Paths

```
# Where your workout notes live
workouts_path: ~/path/to/your/notes/Workouts/

# Your workout plan source file (a markdown file with all your workouts listed by day)
workout_plan_path: ~/path/to/your/workouts/My Workout Plan.md

# Archive folder
archive_path: ~/path/to/your/notes/Workouts/History/
```

---

## Workout Plan Structure

Describe how your workout plan is organized:

- **Total days in plan**: (e.g., 28, 35, 42 — however many days your program has)
- **Workouts per week**: (e.g., 3)

### Workout types to INCLUDE
List the types of workouts you want the skill to pick from:
- (e.g., Full Body Resistance)
- (e.g., Lower Body)
- (e.g., Upper Body)

### Workout types to SKIP
List types the skill should skip when picking the next workouts:
- (e.g., Cardio)
- (e.g., Intervals)
- (e.g., Rest days)

### Day mapping (which days are which type)
List your workout days in order. Example:
```
Day 1: Full Body (include)
Day 2: Cardio (skip)
Day 3: Lower Body (include)
Day 4: Rest (skip)
Day 5: Upper Body (include)
...
```

---

## Formatting Preferences

- **Include warm up**: Yes / No
- **Include cool down**: Yes / No
- **Group supersets**: Yes / No (A1/A2, B1/B2 format)
- **Rep format**: `12x3` (reps x sets)

---

## Notes

Add any context:
- (e.g., "I work out at home with dumbbells and bands")
- (e.g., "Skip exercises that need a cable machine")
- (e.g., "I prefer morning workouts Mon/Wed/Fri")
