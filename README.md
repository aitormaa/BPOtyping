# BPO Typing Test - Back Market

A custom typing speed test built for BPO training teams. Tracks WPM, accuracy, scores and grades across teams and levels -- all in a single HTML file backed by Firebase.

---

## Live URLs

| Who | URL |
|---|---|
| Learners | https://aitormaa.github.io/BPOtyping |
| Admin panel | https://aitormaa.github.io/BPOtyping/?admin=backmarket2026 |

---

## Tech stack

| Layer | Tech |
|---|---|
| Frontend | Vanilla HTML + CSS + JavaScript (single file, no framework) |
| Database | Firebase Firestore (NoSQL, real-time) |
| Hosting | GitHub Pages (free, unlimited bandwidth) |
| Auth | Email-based identity (no password, unique per Back Market email) |

No build step, no dependencies, no npm. Open the file in a browser and it works.

---

## Features

### For learners
- Sign in with Back Market email (one account per email, no duplicates)
- Select team at sign-in
- Two levels: Beginner and Intermediate
- Real-time WPM, accuracy, score and grade (A to F)
- Auto-saves result the moment the test ends
- Results saved locally if offline, synced on next login
- Badges and streak system
- Personal WPM progress chart
- Live race mode (compete in real time)

### For admins
- Tests -- create, edit, toggle, feature, move between levels
- Results -- filter by team, download CSV
- Learners -- assign teams, view email
- Leaderboard -- filter by team, download CSV, auto-excludes abandoned tests
- Races -- create race rooms with a shareable code
- Teams -- create teams with custom colors (appear in learner sign-in)

### Tracking
- Done -- test completed normally
- Quit -- learner exited before finishing (tracked silently, visible in Results)

---

## Grading system

Score = WPM x (Accuracy / 100)

| Grade | Beginner | Intermediate |
|---|---|---|
| A | >= 50 | >= 58 |
| B | >= 42 | >= 49 |
| C | >= 35 | >= 42 |
| D | >= 28 | >= 36 |
| F | < 28 | < 36 |

---

## How to update and redeploy

1. Download the latest index.html from this repo
2. Make your changes
3. Go to the file in GitHub, click the pencil icon, paste the new content, click Commit changes

The live site updates in about 1 minute automatically.

---

## Firebase project

- Project: bm-typing-test
- Console: https://console.firebase.google.com
- Collections: tests, results, learners, teams, races, settings

---

## Built by

Aitor Martin - Back Market CX Training and Instructional Design
