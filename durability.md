# Durability Training

Automated durability training using a "body condition" item and one or more alt accounts. One account takes the hits (the **victim**), another deals them (the **attacker**), and Cypher manages the whole loop — buying the item, equipping it, hitting, watching HP, eating food, and handling stamina — until the victim reaches your target HP.

---

## Quick start

1. Open the **Durability Macro** tab.
2. Choose a **Mode** (see below).
3. For each account card shown, click **Pick Window** and select that account's game window.
4. Use the **Dura** and **Strike** buttons to point Cypher at the right on‑screen spots for that account (where shown).
5. Set your **HP Target**, **Attack Delay**, and any toggles.
6. Press **Start Training**. Press it again (or **F6**) to stop.

---

## Modes

Pick the mode that matches how many accounts you're running and how you want roles assigned:

| Mode | Accounts | What happens |
|------|----------|--------------|
| **Normal** | 2 (Left + Right) | Standard attacker/victim training. |
| **Selfish** | 1 (Right only) | A single account trains on itself — the Left card is hidden. |
| **StrDura** | 2 | Like Normal, but also works in Strength while training durability. |
| **Monster Selfish** | 3 (Victim + two hitters) | Two attacker accounts hit one victim at the same time using the game's own auto‑attack. A third "Right 2" card appears. |

The account cards on screen **change automatically** based on the mode you pick, so you only ever see the windows you need to assign.

> **Monster Selfish note:** this mode relies on the game's built‑in auto‑attack to do the hitting, so the **Attack Delay** option doesn't apply there.

---

## Settings

**Training Settings card:**

- **Mode** — Normal / Selfish / StrDura / Monster Selfish (above).
- **Strike Train** — when training strikes, choose **Strength** or **Speed**.
- **HP Target (%)** — stop hitting the victim once it reaches this HP (choose from 5% up to 45%). Cypher stops a little above the target so it doesn't overshoot.
- **Attack Delay (s)** — pause between hits, from 0.1s to 2.0s. (Ignored in Monster Selfish.)
- **Dynamic Hit** — adjusts hit timing dynamically during the session.
- **One‑Way** — swaps which account starts as attacker vs victim.
- **Attacker Eat** — let the attacker account auto‑eat food too (on by default).

**Per‑account cards:**

- **Pick Window** — assign that account's game window.
- **Dura** — point Cypher at the durability spot for that account.
- **Strike** — point Cypher at the strike spot for that account.

---

## What it handles for you

- **Buys and equips** the training item each round.
- **Watches HP** on the victim and stops cleanly at your target.
- **Auto‑eats food** when an account gets hungry (rotates through your food slots; configurable per account).
- **Stamina aware** — pauses hitting when stamina runs low and resumes once it recovers.
- **Auto‑leave on combat** — if you've enabled auto‑leave in Settings, the macro will pull out when combat is detected.

---

## Tips

- Run the **Monitor** alongside this so you still get disconnect/combat alerts on your alts.
- If hits or HP reads land wrong, re‑check that **every** assigned window is **800 × 600** and re‑pick the **Dura**/**Strike** spots.
- Keep food in your hotbar slots so the auto‑eat system has something to use — see [Inventory Slotter](inventory-slotter.md).

**Emergency stop:** **F6**.
