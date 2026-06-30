# Trials

Automated Trials combat. Cypher holds the fight for you — attacking, weaving skills, blocking, managing stamina, and handling stage transitions — round after round, so you can farm Trials AFK.

---

## Quick start

1. Open the **Trials Macro** tab.
2. Click **Pick Window** and select your game window.
3. Set your **Stamina (%)** target and tune the drain/block timings if you want.
4. Flip on the features you use (talents, auto block, zone, etc.).
5. Press **Start Trials**. Press **Stop Trials** (or **F6**) to end.

---

## Combat settings

- **Stamina (%)** — the macro keeps your stamina at or above this level (choose 20%–100%). When stamina drops below it, the macro stops attacking and waits for it to recover before continuing.
- **Drain M1 Hold (s)** — how long it holds the basic attack during the stamina‑drain phase.
- **Drain Block Hold (s)** — how long it holds block during the drain phase.
- **Block Interval (s)** — how often it blocks.
- **Block Hold (s)** — how long each block is held.

---

## Features

Toggle the ones that match your build and the content:

- **M2 (Unbreakable Talent)** — use your M2/unbreakable in the rotation.
- **Advanced Brawl** — adds extra moves to the rotation.
- **Glutton (Talent)** — allows more food uses per slot (for the Glutton talent).
- **Stage Info** — track and report stage progress.
- **Ignore Food** — don't bother with food handling during Trials.
- **Auto Block** — automatically block on a timer during fights.
- **NPC Tracking** — track and aim at the target so attacks connect.
- **Use Zone** — automatically activate your Zone once per round and wait out the cutscene.

> **Combat alerts are intentionally ignored during Trials.** Because Trials *is* combat, the macro won't auto‑stop or auto‑leave on combat detection — otherwise it could never run.

---

## What it handles for you

- **Round detection** — recognises when a stage clears and the next round begins, and keeps going.
- **Skill weaving** — cycles your skills with their cooldowns instead of just spamming one button.
- **Stamina control** — rests when low, resumes when recovered (your target above).
- **Zone usage** — fires your Zone and waits for the cutscene if **Use Zone** is on.
- **Anti‑stuck** — if a round runs unusually long, it forces a stamina‑drain sequence to push past whatever it's stuck on.
- **Webhook progress** — can post your stage‑clear count to Discord as you go.

---

## Tips

- Set **Stamina (%)** to match how aggressive you want to be — higher means it rests more often but never gasses out; lower means more uptime but riskier.
- Turn on **NPC Tracking** if your hits are missing the target.
- Use **Auto Block** for content that punishes you between hits.

**Emergency stop:** **F6**.
