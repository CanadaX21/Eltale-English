# Eltale Monsters: English Translation

An English translation patch for **Eltale Monsters**, the Japanese release of Quest 64.
Eltale has its own script, ending and gameplay, so this is not Quest 64 again. Everything is in English: every line
of dialogue, the signs, the boss speeches, the ending and its epilogue, the menus and the save screens. The patch also
brings in modern controls and some quality-of-life features.

**Version 1.0**. Download `Eltale_English.bps` from the [Releases](../../releases) page.

## What you need

- Your own ROM of **Eltale Monsters (Japan)** in `.z64` (big-endian) byte order. No ROMs are provided here.

  | | |
  |---|---|
  | CRC32 | `24D937BF` |
  | MD5 | `9b456acb96291fc8b55232a08ae03346` |
  | SHA-1 | `4161b5c100ec82b0241b20ca8f81366e23564ccb` |

  If your ROM is `.n64` or `.v64`, convert it to `.z64` with any N64 byte-order tool first.
- The patch, `Eltale_English.bps`.

## How to patch

1. Open [Rom Patcher JS](https://www.marcrobledo.com/RomPatcher.js/) in your browser, or use
   [Flips](https://github.com/Alcaro/Flips).
2. Pick your Japanese ROM and `Eltale_English.bps`, then apply the patch.
3. Play the patched ROM. It should match:

   | | |
   |---|---|
   | CRC32 | `CE75A721` |
   | SHA-1 | `77eba8e4163262a8502b9214dec4320fb8de7ce7` |

A BPS patch checks the ROM it is given. If the patcher refuses your ROM, it is not the expected Japanese dump.

## Where it runs

- **Project64 4.x with GLideN64:** played through from start to finish.
- **ares:** used throughout development.
- **Real hardware and flash carts:** not tested yet.

Use an in-game save, not an emulator savestate from another version of the patch.

## What's in it

### Translation
- Every line of dialogue, the signs and the boss speeches, rewritten to fit Quest 64's 27 × 4 text box. Story text
  that earlier English patches had dropped is restored.
- The ending, the epilogue scroll, and the backstory pages, which now also play when you start a New Game (A turns
  the pages, Start skips them).
- Quest 64's English names for people, places, items and spells.
- English title logo, menus, map pages, the Controller Pak screens and the save screen's place names.

### Controls and camera
- **D-pad:** works like the C buttons for choosing a spirit, and moves through the menus.
- **Field camera:** tap Z to swing the camera behind Brian; hold Z to keep it there. Hold R to rotate the camera in
  towns, fields and dungeons. Press L outdoors to switch between the normal view and a zoomed-out one.
- **Z-targeting in battle:** on Brian's turn, tap Z to face the enemy in front of him. Hold Z to stay locked on: a
  gem marks the target, its MONSTER card stays on screen, and the camera frames the two of you. While locked, hold R
  or L for a side view; a staff swing brings the camera back behind Brian.
- **Battle camera:** hold L or R to rotate it. When you escape a battle, Brian turns back the way he was facing.
- **Menus:** confirm with A. The item bar closes with B.

### New features
- **Item menu:** every item has a fixed slot with a count.
- **New maps** on the Start menu's Map page for Connor Forest, Glencoe Forest, Windward Forest, the Blue Cave, Baragoon
  Tunnel, Boil Hole and Cull Hazard. Each shows Brian's position, and you can set the map feather on them.
- **Spirit tracker:** every Map page counts the spirits found in its area, and gems mark the ones still waiting. The
  Status page has a Spirits row, and the Elements page is redesigned.
- **31 new things to examine**, including objects whose text the original game never let you read.
- **A save point at Kelly's house** in Glencoe Forest.

### Gameplay changes from the Japanese release
- Spells cost 3 / 5 / 7 MP for one / two / three element presses (originally 1 / 2 / 3), and a staff hit restores
  1 to 3 MP (originally 1).
- Soul Searcher Lv1 always marks its target, and a mark lasts 3 to 5 enemy turns.
- Dondoran Castle's secret passage opens with the Earth Orb. The way between Glencoe Forest and the Blue Cave opens
  with the Wind Jade.
- The Melrode Monastery has fewer empty rooms, and some inn bedrooms are locked.
- The hidden path in Shamwood is a little easier to slip into.

Everything else, including stats, enemies and difficulty, is the original game.

## Controls at a glance

| Button | In the field | In battle |
|---|---|---|
| Stick | Move | Move inside the movement ring |
| A | Talk, examine, open, confirm | Swing the staff |
| B | Cancel, close the item bar | Cancel |
| C buttons / D-pad | Spirits and spells | Spirits and spells |
| Z | Tap: camera behind Brian. Hold: keep it there | Tap: face the enemy. Hold: lock on |
| R | Hold to rotate the camera | Hold to rotate; while locked, a side view |
| L | Zoomed-out view (outdoors) | Hold to rotate; while locked, the other side view |
| Start | Start menu (Status, Map, Elements, Environment) | |

## Credits

- **Translation, design and code:** CanadaX21. Everything after Landmine36's patch, the early 2026 builds included.
- **Landmine36:** the 2022 Eltale Monsters patch. Its item, spell and monster names, its English map pages and its
  battle font are where this project began.
- **zmarotrix:** [Eltale Odyssey](https://github.com/zmarotrix/Eltale-Odyssey), where the Z-targeting idea came from.
- Names and some artwork follow Quest 64's English release.

### Decompilation and research

The code changes stand on the community's work decompiling Quest 64 and Eltale Monsters:

- **Mallos31:** the [Eltale Monsters](https://github.com/Mallos31/EM) and [Quest 64](https://github.com/Mallos31/Quest)
  decompilations, and the Quest 64 function spreadsheet linked from them.
- **Rainchus:** the [Quest 64 decompilation](https://github.com/Rainchus/Quest64-Decomp),
  [Quest 64: Recompiled](https://github.com/Rainchus/Quest64-Recomp) and Quest 64 scratches on decomp.me.
- **vbhayden:** Quest 64 scratches on decomp.me and
  [Quest-64-Lua-Resources](https://github.com/vbhayden/Quest-64-Lua-Resources). They helped map the game's camera,
  collision and menu code.

## Disclaimer

This is a fan project. It is not affiliated with or endorsed by Imagineer, THQ or any rights holder. No ROMs are
distributed. You need your own copy of the game.
