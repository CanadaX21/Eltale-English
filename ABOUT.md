# About this project

**Story spoilers ahead**, including the ending. For how to install and play, see the [README](README.md).

## The idea

Take Eltale Monsters, imagine it had more development time, then was re-translated and brought back to North America.

The Japanese story comes first. Modernization and polish come second. My goal is for you to play this, go back to Quest
64, and feel how much was left on the table, without my turning the game into something else.

## What Eltale Monsters is

Quest 64 and Eltale Monsters are the same game at two stages of its life. Imagineer developed it, and the Japanese
version shipped last.

| Release | Region | Publisher | Date |
|---|---|---|---|
| Quest 64 | North America | THQ | June 1998 |
| Holy Magic Century | Europe | Konami | September 1998 |
| Eltale Monsters | Japan | Imagineer | July 1999 |

The extra time went into the game. As The Cutting Room Floor puts it, "many changes were made to fix the little quirks in
the gameplay." Under the hood it is still close to Quest: 595 of Eltale's 836 functions are byte-identical to Quest 64's.
But the story, ending and many details changed, and English speakers never got that version.

## Version differences

**How to read this:** "Confirmed" means I checked it against the Eltale ROM, its code or its script. "Reported" comes from
community documentation (mainly The Cutting Room Floor) and I haven't independently confirmed it.

### Story and text
| | Quest 64 | Eltale Monsters | Status |
|---|---|---|---|
| The ending | A scene with Shannon and a text scroll | A much longer ending that visits the whole cast | Confirmed |
| Credits | Plain sky | Flyover of the game's places | Reported |
| Zelse | Ambition | Tilly's brother, seeking revenge on King Beigis for burning Greenoch | Confirmed |
| Leonardo | A magician who met "old Bart" and seeks the "Alchemist's Secret" | A young spirit tamer in training who idolizes "Mr. Bart" | Confirmed |
| Signs and objects | Signs can't be read | Signs can be read, and objects examined | Confirmed |
| Mammon's World | | Epona has added dialogue explaining what it is | Reported |
| Names | Brian, Kennishire, Carmagh, Highland, Dondoran, Shamwood, Greenoch | Jean-Jacques, Stonia, Angurus, Veragoon, Darlam, Shellwood, Glenos | Confirmed |

### Gameplay
| | Quest 64 | Eltale Monsters | Status |
|---|---|---|---|
| Critical hits | None | Both sides, for 1.5× damage | Eltale's rule confirmed |
| Item drops | Only when you hold none of that item | When you hold fewer than 3 | Eltale's rule confirmed |
| Brian's heading after a win | | Restored by Eltale-only code | Confirmed |
| Map marker | None | Place a marker; the compass points to it | Confirmed |
| Defense and Agility growth | | Defense twice as fast, Agility faster | Reported |
| Magic Barrier | 2 to 3 turns | 2 to 6 turns | Reported |
| Staff | | Double attack | Reported |
| Boss rewards | HP only | HP and MP | Reported |
| Guilty and Mammon | No element | Have an element, so spells deal about twice the damage | Reported |
| First boss | | Deals less damage | Reported |
| Items | | Different monastery items and one Boil Hole chest | Reported |

### Presentation
| | Quest 64 | Eltale Monsters | Status |
|---|---|---|---|
| HP and MP display | Fades while moving | Always on screen | Reported |
| Stat increase | No signal | Coloured mist and a sound on Brian | Reported |
| Battle ring | Octagons | Circles | Reported |
| Spirit crystal | | Glows when an element is maxed | Reported |
| Save menu | | New music | Reported |

## Where it began

I started this as notes for a Quest 64 balance and quality-of-life mod. My first guiding principles were about spell
levels, element balance, MP, items and grinding, and the last one has stayed with the project ever since:

> Stay within the scope of the original game. Imagine the devs knew the finished game was their end goal... don't add
> quests / NPCs / additional story just because you have the tools to do so. Any additions must serve a specific purpose.

That work moved to Eltale, because Eltale was already the better base and English speakers had never had it. I built on
Landmine36's 2022 patch, made hand-built versions in early 2026, and in October 2026 it grew into a full translation and
polish project.

