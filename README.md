# focus

An app for helping focus and managing your day.

Plan what you have to do today, say how long you think each task takes, run a
timer on one task at a time, and keep a record of where your hours actually go.

One file, no build step, no server, no account: open `index.html` in a browser.

## Features

- **Today's plan** — add a task with an estimate (one click for 15m/30m/45m/1h/1.5h/2h, or type your own).
- **One timer at a time** — a ring shows how much of the estimate you've used; it turns red past the estimate, and alerts you with a sound and an optional desktop notification when time is up.
- **Full-screen focus** — just the clock, nothing else (`F`).
- **Close it whenever** — everything is saved locally. If a timer was running when you closed the app, it asks on reopen whether that away time counts.
- **History** — per-day records plus a 7-day chart of focused vs. planned time, and an estimate-accuracy ratio ("tasks take 17% longer than planned").
- **Carry over** — move unfinished tasks from earlier days into today.
- **Dark mode**, following the system setting with a manual override.
- **Backup** — export/import all data as JSON.

### Keyboard shortcuts

| Key | Action |
|---|---|
| `N` | New task |
| `Space` | Start / pause |
| `F` | Full-screen focus |
| `Esc` | Exit full screen |

## Where the data lives

In the browser's `localStorage`, under the key `focus-app-v1` — on your machine
only, never sent anywhere. It is tied to the browser *and* to the file's
location, so keep `index.html` in a stable path and use the same browser. Clearing
site data, or using a private window, loses the history — **Export** from the `⋯`
menu now and then for a backup.
