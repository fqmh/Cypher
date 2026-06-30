# The Interface

Cypher is a single warm‑glass window with a floating sidebar on the left, your current screen in the middle, and a thin status strip along the bottom.

---

## Navigation (sidebar)

The sidebar lists every screen, in order:

1. **Monitor** — watch your accounts and react to events.
2. **Durability Macro** — durability training (1–3 accounts).
3. **Trials Macro** — automated Trials combat.
4. **Shadow Boxing** — solo shadow boxing grind.
5. **Roadwork** — roadwork training routes.
6. **Fat Macro** — fat training grind.
7. **Inventory Slotter** — auto‑arrange your hotbar.
8. **Timer** — custom cooldown timers.
9. **Settings** — configure everything.

Click any item to switch screens. The view slides in smoothly so you always know where you are.

---

## Status strip (bottom)

Along the bottom you'll always see:

- The **current screen** name.
- **Runtime** — how long the current activity has been running (HH:MM:SS).
- A live **Timer** readout.

---

## Common controls

Most screens share the same building blocks, so once you learn one macro you know them all:

- **Start / Stop button** — the big copper button. It starts the activity and turns red ("Stop") while running. Press it again to stop.
- **Pick Window** — puts Cypher into a short selection mode (a few seconds) so you can click the game window you want this macro to control. The chosen window's title then shows next to the button (it reads "none" until you pick one).
- **Toggles (switches)** — on/off options. Slide on to enable.
- **Dropdowns** — pick from a fixed list (e.g. HP target, stamina %).
- **Text/number fields** — type a value (e.g. interval seconds, in‑game speed).
- **Tooltips** — hover almost any option to get a plain‑language hint about what it does.

> Anytime you change something on **Settings**, click **Save Settings** so it's remembered next launch. Macro screens apply their options live when you press Start.

---

## Global hotkeys

These work anywhere, even when Cypher isn't focused:

| Key | Action |
|-----|--------|
| **F6** | **Emergency stop** — instantly stops the running macro. Your safety key. |
| **F4** | Launch the **Inventory Slotter** run. |
| **F8** | Trigger a **Medal clip** (only if "F8 Medal Clip" is enabled in Settings). |

> Keep **F6** in mind at all times. If a macro does something unexpected, tap F6 and it stops.

---

## A note on multitasking

Cypher runs everything in the background with separate worker threads, so you can:

- Run a macro **and** keep the Monitor watching at the same time.
- Switch screens freely while things run — stopping a macro is done with its Stop button or F6, not by leaving its screen.

Next: **[Monitor & Detections »](monitor.md)**
