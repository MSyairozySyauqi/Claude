# Stride: running schedule tracker

A small website for planning and logging your runs. Plain HTML, CSS and JavaScript: there is no build step and no server. Your data stays in your browser's `localStorage`.

## Features

- **Week planner**: Monday–Sunday view of every planned run. Move between weeks with the arrows, or the ← / → keys.
- **Run types**: easy, long, tempo, intervals, recovery and race.
- **Log results**: tick a run's checkbox to mark it done, or open it to record actual distance, duration and notes. Pace is calculated for you.
- **Repeat weekly**: schedule a run for 2–16 weeks in one go.
- **Weekly summary**: distance done vs planned, runs completed, time on feet and average pace.
- **Weekly distance chart**: the last 8 weeks, with hover details and a table view.
- **Coming up**: your next planned runs.
- **km or miles**: switch at any time. Distances are stored in km and converted for display.
- **Export / Import**: back up your runs to a JSON file, or move them to another browser.
- Light and dark mode follow your system setting. Works on phones.

Keyboard shortcuts: `N` new run, `T` jump to this week, `←` / `→` change week.

## Running it

Open `index.html` in a browser. To serve it locally:

```sh
python3 -m http.server 8000
# then visit http://localhost:8000
```

To host it for free, enable **GitHub Pages** for this repository (Settings → Pages → deploy from branch, root folder).

## Data

Runs are saved under the `stride.runs.v1` key in `localStorage`, so they are tied to one browser on one device. Use **Export** now and then for a backup.
