# Fitness App — Tu Entrenamiento

## Decisions
- Single-file static app (HTML/CSS/JS, no build step)
- Apple-inspired UI, mobile-first
- Push/Pull/Legs split with warm-up phases (bodyweight, dumbbells, multi-joint) + main workout
- GIFs auto-fetched from ExerciseDB with localStorage caching
- Workout progress persists in localStorage (resumes within 6 hours)
- Spanish language UI
- App is for Luigy's parents — designed for when the gym is packed, so every exercise includes alternatives in case the machine/bench is busy
- All main exercises: 4 sets, 6-10 reps, 45 seconds rest between sets
- Alternatives UI: each main exercise has an `alts` array with 2 alternatives. "Equipo ocupado?" button opens a bottom sheet with full GIF + coaching note per alternative — not just text references
- Each alternative has its own ExerciseDB GIF search term for auto-fetching

## Key Insights
- Warm-up phases are fully built out for all 3 routines
- Main workout phase is placeholder ("Ejercicios por definir") for push, pull, and legs
- Live at https://luigyroso.github.io/fitness/
- All GIF URLs are hardcoded with ExerciseDB static URLs as fallback/cache

## Tasks Done
- Built complete app structure with home screen, workout flow, rest timer, overview panel, completion screen
- Populated warm-up exercises for push, pull, and legs (bodyweight, dumbbell, multi-joint phases)
- Added GIF auto-fetch and caching system
- Added workout resume functionality
- Deployed to GitHub Pages
- Filled in Push main workout: bench press, incline bench, dips, lateral raises, military press, tricep extension
- Built alternatives UI system: "Equipo ocupado?" button + bottom sheet with GIF cards and coaching notes per alternative (2 per exercise)
- Extended GIF prefetch to cover alternative exercises

## Tasks Pending
- Fill in main workout exercises for Pull routine
- Fill in main workout exercises for Legs routine
