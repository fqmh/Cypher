# Monitor & Detections

The **Monitor** is Cypher's watchtower. Press **Start** and it continuously scans every game window you have open, recognises what's happening on screen, and reacts — sending Discord alerts and (optionally) taking automatic actions like leaving the game or rejoining.

It's perfect for **AFK farming across multiple accounts**: leave them running, walk away, and let Cypher tell you (and handle it) when something needs attention.

---

## Using the Monitor screen

- **Start / Stop** — begins or ends watching. While running, the status reads "Monitoring".
- **Reset** — sets the on‑screen counters back to zero.
- **Counters** — three at‑a‑glance tallies: **Disconnects**, **Training**, and **Combat**.
- **Activity Log** — a live, colour‑coded feed of everything Cypher sees and does. Use **Clear** to wipe it.

> The Monitor and your macros can run at the same time. Many users start the Monitor first, then launch a grind macro.

---

## How detection works

Cypher reads each game window with computer vision:

- **Text events** (disconnect, training, raids, turf, merchant, rift, boss spawn, setsuna) are read with **Windows OCR** — it literally reads the words on screen, so it keeps working across resolutions.
- **Visual events** (combat, protein/hunger) are recognised by **image matching** against reference pictures.

A detection only counts when Cypher is confident enough. That bar is the **Confidence** setting (default **0.85**, i.e. 85%). Raise it to reduce false alarms; lower it if real events are being missed.

How often Cypher scans is set by **Min Interval** and **Max Interval** (seconds) — it waits a random time in that range between scans, which is gentler on your CPU.

---

## What Cypher can detect

Turn each of these on or off under **Settings → Detections**. (They're all **off by default** — enable the ones you care about.)

| Detection | What it means in‑game |
|-----------|------------------------|
| **Combat** | Your character has entered combat / is being attacked. |
| **Disconnect** | The account got disconnected / kicked. |
| **Training** | The account is actively training (used to track AFK grinds). |
| **Protein Maintain** | A hunger/protein indicator — your character needs food. |
| **Merchant** | A merchant has appeared. |
| **Rift** | A rift event is active. |
| **Raid Base** | A raid encounter has started. |
| **Boss Spawn** | A boss has spawned. |
| **Yakuza Raid Cooldown** | Yakuza raid availability (Raid 1). |
| **S.W.A.T Raid Cooldown** | S.W.A.T raid availability (Raid 2). |
| **Setsuna Boss Cooldown** | Setsuna boss availability. |
| **Turf** | A turf war / territory event is active. |

When any enabled event first appears, Cypher logs it, updates the relevant counter, and (if a webhook is set) sends a Discord alert.

---

## Automatic actions

Detections become powerful when you let Cypher act on them. These are all configured in **Settings**; here's what they do.

### Auto‑Leave (on combat)
If **Leave game after Combat** is on, Cypher will pull the account out of the game when it's attacked — great for protecting AFK alts.

- **Leave Mode → Instant** — leaves the moment combat is detected.
- **Leave Mode → Normal** — waits for combat to actually finish, then leaves.
- **Combat Evasion** — instead of (or before) leaving, makes the character dodge around to try to survive.
- **Leave on Raid Base** — also leave when a raid base is detected.

### After leaving
- **Monitor Off After Leave** — stop the Monitor once it has pulled an account out (so it doesn't keep reacting).
- **Shutdown PC on Alert** — for the truly AFK: shut the computer down after an alert/leave.

### Auto‑Return (auto‑rejoin)
With **Auto‑Return Macroing** enabled, Cypher detects when an account **disconnected** or **stopped training**, waits for things to settle, and **rejoins the game automatically** via a Roblox deep link. It can even server‑hop to a lower‑population server. There's a cooldown between attempts, and a give‑up timeout so it doesn't retry forever.

### Auto‑Wear
**Auto‑Wear** re‑equips your training gear when training resumes after a disruption, so you don't come back to an un‑equipped character.

> See the [Settings Reference](settings.md) for every related option and the [Quality‑of‑Life Features](features.md) page for how these fit together.

---

## Tips

- Start with just **Disconnect** and **Combat** enabled until you trust the setup, then add more.
- Set a **Webhook URL** (and your **Mention ID**) so you actually get pinged. See [Getting Started](getting-started.md#6-recommended-connect-discord).
- If you're getting false alerts, nudge **Confidence** up a little. If you're missing events, nudge it down.

Next: pick a grind from the **Macros** section, starting with **[Durability »](macros/durability.md)**.
