# Execute12 — The 12-Week Execution Program

**Stop overthinking. Start executing.**

A premium Progressive Web App (PWA) for the 12-Week Execution Program — a no-nonsense, decision-free fitness system. Track workouts, calculate nutrition, plan meals, and monitor your 12-week journey — all from your phone's home screen with zero accounts or subscriptions.

[![Live Demo](https://img.shields.io/badge/_Live_Demo-Execute12-FF6B35?style=for-the-badge)](https://execute12.netlify.app)
[![PWA](https://img.shields.io/badge/PWA-Installable-4ECDC4?style=for-the-badge&logo=pwa&logoColor=white)](https://execute12.netlify.app)
[![License](https://img.shields.io/badge/License-MIT-7B68EE?style=for-the-badge)](LICENSE)

---

## Features

### Dashboard
- Weekly workout completion tracker with visual progress cards
- 12-week timeline with color-coded phase indicators
- Streak counter and total workout stats
- Daily calorie and protein targets at a glance

### Workout Tracker
- **4-day Upper/Lower split** — compound and isolation days
- **26 exercises** with custom SVG illustrations showing form and equipment
- **Form tips** for every exercise — tap the 👁️ icon for full-screen guide
- **Set-by-set logging** — weight and reps for every set
- **Built-in rest timer** with auto-countdown
- One-tap workout completion per week

### Nutrition Calculator
- **Calorie calculator** based on weight × goal multiplier
- **Protein formula** — bodyweight in lbs = daily protein grams
- **12 pre-built meal plans** across breakfast, lunch, dinner, and snacks
- **Food logger** with 24 common items — tap to add, adjust quantities
- **Progress bar** tracking daily intake vs. targets
- Category filters: protein, carbs, fats, veggies

### Metric ↔ Imperial Toggle
- One-tap conversion across the entire app
- Weight input auto-converts when switching
- Logged weights display in your preferred unit
- Progression examples adapt to your unit system

### Progress Tracking
- Week selector (1–12) with progress bar
- **4-phase progression map** — Foundation → Build → Overload → Deload
- Weekly completion grid with dot indicators
- Progression example with real numbers

### Program Guide
- Editable profile — name, start date, personal notes
- Core philosophy and non-negotiable rules
- Accordion FAQ section addressing common questions
- Undo support for accidental workout completions

---

## Quick Start

### Install on Your Phone (PWA)

1. Visit the live URL in **Chrome** on your phone
2. Tap the **" Install App"** banner at the bottom
3. Tap **Install** — app appears on your home screen
4. Full-screen, offline-capable, no browser bar

### Run Locally

```bash
git clone https://github.com/jayeshsawarkar/execute12.git
cd execute12
# Open index.html in any browser — that's it, no build step needed
open index.html
```

---

## Tech Stack

| Technology | Purpose |
|-----------|---------|
| **React 18** | UI rendering (via CDN, no build step) |
| **Babel Standalone** | In-browser JSX compilation |
| **Service Worker** | Offline caching and PWA support |
| **Web App Manifest** | Home screen install, splash screen |
| **LocalStorage** | Persistent data — workouts, nutrition, settings |
| **SVG** | Custom exercise illustrations (27 unique drawings) |
| **DM Sans** | Typography via Google Fonts |

**Zero dependencies. No Node.js. No webpack. No npm install.**  
Just 5 files totaling ~76KB. Open `index.html` and go.

---

## Project Structure

```
execute12/
├── index.html      → Full React app (single file, ~76KB)
├── sw.js           → Service worker for offline support
├── manifest.json   → PWA manifest (name, icons, theme)
├── icon-192.svg    → App icon (192×192)
├── icon-512.svg    → App icon (512×512)
└── README.md       → You're reading it
```

---

## The Program

Based on the **Superhuman Lab 12-Week Execution Program** by [@satyajitkumthekar](https://instagram.com/satyajitkumthekar).

### Schedule
| Day | Workout | Focus |
|-----|---------|-------|
| Monday | Upper Body A | Compound (heavy multi-joint) |
| Tuesday | Lower Body A | Compound (heavy multi-joint) |
| Wednesday | REST | Recovery |
| Thursday | Upper Body B | Isolation (targeted muscle) |
| Friday | Lower Body B | Isolation (targeted muscle) |
| Weekend | REST | Recovery |

### Progression Phases
| Weeks | Phase | Strategy |
|-------|-------|----------|
| 1–2 | Foundation | Learn movements, find working weights |
| 3–6 | Build | Push +1–2 reps per week |
| 7–10 | Overload | Increase weight 2.5–5kg at top of range |
| 11–12 | Deload | Reduce 30%, perfect form |

### Nutrition Formula
- **Calories:** Weight (lbs) × multiplier (10–18 based on goal)
- **Protein:** Weight (lbs) × 1 = daily grams
- **Rule:** Buy protein first, do whatever with the rest

---

## Contributing

This is a personal project, but suggestions are welcome! Open an issue or submit a PR.

---

## License

MIT License — free to use, modify, and distribute.

---
