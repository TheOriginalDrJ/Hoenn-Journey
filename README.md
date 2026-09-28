# Hoenn Journey — FireRed v0.3.1

An early playable Hoenn expansion for FireRed Recomp, not a patched GBA ROM.
The full region and new story are still in development. See ROADMAP.md.

## Quick testing shortcut

Open the normal field Start menu and choose **WARP**. It immediately takes you
to Slateport Harbor at the ferry arrival tile (8,12), facing down. No ticket or
League victory is required. It does not grant items, change story flags, or save
automatically. The normal boat route is unchanged. The shortcut is omitted in
Safari/link menus to avoid leaving those sessions in an invalid state.

## Required companion mod

Install and enable **1025Dex 1.1.28 or newer** for FireRed before enabling
Hoenn Journey. The manifest declares `1025dex@>=1.1.28` as a dependency.
The supplied 1.1.28 ZIP was inspected for species-ID and encounter integration.
Future 1025Dex versions still need compatibility testing.

Hoenn Journey does not bundle Pokémon species definitions, battle sprites,
icons or cries. It resolves species by name through the game's active Pokémon
registry. 1025Dex preserves native Gen 1–3 species slots; no National-Dex-number
guessing is used. Overworld NPC sprites remain part of the Hoenn map assets.

1025Dex's WILD GENS replacement is bypassed **only on Hoenn maps**, using its
existing `__completeDexExact` option. This preserves authored Emerald encounter
tables. Kanto's WILD GENS behavior and the companion's settings are unchanged.
Battle rules and presentation remain owned by FireRed and installed mods;
Hoenn Journey does not install a different battle engine or battle layout.

## Playable now

- Existing post-Champion Birch event beside Oak, Hoenn Ferry Ticket, dedicated
  Vermilion sailor at (23,32), and return ferry from Slateport Harbor.
- Seventeen Emerald-layout maps: Slateport City and Harbor; House and Name
  Rater's House; Mart; both Pokémon Center floors; Pokémon Fan Club; both
  Shipyard floors; both Oceanic Museum floors; Battle Tent lobby; Route 110;
  both Cycling Road gatehouses; Trick House entrance.
- Seventy-seven imported static NPC placements, using 39 ROM-extracted Emerald
  sprite sheets, plus the return sailor. Ordinary dialogue is adapted from
  Emerald; story-gated actors/cutscenes are not transplanted into FireRed.
- Center healing restores HP, status and PP and sets the Slateport blackout
  destination. The Mart uses FireRed's buy/sell interface and ROM prices.
  Energy Guru sells vitamins; the Power TM clerk sells TM10 and TM43.
- Walking between Slateport and Route 110. Original Route 110 land encounters
  (levels 12–13) and water encounter data; fourteen trainer teams with original
  species, levels and explicit moves where present. Battles use FireRed's
  native engine; trainer portraits use FireRed equivalents.
- Trainer line-of-sight engagement and victories saved separately in
  `session.meta.hoennJourneyFireRed.trainers`, with no Kanto trainer-flag reuse.
- Seven rendered Emerald music tracks: Slateport, Route 110, Center, Mart,
  Museum, Battle Tent and Trick House. Native FireRed battle music takes over
  during battles; map music restores afterward. Rendered tracks loop with
  their existing end fades, not sample-perfect sequence looping.

## Install / update

1. Back up your save. Install/enable 1025Dex for FireRed.
2. Import HoennJourney-FireRed-v0.3.1.zip, replacing the older Hoenn Journey.
3. Enable it for FireRed and restart the game so the new hooks load.
4. Obtain the ticket from Birch after the Champion sequence, then use the
   dedicated sailor left of the S.S. Anne entrance. He remains visible before
   receiving the ticket and says: “You still have much to learn on your journey.”

Existing custom city/harbor map IDs and ticket data are retained. Keep both
mods enabled while saving/continuing in Hoenn. Return to Vermilion before
disabling Hoenn Journey. Do not load a Hoenn save without the mod.

## Deliberately unfinished

This is a first world-building slice, **not all of Hoenn**. Mauville and Routes
103/109 are not included; their boundaries are blocked. Battle Tent challenges,
Trick House puzzles, link services, naming service, decoration shopping,
Emerald story quests, berry trees, item pickups, signs/exhibits, animated tiles,
full NPC movement routines and original Cycling Road rules are not implemented.
Special services not implemented have explanatory dialogue where applicable.
Fishing tables and full water/cycling traversal have not been validated.

Levels currently follow early Emerald, so an existing League-winning team will
be overleveled. No player party reset or automatic level scaling is performed.
Postgame balancing and the new story belong to a later pass.

## Verification

The isolated native-engine tests use FireRed's real cached map/battle data and
a temporary character, never the user's save. Verified in this batch:

- All 17 map atlases and all NPC sprites load; 49 usable doorway/stairway links
  work through actual player movement. Script-only/off-map ship warps are blocked.
- City/Center/Mart doors, nurse healing, real shop purchase and money deduction.
- Two-way Slateport/Route 110 walking connection and correct map music IDs.
- Actual wild and trainer battles through completion; trainer sight engagement.
- All 14 trainer teams complete the native headless battle path.
- Trainer victories survive save-schema roundtrip/Continue.
- Actual losing battle returns to Slateport Center and heals the party.
- Original Birch/ticket/ferry regression suite.
- Hoenn encounter preservation with the actual encounters component extracted
  from the supplied 1025Dex 1.1.28 ZIP.

This is not yet an end-to-end launcher test with the **entire** 1025Dex mod,
every existing save, or all other installed mods. Shared-release validation must
include those combinations. Screenshots and test reports are in the workspace's
tests folder, not required by the installed mod.

## Assets and rebuild

Layouts, tiles, palettes and overworld NPC sprites were extracted from the
supplied Emerald ROM. Music was previously rendered from that same ROM for the
local MP3 project; only the seven needed tracks are copied into this package.
No ROM or 1025Dex package is included. Provenance is recorded in
assets/slateport/source.json and expansion-source.json.

Map/event/trainer/encounter metadata uses the
[pret Emerald decompilation](https://github.com/pret/pokeemerald).
The builder is tools/build_hoenn_slice.py (run Python with `-X utf8`), the
renderer is tools/extract_slateport.py, and packaging is tools/package_hoenn.py.
