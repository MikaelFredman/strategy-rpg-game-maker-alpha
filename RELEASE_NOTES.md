# Release notes — 0.2.0-beta.7

Released: 24 August 2026

## Highlights

- Fixed AI spectator rounds overwriting arrows, fireballs and damage labels before their animation timeline completed. A resolved round now remains visible for the full effect window.
- Tactical formations advance simultaneously in 0.5-second frames. Round movement duration follows the longest path rather than adding every combatant's route together.
- Equipped bows now provide four-hex attacks and ranged AI positioning to any compatible character; equipped spears provide two-hex reach. Spell range remains four hexes.
- Authoritative battle events preserve both movement routes and tactical effects for diagnostics and future network presentation.
- Tactical movement now follows the resolved hex route one tile at a time at the same 0.5-second cadence used on world maps.
- Sword/axe swings, spear/lance thrusts, bow releases, unarmed strikes and staff-conjuring gestures originate at the acting figure before projectile or impact effects resolve.
- Character Editor supports optional weapon-specific animation chains with at most five steps. Authors can copy the base mesh pose to step 1, copy the previous step forward or use the local Copy/Paste pose clipboard.
- Item Designer explicitly associates a weapon with its fight-animation family, including custom spears and staffs.
- The new **Project Dashboard** turns the complete authoring process into a guided Maps → Rules → Story → Content → Validate → Playtest flow, with project metrics, readiness and a recommended next action.
- Map Browser now offers editable starting templates for an outdoor region, indoor stronghold, cave dungeon and five common tactical arenas: open field, forest, river crossing, great hall and cavern.
- Story dialogues have clearer speaker identity, scene progress and numbered choices.
- Ravenwood conclusions now open a Campaign Chronicle that explains how rescued civilians, bridge support, ritual anchors and the use of Hope shaped the ending.
- Ravenwood Pass now has a classical fantasy opening, a continuous consequence-driven story and three distinct endings.
- Four heroes receive editable permanent progression choices, while 18 campaign items support equipment, consumables, wards and quest outcomes.
- Ten setting-neutral tactical maps cover meadow, river, forest, stone pass, fortress, indoor hall and cavern encounters.
- Game makers can create or retag their own maps as **Battle**, then use them as the game default or assign them to selected world hexes.
- The Hex Actions selector displays a real miniature preview before a separate Apply action changes any selected hexes.
- The AI follows prerequisite-aware story targets and the balance regression runs the complete Ravenwood campaign.

## Ravenwood campaign

The Wardens of Ravenwood defend an old pact between the pass, its common crossing and the living forest. Grimfang, once a Warden himself, seeks the Heartstone beneath Whispering Cavern so he can forge it into the Thorn Crown.

The player begins with **Prologue — The Broken Oath**, chooses whether to rescue refugees or race toward the bridge, develops the four heroes through permanent paths, gathers allies and supplies, breaks Grimfang's anchors and decides how the Hope Gem will shape the ending. The campaign remains setting-neutral and was built entirely from editable Game Maker data.

## Battle-map authoring

- Create or open a map in Map Browser and set its engine tag to **Battle**.
- Build terrain, water, bridges, cover, walls and obstacles with the ordinary map tools.
- Choose the map in Game Rules as the default, or from a selected world hexagon's right-click menu.
- The preview uses the project map's actual saved layout. Combat clears editor-placed units and deploys both sides on opposite passable edges.

## Verification performed

- 80 automated domain and simulation tests passed.
- Production build, server-rendered shell and ESLint passed.
- Ten deterministic full Ravenwood campaign simulations produced wins for both Good and Evil within 100 turns.
- The source-free ZIP was extracted into a separate clean folder, installed with zero reported runtime vulnerabilities and returned HTTP 200 with Ravenwood and Help present.
- Package contents were checked to exclude source, test, Git and private fan-project material.

## Known limitations

- This is a Beta Preview, not a finished AAA commercial release.
- Broader human playtesting is still needed to confirm visual quality, accessibility, campaign length and balance across hardware.
- Chrome and Edge on Windows are the supported browsers.
- Initial setup requires internet access to install the local runtime.
- The client build reports a non-blocking large JavaScript chunk advisory.

## Package integrity

- File: `Strategy-RPG-Game-Maker-0.2.0-beta.7.zip`
- Size: 930,323 bytes
- SHA-256: `653EC707D52D96CFB1BF0D67D9965C49F9357A4FF27B0976BA4EF5403A894354`
