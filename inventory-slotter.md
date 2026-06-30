# Inventory Slotter

A setup tool, not a grind. The Inventory Slotter arranges your **hotbar** for you: you design the layout you want once, save it as a preset, and Cypher drags the right items into the right slots in‑game by recognising their icons.

This keeps your food, weapons, and training items in the exact slots the other macros expect.

---

## How the screen is laid out

**Item Library** (left)
- A grid of item icons loaded from your assets folder.
- **Refresh** re‑reads the icons from disk (use it after adding new ones).
- Click an item to select it.

**Hotbar Layout** (middle)
- The eight‑plus hotbar slots, labelled by their key (**1–7**, plus **R**, **T**, **Y**).
- With an item selected, **click a slot** to assign it there.
- **Right‑click a slot** to clear it.
- Empty slots show a **+**; a slot whose image is missing shows a "not found" icon.

**Presets** (right)
- **Preset name** + **Create** — save your current layout under a name.
- **Preset dropdown** + **Load** — load a saved layout into the slots.
- **Save** — overwrite the selected preset with the current layout.

---

## Using it

1. Open the **Inventory Slotter** tab.
2. Build the layout you want: click an item in the Library, then click the hotbar slot it should go in. Repeat. Right‑click to clear mistakes.
3. (Optional) Type a **Preset name** and click **Create** to save this layout for later.
4. Press **Start Slotting** — Cypher opens your in‑game inventory, finds each configured item by its icon, and drags it into the matching hotbar slot.

> You can also trigger a slotter run with the **F4** hotkey.

---

## Adding your own item icons

The Library shows whatever `.png` icons are in your **assets** folder (set under **Settings → Assets Path**). To add an item:

1. Save a clean screenshot/crop of the item's inventory icon as a `.png` in that folder.
2. Back in the Slotter, click **Refresh** — it appears in the Library.

If the Library is empty, the screen tells you which folder to drop icons into.

---

## Tips

- Keep your **food** in the slots the auto‑eat system uses so every macro can feed your character.
- Recognition uses image matching, so use crisp, correctly‑sized icons for reliable slotting.

**Emergency stop:** **F6**.
