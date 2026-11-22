<div align="center">

# 🧱 BRICKDAY
### BUILD YOUR DAYS. EARN YOUR XP. CLAIM YOUR LIFE.

**A tiny productivity RPG for people who are tired of treating their goals like chores.**

[![Made with](https://img.shields.io/badge/BUILT_WITH-HTML%20%2B%20CSS%20%2B%20REACT-1F2340?style=for-the-badge)](#-under-the-hood)
[![Storage](https://img.shields.io/badge/DATA-LOCAL%20%7C%20YOUR%20BROWSER-A8A4FF?style=for-the-badge)](#-your-data-your-device)
[![Vibe](https://img.shields.io/badge/VIBE-PLAYFUL%20PRODUCTIVITY-F7D257?style=for-the-badge)](#-the-brickday-philosophy)

<br/>

### `ONE TASK AT A TIME. ONE BRICK AT A TIME.`

</div>

---

## ⚡ WHAT IS BRICKDAY?

You know the loop.

You make a plan. You write a to-do list. You stare at it. You move things to tomorrow. Tomorrow becomes next week. And suddenly, the list is more intimidating than the work itself.

**Brickday turns that loop into a game.**

Every task is a mission. Every completed mission earns XP. Every XP point gets you closer to a level-up—or to a reward you actually want.

You don't just check boxes. **You build progress.**

Brickday is a lightweight, browser-based productivity RPG built around one simple idea:

> Make the work feel rewarding. Make the reward worth working for.

---

## 🎮 THE GAME LOOP

```text
       PICK A TASK
            │
            ▼
      CHOOSE ITS DIFFICULTY
            │
            ▼
       GET THE WORK DONE
            │
            ▼
         EARN XP
            │
            ▼
      LEVEL UP OR SAVE IT
            │
            ▼
       REDEEM A REWARD
            │
            └──────────► REPEAT.
```

No complicated productivity system. No overwhelming dashboard. Just a clean loop that makes showing up feel good.

---

## 🧩 THREE SPACES. ONE PROGRESSION SYSTEM.

### 01 — ⚔️ TASKS: YOUR DAILY MISSIONS

Turn the things you need to do into missions.

- **Create tasks** with a title and optional description.
- **Set difficulty** to Easy, Medium, or Hard.
- **Earn XP** based on the difficulty you choose.
- **Repeat tasks** daily or weekly.
- **Edit or delete** tasks whenever plans change.
- Switch between **Pending** and **Completed** tasks.
- Accidentally completed something? Use the **10-second Undo** window to reverse the XP award, provided that XP has not already been spent.

| Difficulty | XP earned | |
|:---|---:|:---|
| 🟢 Easy | **10 XP** | Small wins count. |
| 🟡 Medium | **15 XP** | A solid chunk of progress. |
| 🔴 Hard | **20 XP** | Big effort. Bigger payout. |

**The rule:** complete the task, collect the XP. A task awards XP only once per completion.

### 02 — 🎁 REWARDS: GIVE YOUR XP A PURPOSE

What are you working toward?

Create rewards that make sense to you. Maybe it's a movie night, a new game, a meal outside, or an entire day off.

- Add a reward and set its XP price.
- Edit or remove rewards whenever you want.
- Redeem a reward when your balance is high enough.
- Your XP balance updates immediately after redemption.
- Your redeemed rewards appear in your Profile history.

**Your rewards. Your prices. Your rules.**

A reward isn't just something you buy with XP. It's something you deliberately make time to earn.

### 03 — 📊 PROFILE: SEE THE PROGRESS

Your Profile keeps the important numbers in one place.

- **Current level** — your progression rank.
- **XP progress bar** — how far you are from the next level.
- **Total XP earned** — lifetime XP earned from completed tasks.
- **Tasks completed** — your total completion count.
- **Current streak** — consecutive days with recorded task activity.
- **Redeemed rewards** — a history of your latest eight redemptions.

Your level is based on lifetime XP earned—not your spendable balance. Spending XP on rewards doesn't erase your progress.

---

## 🏆 THE LEVEL SYSTEM

Every level takes more lifetime XP than the last. The climb gets steeper as you progress.

The XP required to reach the start of level `L` is:

```js
XP required = 25 × L × (L - 1)
```

| Level | Lifetime XP required to reach it |
|---:|---:|
| 1 | 0 XP |
| 2 | 50 XP |
| 3 | 150 XP |
| 4 | 300 XP |
| 5 | 500 XP |
| 6 | 750 XP |
| 7 | 1,050 XP |

Your progress bar shows how much XP you've earned inside your current level and how much remains until the next one.

**There is no final level. Keep building.**

---

## 🔥 THE XP ECONOMY

Brickday separates what you've **earned** from what you can **spend**.

```text
AVAILABLE XP = TOTAL XP EARNED − TOTAL XP SPENT
```

Example:

```text
Lifetime XP earned       250 XP
XP spent on rewards       80 XP
                         ──────
Available balance        170 XP
```

- Completing tasks increases lifetime XP and your available balance.
- Redeeming rewards decreases your available balance.
- Your level is calculated from lifetime XP earned.
- Deleting a completed task does **not** remove the XP already earned.
- Deleting a reward does **not** refund XP spent on an earlier redemption.

This keeps your progression separate from your reward spending.

---

## 🗓️ STREAKS & REPEATING TASKS

Consistency is built one day at a time.

- Your streak counts consecutive calendar days with recorded task completions.
- If you haven't completed anything today, a streak from yesterday can remain alive.
- Daily tasks become available again on the next day.
- Weekly tasks reset at the start of a new week (Sunday-based).
- Completing a recurring task in a new period can earn XP again.

A streak is a signal of consistency—not a reason to punish yourself. Miss a day, return to the work, and keep building.

---

## 🎨 THE LOOK

Brickday uses a playful, tactile visual language:

- A soft blue wave-pattern background.
- Bold, high-contrast typography.
- Purple XP badges and navigation states.
- Yellow, mint, and coral accents.
- Solid borders and offset shadows that make buttons and cards feel almost physical.
- Difficulty-coloured task cards.
- Responsive layouts for smaller screens.
- Reduced-motion support for people who prefer less animation.

The design is meant to feel less like a corporate task manager and more like **your own little productivity arcade**.

---

## 🚀 RUN IT LOCALLY

Brickday is a single-page app contained in one HTML file.

### 1. Get the project

Download or clone the repository, then locate:

```text
Brickday.html
```

### 2. Open it

The simplest option:

1. Double-click `Brickday.html`.
2. Open it in a modern browser.
3. Start adding tasks and rewards.

You can also serve the file through a local development server if you prefer.

### 3. Start building

- Add your first task.
- Choose its difficulty.
- Complete it.
- Collect your XP.
- Add a reward worth saving for.

That's it. You're in.

---

## 🛠️ UNDER THE HOOD

Brickday keeps its implementation deliberately lightweight.

| Layer | Technology |
|:---|:---|
| Structure | HTML5 |
| Styling | CSS3 |
| UI | React 18 |
| JSX-like templating | HTM |
| State | React Hooks |
| Persistence | Browser `localStorage` |
| Navigation | URL hash routes |
| Typography | Bricolage Grotesque (Google Fonts) |

### No build step required

The current app loads React, ReactDOM, and HTM from CDNs. There is no package installation or compilation step required to run the standalone HTML file.

### Data storage

The app stores its state in browser `localStorage` under:

```text
brickday:v1
```

Your tasks, rewards, XP totals, activity data, and redemption history are saved in the browser you're using.

**Important:** this is local browser storage—not a cloud account or database. Your data does not automatically sync across browsers or devices. Clearing the browser's site data may erase your Brickday progress, so keep that in mind before clearing storage.

---

## 🧭 PROJECT STRUCTURE

The project is currently intentionally simple:

```text
Brickday/
└── Brickday.html
    ├── HTML document
    ├── CSS design system
    ├── XP and progression logic
    ├── Task management
    ├── Reward management
    ├── Profile and statistics
    └── React application
```

Everything lives in one file, making the project easy to carry, open, inspect, and experiment with.

---

## 🧠 THE BRICKDAY PHILOSOPHY

Productivity apps often make you manage productivity.

Brickday wants you to spend less time managing the system and more time doing the actual work.

Don't wait for motivation to magically appear. Don't make a perfect plan that you never execute. Don't underestimate the small tasks that move a bigger project forward.

Complete the assignment. Solve the problem. Write the page. Ship the feature. Take the XP.

Then do it again tomorrow.

**You don't build a great day all at once. You build it one brick at a time.**

<div align="center">

# 🧱 BUILD YOUR BRICKDAY.

### SHOW UP. DO THE WORK. EARN THE REWARD.

<sub>Made for the long game. ✦</sub>

</div>

---

## 📌 NOTES & LIMITATIONS

- Brickday currently has no sign-in, cloud sync, or multi-device account system.
- Progress is stored locally in the browser through `localStorage`.
- XP values and level thresholds are defined in the app's JavaScript.
- The app depends on its external CDN resources and Google Fonts for the intended runtime and typography.
- The current implementation is a standalone personal productivity tool; it does not include a backend or shared leaderboard.
