# Getting Started

This page takes you from a fresh license key to a running app.

---

## 1. What you need

- A **Windows 10 or 11** PC.
- Your Roblox game installed and able to launch.
- Your **Cypher license key** (you receive this when you purchase).

> Cypher cannot run on Mac or Linux — it relies on Windows‑only input and screen‑capture APIs.

---

## 2. Install Cypher

Cypher ships with a small **installer** that does everything for you:

1. Run the **Cypher installer** (`setup`/`CypherMacro setup` executable you were given).
2. When prompted, **paste your license key** and confirm.
3. The installer talks to the license server, downloads the current version, and unpacks it into a `CypherMacro` folder next to itself.
4. It creates a **Start‑menu shortcut** and launches the app for you.

That's it — from then on you launch Cypher from the **Start menu** (or the shortcut it created). Your key is saved, so you won't have to paste it every time.

> **Updating later is automatic.** When a new version is out, Cypher detects it on launch and offers to update. If you accept, it downloads the new files, swaps them in, and relaunches — keeping your `config.json` settings and saved key intact.

---

## 3. First launch & license

On every launch, Cypher verifies your license before the app opens.

- If your key is valid, the main window appears.
- If it's the first time on this machine, you may be asked to **enter your key** once; it's then stored securely on your PC.
- Your license is tied to your machine. If you revoke or share it, the session can be ended automatically.

If the license check fails, double‑check that you typed the key correctly and that you have an internet connection, then relaunch. See [Troubleshooting](troubleshooting.md) for more.

---

## 4. Set your game window to 800 × 600

**This is the single most important setup step.** All of Cypher's vision and clicking is calibrated for an **800 × 600** game window.

- Make sure your Roblox game is running in **windowed mode** at **800 × 600**.
- Don't maximize it, don't resize it, and keep it fully visible (Cypher captures the window directly, but a correct size is essential).

If clicks land in the wrong place or detections never fire, the window size is the first thing to check.

---

## 5. Point Cypher at your game

Open the **Settings** tab and confirm how Cypher finds your game:

- **Detect By** — `Window Title` (default) or `Executable`.
- **Window Title** — default `Roblox`.
- **Exe Name** — default `RobloxPlayerBeta.exe`.

The defaults work for a standard Roblox install. Only change these if you run a custom launcher. Full details are in the [Settings Reference](settings.md).

---

## 6. (Recommended) Connect Discord

To get alerts on your phone or desktop:

1. In your Discord server, create a **webhook** (Server Settings → Integrations → Webhooks → New Webhook → Copy URL).
2. Paste it into **Settings → Webhook URL**.
3. Optionally add your **Discord Mention ID** so important alerts ping you.
4. Click **Save Settings**.

Now go to [Monitor & Detections](monitor.md) to choose what you want to be alerted about.

---

## 7. You're ready

- To **watch accounts**, open **Monitor** and press **Start**.
- To **run a grind**, open the macro you want (e.g. **Durability**), pick your window(s), and press its **Start** button.
- To **stop everything instantly**, press **F6**.

Next: learn your way around the app in **[The Interface »](interface.md)**