## The rules I worked by

1. **The Japanese script is the story.** Who says what, why, and what it reveals stays the same.
2. **Natural English, not word for word.** Readability comes first, but the meaning stays.
3. **Quest 64 supplies the names** a North American player knows. Japanese-derived names only where Quest has none.
   Monster names came from Landmine36's patch and mostly matched Quest; the next update brings the rest in line.
4. **Never cut story to fit the ROM.** If text doesn't fit, move it or fix the engine.
5. **Additions need a reason:** the player would otherwise be stuck or unaware, or the game already establishes the fact.
   They must not contradict the Japanese.
6. **The best version of the game, not a museum piece.** Eltale's additions stay. Quest was one of the first 3D RPGs on
   the N64, and fixing poor early decisions is welcome. Ocarina of Time is the baseline players expect.
7. **Interfaces can be rebuilt** if that plays better, in Eltale's own art style.
8. **A logical, documented ROM** that others can build on.

## Where both games fell short

Eltale fixed a lot of Quest 64, but much of the underlying design carried over, since the two share so much code. These
are the problems I set out to help with:

| Problem | What I did |
|---|---|
| Eltale's full story and ending never reached English speakers | **Translated it in full** |
| The dialogue box was too small for full English text | **Quest's 27 × 4 box** |
| The camera was awkward: hold a button and wait for it to come round | **Tap and hold Z, R to rotate, L to zoom** |
| No way to aim at or stay facing an enemy | **Z-targeting with a lock-on camera** |
| Running from a battle left you disoriented | **Brian turns back to his heading** |
| The item list was a scrolling strip | **Fixed-slot item menu with counts** |
| Forests and caves showed only the surrounding region's map | **Seven new area maps** |
| Nothing tracked which spirits you had found | **Spirit tracker** |
| The game could leave you unsure where to go next | **A few short, grounded hints** |
| The monastery opens with a run of empty rooms | **Monastery rearranged** |
| Glencoe Forest has no save point | **A save point at Kelly's house** |
| Standing still and spamming low-cost spells | **Partly addressed:** spells cost 3 / 5 / 7 MP, staff hits restore 1 to 3 |
| Element balance, spell progression, grinding | **Not addressed in 1.0** |

## Why this improves the game without overhauling it

**What stayed the same:** the regions and the story's order; every monster and its stats; Brian's growth; the spell list
and how spirits work; bosses and difficulty.

**What changed:** how the game is read, controlled and navigated. Only a handful of rules changed, along with the
monastery's layout, and the README lists them with their original values. The two that change play most are spell costs
and reusable Wings.

**What I held back from:** new quests, new areas or a new battle system. I added no new story arcs. Added text is short,
listed below, and has a stated reason wherever I could give one. Balance is a separate job, and I left it out of 1.0 rather
than rush it.

## My English sources, and where I diverged

**Order of authority:** the Japanese script, then Quest 64's English for names, then everything else.

| Source | What I used it for | Where I diverged, and why |
|---|---|---|
| **Eltale Monsters (Japan)**, the ROM's script | The story. Every line was checked against it. | Not word for word, for natural English. The additions below go beyond it. |
| **Quest 64 (USA)**, the ROM's English script | The authority on names, plus the text box, font and some artwork. I searched its text directly. | Its story text isn't copied, because Eltale often says something different. Only 1.6% of the display lines match a Quest line exactly, mostly save messages. |
| **Landmine36's 2022 patch** | Item, spell and monster names, map pages, the battle font, the opening and some system text. | Dialogue was redone. Name display errors were fixed, and the opening was retranslated. |
| **My early 2026 builds** | The first English for inns, NPCs and system messages. | Checked against the Japanese in October 2026. Of 189 inherited lines that had never been checked, 146 were retranslated, restoring things like Shannon's reveal and Zelse's motive. Spell names I had shortened went back to Quest's full ones. |
| **Chibitamashi's ending script** | A reference for reading the Japanese ending, and for "master spirit tamer". | Rewritten for my names, box and voice. I use "master" in the ending only (see below). |
| **Eien Ni Hen's ending (VGMuseum)** | A second reference for the ending. It also says "master Spirit Tamer". | Rewritten the same way. |
| **The Cutting Room Floor** | Version differences, Quest-to-Japanese name pairs, and a third English reading of the ending. | Quest's own ROM decides spellings. TCRF writes "Bartholomew", while Quest and my text say "Bartholomy". |
| **Version differences list** (community notes) | Where to look for gameplay differences. | Treated as leads. Items are marked above as confirmed or reported. |
| **TestaALT's Quest 64 guide** | My first name list, and a note that the game gives no hint after Nepty. | The Quest ROM replaced it as the authority on spelling once I could search it. |
| **Lvl Jake's *The Case for Quest 64*** | Background on the world and story. | It covers Quest, not Eltale. The Japanese always wins, its theories were never used as canon, and its names were checked against the ROM. |

