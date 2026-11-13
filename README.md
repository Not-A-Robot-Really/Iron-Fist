# IRON FURY — Blood · Steel · Glory

A 2D pixel-art, Mortal Kombat-style street fighting game (1 Player vs CPU) built as a **single self-contained HTML file**: no assets, no dependencies, no build step. All art, lighting and the pixel fonts are generated on canvas at runtime, and all audio is synthesized with WebAudio.

**▶ Play:** open `index.html` in any modern browser (or visit this repo's GitHub Pages site).

## What's new in v3
- **DASH (C)**: a burst → glide → skid dash that costs stamina, with a backdash, an air dash and **dash-cancels** out of landed hits. The first frames hop over low attacks. Without enough stamina you stumble.
- **Stamina gauge on top**: a segmented 10-cell gauge above the health bar. It shows the drain ghost, a regen shimmer, a WINDED warning, and a red bracket marking the cost of an action you couldn't afford.
- **Lighting and post-processing**:
  - Per-arena light rigs and projected silhouette shadows (weapon included).
  - Rim light, plus a dynamic point-light lightmap: torches, fire, projectiles and hit sparks all light the scene.
  - Bloom, colour grading, depth fog, heat haze, wet-floor reflections and film grain.
  - Options › FX Quality has HIGH and LOW, and the game auto-drops to LOW on slow machines.
- **Weapon life**: blade glints, venom drips, hammer embers, scythe soul-wisps, flask bubbles and more. Edges flash on active frames, a weapon glows while its status burns on the foe, and impacts puff in the status's colour.
- **Camera director**: rare, cooldown-gated punch-in zooms on counter-hits, perfect parries, clash wins, disarms and reactions, plus a slow push-in on the final K.O. and a match-point tension zoom.
- **Pixel-art game UI**:
  - Riveted iron 9-slice frames everywhere, and a custom IronPixel bitmap font (regular and bold) used by the HUD, menus and banners.
  - Buttons with stepped shine sweeps, rivet glints, rising forge embers, press sparks and a metallic click.
  - A pixel HUD with dithered chip damage, 8×8 status icons, a pixel timer plate, diamond round pips and a pixel difficulty gauge.
- **New fighters**:
  - **ITZEL, Jaguar Warrior** (pouncing rushdown, Jaguar Spirit, *Fifth Sun Eclipse* Ultimate).
  - **DR. CORVUS, Plague Doctor** (trapper and zoner: Miasma, Crow Swarm, *Black Death* Ultimate).
- **New weapons**:
  - **Obsidian Macuahuitl** (bleed + sunder; obsidian shatters inside the wound on counter-hits).
  - **Alchemist Flasks** (auto-aimed lobbed fire, tar and venom pools; fire ignites tar).
- **New arenas**:
  - **Templo Mayor** under a total eclipse (Solar Flare hazard).
  - **London Rooftops, 1888** in pea-soup fog (Big Ben tolls and the chimneys belch blinding soot).

## Features
- **13 fighters** with distinct styles: unique chains, a FWD+Q command normal, two specials (F›FWD›E and BACK›FWD›Q), their own weight, jump and defense, and cinematic Ultimates.
- **13 weapons**, each with its own speed, range, damage and status: Sword (bleed), Bow (pin), Dual Daggers (poison), War Hammer (stun), Frost Glaive (freeze), Inferno Whip (burn), Storm Chakram (shock), Kusarigama (pull), Reaper Scythe (curse), Shield & Mace (sunder + reflect), Nunchaku (momentum), Macuahuitl (bleed + sunder), Alchemist Flasks (burn / slow / poison).
- **11 animated pixel-art arenas**, each with a hazard: Colosseum, Great Wall, New York alley, Iron Forge, Sakura Temple, Frozen Fjord, Pyramids of Giza, Neo-Tokyo Rooftop, Storm Pirate Ship, Templo Mayor and London Rooftops.
- **Combat systems**:
  - Elemental Reactions: Shatter, Toxic Blast, Conduct, Hemorrhage, Neuroshock.
  - Blade Clash duels, disarm & steal, crowd Hype and **FINISH THEM** finishers.
- A CPU AI with 4 difficulty levels (it dashes, backdashes and dash-cancels), costume customization and a practice mode.

## Controls
| Key | Action |
|---|---|
| A / D | Move (double-tap also dashes) |
| **C** | **Dash** (hold back = backdash; in air = air dash; after a landed hit = dash cancel) |
| W / Space | Jump (again in air = double jump) |
| E | Punch |
| Q | Kick |
| F | Crouch (F+E uppercut, F+Q sweep) |
| R | Weapon strike (hold with bow to charge; pick up weapons) |
| 2 | Weapon Art |
| 1 | Ultimate (charges from damage dealt) |
| S | Block. Tap just before a hit to Perfect Parry |
| Shift | Dodge roll / air dash |
| G | Grab / throw (in air: throw your weapon) |
| X | Swap weapon |
| Esc | Pause |

**Combo inputs:**
- `FWD+Q`: command normal
- `back fwd Q`: second special
- `E E Q`: Iron Chain
- `Q Q R`: Rising Steel
- `back fwd R`: Steel Lunge
- `F → fwd → E`: character special
- `hit → C`: dash cancel
