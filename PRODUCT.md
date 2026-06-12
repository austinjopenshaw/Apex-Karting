# Apex — Kart Racing Companion

A mobile app (iOS + Android) for grassroots / club kart racers to **time their
laps, log their sessions, dial in kart setup, and watch themselves get faster.**

Designed around the real-world use case: a parent and child who race together
and want everything for the whole family under one account.

---

## The opportunity

Searching the App Store turns up essentially **one** competitor in this niche,
and it gets poor reviews. The recurring complaints in apps like this are almost
always the same:

- Clunky, fiddly data entry at the track (where you're wearing gloves, it's
  loud, and you have 90 seconds between runs)
- Ugly / dated UI
- Crashes and lost data
- Everything locked behind an aggressive paywall
- A lap timer that's *just* a stopwatch — no insight, no memory, no progress

That's the wedge. **A clean, fast, beautiful tool that turns lap times into
progress** is a genuinely open lane.

---

## Who it's for

| Persona | Needs |
|---|---|
| **The racing parent** (primary) | Manage their own racing *and* their kid's from one account. Quick logging, see if the kid is improving, remember what setup worked. |
| **The young driver** | A simple, motivating view of "am I getting faster?" Big lap timer, personal bests, streaks. |
| **The serious club racer** | Setup notebook tied to results, consistency stats, track-by-track records. |

Multi-driver, one account is a core design decision — not an afterthought.

---

## MVP — the 5 core features

The goal of an MVP is to ship the *smallest* thing that's genuinely useful and
clearly better than the competitor. Everything here earns its place; anything
that doesn't is parked in "Later" below.

### 1. ⏱️ Lap Timer (the hero)
The thing people open the app for. Must be **dead simple to operate trackside.**
- Huge, glanceable current-lap display
- One giant "+ Lap" button, thumb-reachable so it's easy to tap trackside
- Live delta vs. your best lap (green = faster, red = slower) so you get instant
  feedback lap to lap
- Last / Best / Lap-count always visible
- Saves the whole run as a session when you finish — **never lose data**

### 2. 📋 Session Log
Every time on track becomes a saved record.
- Track, date, kart, weather + track temp, wet/dry
- Full lap-by-lap times, best & average
- A few quick driver notes + tags ("#braking", "#newPB")
- Browsable history grouped by week

### 3. 🔧 Garage (karts & setups)
Where the "what worked" lives — the competitor's apps largely ignore this.
- Add karts (chassis, engine/class)
- Save setup sheets: tire pressures, gearing, axle, carb, seat, notes
- Setup is attached to each session, so you can answer *"what did we run the day
  he set his PB?"* in one tap

### 4. 📈 Insights
Turns raw times into motivation and direction.
- Best-lap trend over time (the "I'm getting faster" chart)
- Personal best per track
- Consistency score (how tight your lap spread is — race pace, not just one hot lap)

### 5. 👥 Multi-driver account
- Switch between drivers (Dad / kid / more) instantly from any screen
- Each driver has their own karts, sessions, PBs, and stats
- One login for the whole family

---

## Deliberately *not* in the MVP (the "Later" list)

Parked on purpose to keep v1 focused and shippable:

- Social feed / friends / public leaderboards
- Live multi-driver session sharing & spectating
- GPS auto-lap (cross the start/finish line, it logs automatically — no tapping)
- Video sync (overlay lap times on GoPro footage)
- Full GPS telemetry: sector times, speed traces, track maps
- Coaching marketplace / share setups with other racers
- Maintenance & cost tracking (engine hours, tire life, spend)
- Race-day / event mode (heats, grids, championship points)
- Apple Watch / wearable companion
- Offline-first sync across devices

Several of these (video, telemetry, event mode, watch app) are strong
**premium / paid** candidates once the free core has traction.

---

## Why this beats the incumbent

| Pain in existing app | Apex's answer |
|---|---|
| Fiddly trackside entry | One huge, thumb-reachable lap button |
| "Just a stopwatch" | Live delta, PBs, trend, consistency |
| Ugly / dated | Clean dark "performance tool" design |
| Forgets your setup | Garage with setups tied to every session |
| One driver only | Multi-driver family account |
| Lost data / crashes | Auto-save every session |

---

## Suggested business model

- **Free**: lap timer, session log, garage, basic insights (the whole MVP)
- **Apex Pro** (subscription): GPS telemetry & sector times, video overlay,
  event/championship mode, watch app, cloud backup across devices

Free core builds the habit and word-of-mouth; the data-rich features are what
serious racers happily pay for.

---

## About this prototype

`index.html` is a **fully interactive, phone-viewable mockup** — not the real
app, but a clickable demonstration of the design and core flows:

- Tap through all 5 sections via the bottom nav
- The **lap timer actually works** — hit Start, tap "+ Lap", watch the live delta
- **Switch drivers** (top-right avatar → Mike / Tyler) and watch all the data,
  karts, and stats change
- Open any session to see lap-by-lap times, the setup used, and notes

It's a single self-contained HTML file (no install, no build step) so it opens
instantly on any phone. Built to show your buddy the *vision and feel* before
anyone writes a line of real app code.