### Specific choices

- **"True" and "master" spirit tamer.** The Japanese uses 真の精霊使い, literally "true spirit tamer". Both fan ending
  translations use "master spirit tamer" for Leonardo's line, and TCRF's has "envoy." I use "true spirit tamer" while the
  journey asks whether Brian is one, and "master spirit tamer" in the ending, where everyone answers that he is.
- **Sylph, not Shilf.** Quest says Shilf. I use Sylph, which she introduces herself as.
- **"My Master."** Sylph, Guilty and Shannon call Mammon 『あの方』, never by name, and I keep that distance. Quest just
  says "Mammon."
- **Leonardo.** His name comes from Quest, his character from Eltale.
- **Pirate Ship,** not Quest's "Seagoing Ship," to match the dialogue.
- **"Gaol."** Dark Gaol is the place, plain "prison" is the common word, and Lavaar alone says "the gaol", being a
  thousand years behind.
- **The backstory pages** reuse Quest's English artwork and wording where it fits. This is the one place where I knowingly
  follow Quest over the Japanese. For example, "fell under an evil spell" isn't in the Japanese, which simply says the
  book vanished.

### Text that isn't in the Japanese

| Where | What I added or changed | Why |
|---|---|---|
| Epona, after Nepty | Where to go next | The original gives no hint here |
| Ellis, Larapool | The ship to Limelin sails again | Nothing in Larapool tells you |
| Talco and Walt | Pointers toward Shamwood | It's optional, and nothing leads there |
| Morague, the ferry | Entering the cabin sets sail | Players could leave before they were ready |
| Kelly, Glencoe Forest | A rest offer, and a line that names no jewel | She is a new save point, and the door's requirement moved |
| Pete, Fergus, Todd and other tips | The new controls and the map feather | They teach what changed |
| Wings givers | The new Wings rules | Wings are reusable and don't work everywhere |
| Shannon | A line as she hands over the Dark Gaol Key | She gives it silently in the Japanese; Quest mentions it |
| Mammon's last words | My wording, built around the Japanese lines | The climax, kept to the Japanese beats |
| Dondoran library shelf | A clue about a draft, replacing three joke titles | The joke didn't work in English |
| Inn doors | Guests' voices and signs | Inns felt empty; this is a small touch of world-building |
| Princess Flora | Her wish to see the world, and "Promise you'll come back" | Sets up her ending line, "You'll come back, won't you?" This is my largest creative addition. |

## How it was made

I built the early versions by hand, on top of Landmine36's patch, and the translation, planning, design and project as a
whole are mine. Claude, Anthropic's AI model, was the tool that took that hand-made mod and added a level of polish I
couldn't have reached alone.

I also reorganized the ROM into a documented base for other mods and balance patches. I'm happy to share the docs.

## If you read Japanese

My translation sources cover a lot of this, especially the ending, but I'd still love a Japanese reader's eye on the
script. If you spot something off, please open an issue.

## What's next

- Real hardware testing.
- A 1.0.1 update with small fixes, including monster names that match Quest 64.
- A balance pass, starting from my original principles. It may ship as an optional patch.
