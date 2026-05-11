# GRIND — Gym Tracker

A lightweight, mobile-first gym tracking app built as a single HTML file. No frameworks, no dependencies, no server — just open it in a browser and start logging.

## Features

- **Exercise search** — type a few letters to filter from 70+ built-in exercises across arms, legs, core, and CrossFit
- **Auto-fill from last session** — weight, reps, and sets are pre-populated from your previous log for that exercise
- **Large touch targets** — designed for sweaty hands and gloves; all buttons are 66px+
- **Volume tracking** — computes reps × sets × weight live as you adjust
- **1RM logging** — optional max weight field per session to track personal records
- **PR badge** — history cards are flagged when a session matches your all-time max for that exercise
- **Full history** — sessions grouped by week (This Week / Last Week / date ranges), scrolling back indefinitely
- **Add custom exercises** — any name not in the built-in list can be saved permanently
- **Settings** — toggle lbs/kg, choose weight step (2.5 / 5 / 10), clear history

## Usage

Open `grind-gym-tracker.html` in any modern browser. No build step, no install.

**Recommended for mobile:** In Safari or Chrome, use *Add to Home Screen* to install it as a standalone app icon.

## Data storage

All data is saved to `localStorage` in the browser — nothing leaves your device. Three keys are used:

| Key | Contents |
|-----|----------|
| `gt_sess` | Array of logged sessions |
| `gt_lu` | Last-used values per exercise (for auto-fill) |
| `gt_ex` | Exercise list (built-ins + any custom additions) |
| `gt_cfg` | Settings (unit, weight step) |

## Exercise categories

| Category | Examples |
|----------|---------|
| Arms / Upper Body | Chest Press Machine, Lat Pulldown, Bicep Curl Machine, Tricep Pushdown, Shoulder Press Machine |
| Legs / Lower Body | Leg Press, Leg Extension, Leg Curl, Hip Abductor, Hack Squat, Romanian Deadlift |
| Core | Ab Crunch Machine, Cable Crunch, Rotary Torso, Hanging Leg Raise, Pallof Press |
| CrossFit / Free Weights | Wall Balls, Kettlebell Swing, Deadlift, Thruster, Power Clean, Double Unders |

## Tech stack

- Vanilla HTML, CSS, JavaScript — no build tools or dependencies
- Google Fonts: [Barlow Condensed](https://fonts.google.com/specimen/Barlow+Condensed), [Barlow](https://fonts.google.com/specimen/Barlow), [Share Tech Mono](https://fonts.google.com/specimen/Share+Tech+Mono)
- Browser `localStorage` for persistence

## Screenshot

> Dark industrial aesthetic — near-black background, orange accent, monospace number readouts, glove-friendly tap targets.

## License

MIT
