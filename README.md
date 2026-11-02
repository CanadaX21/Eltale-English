# Eltale Monsters: English Translation

**Take Eltale Monsters, imagine it had more development time, then was re-translated and brought back to North
America.** That's what I set out to make.

Eltale Monsters is the Japanese release of Quest 64. It came out a year after Quest, with a revised game, a rewritten
story in places and a much longer ending, and it never left Japan. This patch brings it to English, and my priorities
were, in order:

1. **A faithful recreation of the Japanese story.** Every line was worked from the Japanese script and written as
   natural English, using the names Quest 64 players know.
2. **Modernization and polish.** Better controls and camera, friendlier menus, and the help a modern player expects.

It is not an overhaul. The world, story, enemies, stats and progression are Eltale's own, and every gameplay change is
listed below with its original value.

**Want the full story?** [ABOUT.md](ABOUT.md) covers what Eltale is, how it differs from Quest 64, where both games fell
short, my English sources, and where I diverged from them and why. It contains story spoilers.

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

1. Open [Rom Patcher JS](https://www.marcrobledo.com/RomPatcher.js/) in your browser.
2. Pick your Japanese ROM and `Eltale_English.bps`, then apply the patch.
3. Play the patched ROM. It should match:

   | | |
   |---|---|
   | CRC32 | `206DE52D` |
   | SHA-1 | `9d93339076ead19a758634afe59021f1674d5c48` |

A BPS patch checks the ROM it is given. If the patcher refuses your ROM, it is not the expected Japanese dump.

## Where it runs

- **Project64 4.x with GLideN64:** played through from start to finish.
- **ares:** used throughout development.
- **Real hardware and flash carts:** not tested yet. Reports are welcome.

Use an in-game save, not an emulator savestate from another version of the patch.

## Controls at a glance

| Button | In the field | In battle |
|---|---|---|
| Stick | Move | Move inside the movement ring |
| A | Talk, examine, open, confirm | Swing the staff |
| B | Open and close the item menu; cancel | Open and close the item menu; cancel |
| C buttons / D-pad | Spirits and spells | Spirits and spells |
| Z | Tap: camera behind Brian. Hold: keep it there | Tap: face the enemy. Hold: lock on |
| R | Hold to rotate the camera | Hold to rotate; while locked, a side view |
| L | Zoomed-out view (outdoors) | Hold to rotate; while locked, the other side view |
| Start | Start menu (Status, Map, Elements, Environment) | |

Changed from the Japanese release: the item menu moved from R to B, and the camera button from B to Z.

## Everything I changed

### The translation
- **The whole script in English:** 272 dialogue lines, 21 ending lines, the boss speeches, the signs, the backstory
  pages, the epilogue scroll, the menus, and the save and Controller Pak messages.
- **Worked from the Japanese.** Story text that earlier English patches had dropped or changed is restored.
- **Quest 64's text box:** dialogue uses Quest's 27-character, 4-line layout and its English font, so the text can run
  at full length (the Japanese layout held 24 × 3 once in English).
- **Quest 64's English names** for people, places, items and spells, with a few deliberate exceptions listed in
  [ABOUT.md](ABOUT.md).
- **English graphics:** the title logo, menu labels, map pages, the backstory and Controller Pak screens, and the
  epilogue scroll.
- **Dialogue that teaches the new controls:** the monastery and Melrode tutorial characters explain A to confirm, the C
  buttons or D-pad for spirits, Z and the battle camera, and how to use the map feather.

### Field camera and movement
- **Tap Z** to swing the camera behind Brian. **Hold Z** to keep it there (originally hold B). Pull the stick back while
  holding and Brian walks toward the camera while it holds still, with no whiplash.
- **Hold R** to rotate the camera in towns, fields and dungeons.
- **Press L** anywhere outdoors to switch between the normal view and a zoomed-out one. Originally L only changed the
  view in some fields.
- **D-pad** works like the C buttons for choosing a spirit.

### Battle controls and camera
- **Z-targeting:** on Brian's turn, tap Z to face the enemy in front of him. Hold Z to stay locked on while you move.
  A floating gem marks the target, its MONSTER card stays on screen, and the camera frames the two of you.
- **Side views:** while locked on, hold R or L for a side view. A staff swing brings the camera back behind Brian.
- **Battle camera:** hold L or R to rotate it, with steadier aim and follow.
- **Identified enemies:** Soul Searcher's mark is a gem in the enemy's element colour instead of the spell's big orb.

### Quality of life
- **Brian keeps his heading after a battle, whether you win or run.** Eltale already restored it after a win. Escaping
  left him facing wherever the fight ended, so he now turns back too, and the camera follows.
- **The backstory** now also plays when you start a New Game (A turns pages, Start skips).
- **31 new things to examine:** 18 objects whose Japanese text the original game never let you read, and 13 locked
  doors.
- **A save point at Kelly's house** in Glencoe Forest, where the original has none.
- **Fewer empty rooms:** the Melrode Monastery is rearranged so you reach what matters sooner, and some inn bedrooms are
  locked (some with a voice or a sign on the door).

### Item menu
- **A modern fixed-slot panel** in place of the scrolling strip: 14 items with counts, 6 Wings and 6 treasures, each
  always in the same slot, with a description box.
- **On B** (originally R). A uses an item.
- Your saves keep track of which items you have found. Older saves still work.

### Maps and the Start menu
- **New maps** for Connor Forest, Glencoe Forest, Windward Forest, the Blue Cave, Baragoon Tunnel, Boil Hole and Cull
  Hazard, drawn from the game's own layouts in the style of the original maps. Each shows Brian's position, and the map
  feather works on them.
- **Spirit tracker:** every Map page counts the spirits found in its area, and gems mark the ones still waiting. The
  Status page has a Spirits row. The original game counted nothing.
- **Elements page** redesigned: the four elements around an orb that fills as Brian's spirits grow.
- **Feather cursor:** it speeds up as you hold a direction, so a tap moves it about a pixel (originally it jumped).
- **Menu controls:** the D-pad works in menus and on the title screen, and L also turns Start menu pages left.

### On-screen display
- **MONSTER card:** moved to the top right, wider so every name fits, and it shows that enemy's own current HP and
  live Def and Agi (originally the HP was the kind's maximum).
- **Spell labels:** wider, with Quest 64's full spell names. Bosses have names on the card.
- **Text and layout:** roomier dialogue box, centred signs and menu text, and sharper lettering.

### Gameplay changes from the Japanese release
| Change | Now | Originally |
|---|---|---|
| Spell MP cost for one / two / three element presses | 3 / 5 / 7 | 1 / 2 / 3 |
| MP restored by a staff hit | 1 to 3 at random | 1 |
| Wings | Not used up | Used up |
| Soul Searcher Lv1 | Always marks its target | The enemy could avoid it |
| Length of a Soul Searcher mark | 3 to 5 enemy turns | 2 to 4 |
| Dondoran Castle's secret passage opens with | The Earth Orb | The Wind Jade |
| Glencoe Forest and Blue Cave passage opens with | The Wind Jade | The Water Jewel |
| Confirm button | A only | A or Z |
| Shamwood's hidden path | Two tight gaps a little wider | Exactly Brian's width |

Everything else, including stats, enemies and difficulty, is the original game.

### Bug fixes
- Mashing A no longer drops the last line of a message, and a full last line no longer leaves a blank page.
- From earlier English patches: overlong text that froze the game at Nepty, and monster names that showed the wrong text
  on the MONSTER card.
- Thin lines on the map pages under GLideN64.

## What this version doesn't do

- **Balance is not reworked.** MP costs and staff MP are the only balance changes. Spell, element and grinding issues
  shared by both games are left for later.
- **Not yet tested on real hardware.**

My translation sources cover a lot of the Japanese, especially the ending, but I'd still love a Japanese reader's eye on
the script. If you spot something off, please open an issue.

## Credits

- **Translation, planning, design and the project as a whole:** CanadaX21, from the hand-made early 2026 builds on.
- **Claude** (Anthropic's AI model): the tool that took CanadaX21's hand-made mod and added a level of polish that
  wouldn't have been reachable alone.
- **Landmine36:** the 2022 Eltale Monsters patch. Its item, spell and monster names, its English map pages and its
  battle font are where this project began.
- **zmarotrix:** [Eltale Odyssey](https://github.com/zmarotrix/Eltale-Odyssey), where the Z-targeting idea came from.
- Names and some artwork follow Quest 64's English release.

### Translation references

- **Chibitamashi:** [Quest 64 Japanese Ending Script](https://docs.google.com/document/d/1K2UsopNWlO-q68A5TQ7d1pI9E3QPJVozdgis-KSkoiA/),
  an English translation of the ending.
- **Eien Ni Hen:** the English translation of the ending on
  [VGMuseum](https://www.vgmuseum.com/end/n64/b/eltale.htm).
- **The Cutting Room Floor:** [Quest 64/Regional Differences](https://tcrf.net/Quest_64/Regional_Differences).
- **TestaALT:** the Quest 64 FAQ/walkthrough, my first reference for Quest's names.
- **Lvl Jake:** *The Case for Quest 64*, a video series used for background on the world and story.

[ABOUT.md](ABOUT.md) explains what each one was used for.

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
