# Hoenn Journey

**Continue your FireRed adventure in Hoenn.** Hoenn Journey is a playable expansion for **FireRed Recomp**, bringing Emerald's towns, routes, interiors, encounters and familiar faces into your existing character's journey, with a new post-Champion story.

**Current version: v0.18.0** · **In active development** · **Standalone — no companion mod required**

[Download the latest release](https://github.com/TheOriginalDrJ/Hoenn-Journey/releases/latest) · [Report a bug](https://github.com/TheOriginalDrJ/Hoenn-Journey/issues)

## New in v0.18.0

Hoenn Journey now uses FireRed Recomp's native **Gen 1–3 roster** directly: all **386 Pokémon**, **354 moves**, original sprites and cries, abilities, learnsets, evolutions, TM/HM compatibility and breeding data. **1025Dex is no longer required.** The existing Hoenn Pokédex and regional gameplay remain integrated with the native battle, capture, party, storage and save systems.

Only FireRed Recomp and its normal FireRed ROM import are needed. The standalone package does not include later-generation Pokémon or companion-mod HD art. If your save contains Gen 4+ Pokémon, keep their original provider mod enabled; this update does not convert or delete them.

See the [v0.18.0 release notes and screenshots](https://github.com/TheOriginalDrJ/Hoenn-Journey/releases/tag/v0.18.0). The build's full serial regression passed with 307 PASS records; all 2,720 packaged files were byte-verified before publication.

## Previous expansion updates: v0.17.0–v0.17.3

- **Battle Frontier:** all seven single-player facilities, Frontier Brain battles, Symbols, BP, Frontier Pass and surrounding areas, plus all three Battle Tents.
- **Mauville and Trick House:** Rydel's bike selection/exchanges, the Gym's switches and Wattson rewards, and all eight Trick House puzzles.
- **Central Hoenn:** New Mauville's power-plant quest, paired-trainer double battles and Briney's coastal sailing sequences.
- **Interface improvements:** bag quantities, Pokédex alignment, Safari admission dialogue and a reorganized Cheats menu with Left/Right warp paging.

The cumulative import now contains **452 maps**. See the [v0.17.3 release notes and gameplay screenshots](https://github.com/TheOriginalDrJ/Hoenn-Journey/releases/tag/v0.17.3) for details, installation and current limitations.

## Explore Hoenn

- A region-wide collection of imported towns, Routes 101–134, connected interiors, caves, gyms, ocean routes and underwater areas.
- Emerald-based maps, collision and field behavior, NPC placements, dialogue, trainer teams and wild encounter tables.
- Land, water, fishing and Rock Smash encounters preserve Emerald's authored species and level ranges. Battles run through the native FireRed engine.
- Regional travel, Fly destination selection, Surf, Dive, field interactions, Pokémon Centers, shops and Mauville's Game Corner.
- Hoenn location records for caught Pokémon, plus save support for regional progress.

The imported world is the foundation for the new story. Map availability does not mean every Emerald event or service is complete; see [development status](#development-status).

## A Ticket to Hoenn

Chapter 1 continues with your existing FireRed character after the Champion sequence. Oak introduces the PokéNav, Birch invites you to Hoenn, and the journey takes you from Vermilion to Slateport and onward to Littleroot for a briefing at Birch's lab.

The chapter includes calls, ferry travel, the moving truck sequence and a mission system. Your character and party carry forward; this does not restart Emerald's original opening.

## Two regions, your style

Open **Options → Hoenn - Kanto Settings** to choose:

| Setting | Choices |
| --- | --- |
| Player Sprite | Boy, Girl, Brendan, May, Gary, Birch or Oak |
| Backpack | Kanto or Hoenn presentation |
| Pokédex | Kanto or Hoenn presentation |
| Cheats | Show or hide the Hoenn Cheats menu |

Player Sprite changes overworld appearance, including the Fly passenger. Trainer identity, story counterpart and battle backsprites remain unchanged. Gary, Birch and Oak reuse their NPC poses for actions without dedicated animation sheets.

The PokéNav includes Emerald-style menus, the Hoenn region map with zoom and location information, Condition, Ribbons, and Match Call with Oak plus Emerald contacts and rematches. **Highlight the map row on the PokéNav main screen and press Left/Right** to select Hoenn Map or Kanto Map, then press A. Kanto opens FireRed's native map; directions inside either map move its cursor.

## Screenshots

Actual in-game captures. The first four are from the v0.18.0 standalone build; the regional exploration gallery below includes earlier development builds.

| Native Pokémon in the Hoenn Pokédex | Battle Frontier |
| --- | --- |
| ![Hoenn Pokédex with native Treecko artwork](https://github.com/user-attachments/assets/16a9200d-bccf-4633-b406-6391a21c5bd4) | ![Native trainer battle at the Battle Frontier](https://github.com/user-attachments/assets/7afd5c89-ec18-46ee-ad97-dd495020c9d9) |

| Hoenn backpack | Hoenn trainer card |
| --- | --- |
| ![Hoenn backpack in the standalone build](https://github.com/user-attachments/assets/21311a96-4866-451f-8842-a5c05af555c0) | ![Hoenn trainer card in the standalone build](https://github.com/user-attachments/assets/c64c0e88-0ab4-487e-bf14-6fea97be8bd6) |

| Hoenn exploration | Chapter 1 at Birch's lab |
| --- | --- |
| ![Surfing on Route 103](https://github.com/user-attachments/assets/f2c854d6-7751-4194-bbaf-d3c3b7c28ba1) | ![The player meets Birch and May in the lab](https://github.com/user-attachments/assets/833324f9-ad14-4319-a6b0-e574cf615ed6) |

| PokéNav and regional map selection | Hoenn map |
| --- | --- |
| ![PokéNav with Kanto and Hoenn map selector](https://github.com/user-attachments/assets/c877e2ef-975f-424c-bc02-0e13606eaab9) | ![Hoenn region map focused on Slateport](https://github.com/user-attachments/assets/b1d5de7f-7f6a-422a-bff2-bc4599d75f73) |

| Hoenn Pokédex | Appearance and regional settings |
| --- | --- |
| ![Hoenn Pokédex species list](https://github.com/user-attachments/assets/50dbe3e2-561e-4077-a78f-a0d1b4c26104) | ![Player Sprite and Hoenn-Kanto options](https://github.com/user-attachments/assets/800d2bd8-3b25-4dd3-bdf4-77db7bff9b83) |

## Install or update

1. Back up your save. Ensure FireRed Recomp is installed with its normal FireRed ROM import; **no companion mod is required**.
2. Download **HoennJourney-FireRed-v0.18.0.zip** from [Releases](https://github.com/TheOriginalDrJ/Hoenn-Journey/releases/latest). Use the named mod ZIP, rather than GitHub's automatically generated source-code archives or the older ZIP in the repository root.
3. Import it through the game's mod system, replacing the previous Hoenn Journey version, and enable it for FireRed.
4. Restart the game so the updated hooks load, then continue your save.

This is a Recomp mod package, not a patched GBA ROM. Keep Hoenn Journey enabled while continuing a save in Hoenn; return to Kanto before disabling the expansion. If an existing save contains later-generation Pokémon supplied by another mod, keep that provider enabled. v0.18.0 neither converts nor deletes those Pokémon.

Normal access follows the post-Champion invitation and ferry journey. Testing shortcuts are available below.

## Optional testing tools

Enable **Options → Hoenn - Kanto Settings → Cheats**, then open **Hoenn Cheats** from the Start menu. Its root now groups actions into **Ease of Use** and **Warp**; Left/Right changes warp pages.

- Grant all Hoenn badges or all Kanto badges separately.
- Browse imported destinations through **Warp**.
- **HM Move Pokemon:** add two level-100 Zigzagoon with full HP/PP. One knows Surf, Dive, Waterfall and Rock Smash; the other knows Fly, Cut, Strength and Flash. Requires two free party slots.
- Unlock all imported Hoenn town Fly destinations; normal Fly move and badge requirements still apply.
- Toggle NPC battles or random encounters. Disabling battles does not award trainer victories; explicit scripted Pokémon challenges remain separate from random encounters.

**Warp → Flags** offers these checkpoints in order:

1. **Champion Defeat** — test the congratulations and PokéNav gift sequence.
2. **Post Game** — resume in the player's room for the postgame opening.
3. **Birch Conversation 1** — set the preceding Chapter 1 prerequisites and arrive two tiles below Birch after the lab briefing, with the PokéNav and Hoenn map available.

Cheats do not automatically save. Encounter toggles persist with your save and remain active when the Cheats menu is hidden. These tools are intended for development testing and may change before the final release.

## Previous update: v0.16.7

Fixes the crash after saving by preserving Hoenn story progress, flags, defeated trainers, cheats and other regional state through the native save flow. Older saves without Hoenn metadata initialize safely. Replace the mod ZIP and restart; no new game is required. Progress already missing from an earlier save cannot be reconstructed.

## Previous update: v0.16.6

- Added seven selectable overworld appearances to regional settings, with saved selection and support during travel and field actions.
- Raised both HM helper Zigzagoon to **level 100**; existing party Pokémon are unchanged.
- Includes the recent PokéNav Kanto/Hoenn map selector, native Kanto badge grant, encounter toggles, Fly unlocks, story checkpoints and underwater movement repairs.

## Development status

Hoenn Journey is an evolving expansion. Later story chapters, postgame balancing and some Emerald progression events and services still need work. Safari battles currently use FireRed's bait/rock rules rather than complete Emerald mechanics. Some later gym and Wally story progression remains partial. Frontier multiplayer/link modes, Apprentice training and recorded replays are not included. Mach and Acro currently share native bicycle movement.

Emerald graphics, data and behaviors are adapted to the FireRed runtime; complete frame-for-frame Emerald parity has not been established. Encounter levels generally follow Emerald, so an existing Champion team can be overleveled. There is no automatic party reset or level scaling.

When reporting a bug, include the mod version, map or building, steps to reproduce, enabled companion mods and any error text or screenshot.
