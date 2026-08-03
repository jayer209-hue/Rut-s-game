# Life HQ — Personal Dashboard

A single-file personal dashboard that organizes everything across **Fitness**, **Finance**,
**Rutledge**, and **Other** (all renamable). One `dashboard.html` file — no install, no server,
no accounts. Works offline; all data is saved privately in the browser.

Built to be **iterated on with Claude**: use it for a week, and when you want it to work
differently, just ask Claude to change it.

## What's inside

| Tab | What it does |
|-----|--------------|
| 🏠 **Today** | One command center — today's tasks, habit check-ins, goal progress, and a snapshot of every area of life |
| 🎯 **Goals** | Big outcomes with a number to move (e.g. "Emergency fund → $10,000"). Log progress, watch the bar fill |
| ✅ **Tasks** | Today / This week / Later, tagged by area, with priority, due dates, and per-area filtering |
| 🔥 **Habits** | Daily check-ins with streak counters and a 7-day dot strip |
| 📈 **Track** | Log any number over time (weight, spend, savings, miles, mood) with a live trend sparkline |
| ✨ **Iterate** | The feedback loop — a copy-paste prompt and ideas for evolving the app with Claude |

Plus a top-right **📝 Weekly Review** (wins / challenges / next-week focus + a rating per area) —
that's the reflection loop that makes each week better — and **⚙️ Settings** to rename the
areas of life and back up data.

## How to use it

1. Open `dashboard.html` in any browser (double-click it, or drag it into a browser tab).
2. Add real goals, tasks, habits, and trackers.
3. It saves automatically. Everything stays on that device, in that browser.

> **Backup note:** data lives in the browser's localStorage (key `lifehq_v1`). Before switching
> devices or replacing the file, use **Iterate → Export backup** (or ⚙️ Settings → Export).
> Import the JSON on the other side to bring everything over.

## Porting it into your Claude account (the iteration loop)

This is the fun part — the dashboard is meant to grow around how *you* actually work.

1. In [claude.ai](https://claude.ai), create a **Project** (or just start a chat) and attach /
   paste `dashboard.html`.
2. Use the starter prompt (it's built into the **✨ Iterate** tab — tap **Copy**):

   > I have a single-file personal dashboard called "Life HQ" (one `dashboard.html` file —
   > vanilla HTML/CSS/JS, data saved in localStorage). I'm attaching the file. Please act as my
   > product engineer for it. Keep it as ONE self-contained file with no external dependencies,
   > preserve my data model and the localStorage key `lifehq_v1`, and make this change: **_your
   > idea here_**. Return the complete updated `dashboard.html`.

3. Claude returns a new `dashboard.html`. **Save over the old one.** Your data survives because
   it's stored in the browser, not the file.
4. Repeat whenever you want something new.

### Things you could ask Claude to add

- 🍽️ A meal & grocery planner that builds a shopping list
- 💵 A monthly budget with per-category targets vs. actual spend
- 🏋️ A workout logger (sets, reps, weekly training plan)
- 🏡 Rename "Rutledge" to Home / Family / a business and add a project board
- 🔔 Recurring tasks that come back every week
- 🎨 A lighter theme, different colors, a new name and logo

## Files

- **`dashboard.html`** — the whole app. This is the only file to share, open, or hand to Claude.
- **`DASHBOARD.md`** — this guide.
