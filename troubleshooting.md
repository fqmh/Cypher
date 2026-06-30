# Troubleshooting & FAQ

Quick answers to the most common issues. If your problem isn't here, check the **Activity Log** (turn on **Debug Mode** in Settings for more detail) and reach out in the support server.

---

## Clicks land in the wrong place / detections never fire

**Almost always a window‑size problem.** Cypher is calibrated for an **800 × 600** game window. If the window is any other size, vision and clicking break.

- Set the game to **windowed 800 × 600**.
- Don't maximize or resize it after picking it.
- Re‑pick the window (and any per‑account coordinate spots) after fixing the size.

---

## Detections are too sensitive / not sensitive enough

Adjust **Settings → Confidence**:

- **Too many false alerts?** Raise it (e.g. 0.85 → 0.90).
- **Missing real events?** Lower it (e.g. 0.85 → 0.80).

Also make sure the event you care about is actually enabled under **Settings → Detections** — everything is **off by default**.

---

## The macro picked the wrong window

Use **Pick Window** again on that macro's screen and select the correct game window during the short selection window. The chosen title shows next to the button; if it reads "none", nothing is assigned yet.

---

## Auto‑eat / re‑buy isn't working

The food and item systems need the right items in your hotbar:

- Keep **food** in the slots the auto‑eat system uses.
- Keep your **training item** stocked and in the expected slot.
- Use the [Inventory Slotter](macros/inventory-slotter.md) to set this up consistently.

---

## A macro is doing something I don't want — stop it!

Press **F6**. That's the emergency stop and it halts the running macro immediately. You can also press its **Stop** button.

---

## License / activation problems

- Make sure you typed your key correctly and have an internet connection, then relaunch.
- Your license is tied to your machine; sharing or revoking it can end your session.
- If Cypher says your version is out of date, accept the **update prompt** — it will download the new version and relaunch, keeping your settings.

See [Getting Started](getting-started.md#3-first-launch--license).

---

## It won't run at all

- Cypher is **Windows‑only** (Windows 10/11). It cannot run on Mac or Linux.
- Launch it from the **Start‑menu shortcut** the installer created, not from inside a zip.

---

## Discord alerts aren't arriving

- Confirm the **Webhook URL** is pasted correctly in Settings and you clicked **Save Settings**.
- Test by enabling a simple detection (like Disconnect) and the Monitor.
- If you want to be pinged, set your **Discord Mention ID** too.

---

## Frequently asked

**Can I run more than one account?**
Yes — that's a core use case. The Monitor watches all your open game windows, and several macros support multiple accounts (Durability supports up to three).

**Can I run a macro and the Monitor together?**
Yes. Start the Monitor, then start your macro — they run side by side.

**Will updating wipe my settings?**
No. Updates preserve your `config.json` (settings) and your saved license key.

**Where are my settings stored?**
In `config.json` next to the app. You normally edit everything through the Settings tab.
