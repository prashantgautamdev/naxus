# NEXUS // Performance Dashboard

A single-file, dark-themed executive productivity dashboard built with **HTML, Tailwind CSS, and Chart.js**. It combines habit tracking, weekly task planning, alarms/reminders, and biometric analytics in one self-contained page — no backend, no build step, just open the HTML file in a browser.

![Status](https://img.shields.io/badge/status-active-14b8a6) ![Type](https://img.shields.io/badge/type-single--file%20HTML-informational) ![License](https://img.shields.io/badge/license-MIT-lightgrey)

## ✨ Features

### 📊 Analytics Overview
- **Daily Execution Volume** — 7-day bar chart of task throughput
- **Macro Goal Completion** — doughnut chart showing overall goal progress
- **Quick Stats Panel** — current streak, consistency index, task resolution rate, focus efficiency

### ⏰ Tactical Alarm & Reminder Hub
- Create named alarms with a specific time trigger
- Toggle alarms on/off, delete with one click
- Time auto-formats to 12-hour AM/PM display

### ✅ Habit Execution Matrix
- 30-day grid to track any habit day-by-day via checkboxes
- Add new habits dynamically with a text input
- Visual "completed vs pending" legend

### 🗓️ Weekly Tactical Planner
- One card per weekday (Mon–Sun) with editable task lists
- Add/remove tasks on the fly (press Enter or click +)
- Circular progress ring + percentage per day, auto-updates as tasks are checked off
- Live task count per day

### 📈 Biometric Recovery Correlation
- Line chart comparing sleep hours vs. performance rating over 7 days

### 🕐 Live Date Engine
- Header auto-displays the current date (e.g. `FRIDAY, JULY 03, 2026`)

## 🛠️ Tech Stack
| Library | Purpose |
|---|---|
| [Tailwind CSS](https://tailwindcss.com/) (CDN) | Layout & utility styling |
| [Chart.js](https://www.chartjs.org/) (CDN) | Bar, doughnut, and line charts |
| [Font Awesome 6.4.0](https://fontawesome.com/) (CDN) | Icons |
| Vanilla JavaScript | All interactivity — no framework, no build tools |

## 🚀 Getting Started

No installation needed — it's a static HTML file.

```bash
git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name>
```

Then just open `nexus.html` (or `index.html`) directly in your browser, or serve it locally:

```bash
python3 -m http.server 8000
# visit http://localhost:8000
```

### Deploy for free with GitHub Pages
1. Push this repo to GitHub
2. Go to **Settings → Pages**
3. Source: `Deploy from branch`, branch: `main`, folder: `/ (root)`
4. Your live dashboard will be available at:
   `https://<your-username>.github.io/<repo-name>/`

> 💡 Tip: rename `nexus.html` to `index.html` so the Pages link opens the dashboard directly at the root URL.

## ⚠️ Known Limitations
- **No data persistence** — added habits, tasks, and alarms reset on page reload (all state lives in memory / the DOM, nothing is saved to `localStorage` or a backend)
- Chart data (bar, doughnut, line) is currently **static/hardcoded** as sample data, not connected to real metrics
- Single-user, client-side only — not designed for multi-device sync

## 🗺️ Possible Improvements
- Persist habits/tasks/alarms using `localStorage` or a backend + database
- Wire up the analytics charts to real, dynamic data instead of hardcoded sample values
- Add actual browser notifications for alarms (currently visual-only, no real triggers)
- Add data export/import (JSON/CSV)
- Mobile-responsive refinements for the 30-day habit matrix (currently wide and scrolls horizontally)

## 📄 License
MIT — free to use, modify, and distribute.
"# naxus" 
