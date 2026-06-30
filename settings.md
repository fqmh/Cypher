# Settings Reference

Everything Cypher does can be tuned on the **Settings** tab. Change what you need, then click **Save Settings** (you'll see a "✓ Saved" note). Settings are remembered between launches.

This page lists every option, grouped exactly as they appear on screen.

---

## Important Configuration

| Setting | What it does | Default |
|---------|--------------|---------|
| **Webhook URL** | Discord webhook for alerts. | empty |
| **Discord Mention ID** | Your user/role ID so alerts can ping you. | empty |
| **Delete messages after** | Auto‑delete alert messages after a time, or **Keep Pings**. | Keep Pings |
| **Detect By** | Find the game by **Window Title** or **Executable**. | Window Title |
| **Window Title** | Title to match when detecting by title. | `Roblox` |
| **Exe Name** | Executable to match when detecting by exe. | `RobloxPlayerBeta.exe` |
| **Assets Path** | Folder of reference images & item icons. **Browse** to pick it. | `assets/` |
| **Min Interval (s)** | Shortest wait between detection scans. | 1.0 |
| **Max Interval (s)** | Longest wait between detection scans. | 2.0 |
| **Confidence** | Match strength required for a detection (0–1). Higher = stricter. | 0.85 |
| **Anti‑AFK Key** | Key tapped to prevent idle kicks. | Space |

---

## Detections

Switch on the events you want Cypher to watch for. All are **off by default**. Full meanings are on the [Monitor & Detections](monitor.md) page.

**Combat · Disconnect · Training · Protein Maintain · Merchant · Rift · Raid Base · Boss Spawn · Yakuza Raid Cooldown · S.W.A.T Raid Cooldown · Setsuna Boss Cooldown · Turf**

---

## System & Advanced

**System toggles**

| Setting | What it does | Default |
|---------|--------------|---------|
| **Debug Mode** | Extra detailed logging. | Off |
| **F8 Medal Clip** | Allow triggering Medal.tv clips with F8. | Off |
| **Combat Screenshot** | Capture the screen when combat is detected. | Off |
| **Anti‑AFK** | Send a key on a timer to avoid idle kicks. | Off |
| **Auto Return Focus** | Restore your previous window after an anti‑AFK tap. | Off |
| **Test Anti‑AFK** | Button — fire a test key to all game windows now. | — |

**Leave settings**

| Setting | What it does | Default |
|---------|--------------|---------|
| **Leave game after Combat** | Auto‑leave when combat is detected. | Off |
| **Leave Mode** | **Normal** (wait for combat to end) or **Instant**. | Normal |
| **Combat Evasion** | Try to dodge/survive instead of leaving. | Off |
| **Leave on Raid Base** | Also leave when a raid base appears. | Off |
| **Monitor Off After Leave** | Stop the Monitor after leaving an account. | Off |
| **Shutdown PC on Alert** | Shut the PC down after an alert/leave. | Off |
| **Auto‑Return Macroing** | Auto‑rejoin after disconnect / training stop. | Off |
| **Auto‑Wear** | Re‑equip gear when training resumes. | Off |

**FPS Cap settings**

| Setting | What it does | Default |
|---------|--------------|---------|
| **FPS Cap** | Limit Roblox frame rate. | Off |
| **FPS Value** | The cap to apply. | 30 |
| **Uncap Focused** | Remove the cap on the window you're looking at. | Off |

---

## Periodic Stat Check

| Setting | What it does | Default |
|---------|--------------|---------|
| **Enable** | Press a key on a schedule (e.g. to open stats). | Off |
| **Key** | Which key to press (1–7, R, T, Y). | — |
| **Interval (mins)** | How often to press it. | — |

---

## Periodic Screenshot

| Setting | What it does | Default |
|---------|--------------|---------|
| **Enable** | Save a screenshot on a schedule. | Off |
| **Interval (mins)** | How often. | — |

---

## Game Overlay

| Setting | What it does | Default |
|---------|--------------|---------|
| **Enable Overlay** | Show the on‑screen HUD. | On |
| **Lock Position (Click‑through)** | Lock it and let clicks pass through. | On |
| **Show Setsuna** | Show the Setsuna cooldown. | On |
| **Show Yakuza (Raid 1)** | Show the Yakuza raid cooldown. | On |
| **Show SWAT (Raid 2)** | Show the S.W.A.T raid cooldown. | On |
| **Test Overlay HUD** | Button — preview the overlay. | — |

---

## Saving

Click **Save Settings** to write your changes. Detection toggles, intervals, webhook, and feature switches all take effect from then on. A few advanced timing values for auto‑return live in your `config.json` if you ever need to fine‑tune them, but the defaults are sensible for almost everyone.
