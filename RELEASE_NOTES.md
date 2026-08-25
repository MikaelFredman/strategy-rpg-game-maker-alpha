# Release notes — 0.2.0-beta.13

Released: 25 August 2026

## Highlights

- Asset Studio's joint-authored animations now drive the corresponding actions in tactical gameplay instead of existing only as editor previews.
- Added protected, copyable preset animation families for unarmed combat, sword, spear, longbow, staff magic, defence and drinking/consumables. Animation chains may contain as many authored poses as the movement needs.
- Equipped weapons and shields attach to the animated hands. The longbow uses a moving two-part string, a visible loaded arrow that follows the drawing hand and a timed release into the projectile flight.
- Ravenwood Pass assigns suitable visual assets, active equipment and animation families to its named heroes and Ashen Banner opponents so the complete runtime path can be tested immediately.
- Tactical faction geography is now consistent: Good deploys on the left/west side and is summarized with green health; Evil deploys on the right/east side and is summarized with red health. This remains true when Evil initiates the encounter.

## Verification performed

- 96 automated domain and simulation tests passed, including a regression in which Evil attacks but still deploys on the Evil side.
- Three rendered-interface tests, production build and ESLint passed.
- Ten deterministic Ravenwood simulations completed within 100 turns and produced victories for both Good and Evil.
- A live River Crossing spectator battle visually confirmed the canonical Good/green/left and Evil/red/right presentation.
- The source-free ZIP was installed in a separate clean folder, audited with zero reported runtime vulnerabilities and returned HTTP 200 with Ravenwood Pass and Help present.

## Known limitations

- This remains a Beta Preview and needs broader human testing of animation quality, accessibility and campaign pacing.
- Chrome and Edge on Windows are the supported browsers.
- Initial setup requires internet access to install the local runtime.
- The production build reports a non-blocking large JavaScript chunk advisory.

## Package integrity

- File: `Strategy-RPG-Game-Maker-0.2.0-beta.13.zip`
- Size: 1,011,784 bytes
- SHA-256: `8B222964282ACF42E91703768BEBE37481189829C4457CA487DEC510153CE868`

Version 0.2.0-beta.12 was an internal release candidate that was rejected during package validation and was never published.

---

# Previous release — 0.2.0-beta.11

Released: 25 August 2026

## Highlights

- Added a unified **Content Studio** for Characters & Creatures, Items & Equipment and reusable Visual Assets.
- Content Studio lists every placed formation across all maps and opens it at the correct map and coordinate for editing.
- Added a lightweight articulated Visual Asset editor with ready-made Humanoid, Quadruped, Winged and Static / Item templates.
- Visual Assets support reusable parts, materials, safe parented joints, smooth quaternion-interpolated poses and up to five poses per action.
- Gameplay-event markers synchronize melee hits, projectile releases and spells with authored movement. Animated visuals can be assigned to characters and static visuals to items.
- Reordered both the sidebar and Project Dashboard to the same authoring sequence: Game Setup & Rules → Maps & Locations → Content Studio → Story, Quests & Dialogues → Validation → Playtest.
- Updated Help & Guide and installation material to explain the unified workflow while keeping appearance separate from gameplay rules internally.

- Tactical Team Summary panels now preserve both complete opening rosters and their opening maximum HP throughout an encounter.
- Fallen characters remain in their original list position at 0 HP, with the complete row shown in red instead of disappearing after the round.

- Strategic AI now estimates route-aware arrival time, projected battle duration and the nearest compatible enemy reinforcement before attacking.
- AI exploits isolated weaker formations when it can finish before support arrives, but consolidates with a compatible same-team force when the opportunity window is unsafe.
- Full groups can combine into a multi-group army of up to four configured group capacities; individual group limits and character identity remain intact.
- Tactical AI no longer spends its only AP on an equivalent positioning move when a clear attack is already available, eliminating the observed circling-without-attacking loop.
- Seeded combat and AI activation ordering use stable game identity rather than random runtime UUID ordering, improving reproducible balancing.

- Standardized camera interaction: left-drag pans, middle-drag rotates around the hex beneath the pointer, wheel zooms and right-click is reserved for Hex Actions.
- Added multi-select Clear tile and reversible Hide/Show tile actions. Hidden tiles are black on every visible side and keep their data for restoration.
- Tactical AI scores hit-adjusted damage, target resistance, kill opportunity, target threat, combat role and defence timing.
- Casters, ranged units, guardians, brutes, skirmishers and beasts use distinct tactics. Magical beasts no longer automatically cast wizard spells.
- AI uses useful health and mana potions as real AP actions; charges decrease and the final charge removes the item. Empty or unnecessary potions are rejected.
- A reusable 100-fight tactical balance harness now reports outcomes, rounds, action mix, consumable use and character matchups.

- Fixed AI spectator rounds overwriting arrows, fireballs and damage labels before their animation timeline completed. A resolved round now remains visible for the full effect window.
- Tactical formations advance sequentially in 0.5-second-per-hex frames. One character completes its route before the next character begins.
- Equipped bows now provide four-hex attacks and ranged AI positioning to any compatible character; equipped spears provide two-hex reach. Spell range remains four hexes.
- Authoritative battle events preserve both movement routes and tactical effects for diagnostics and future network presentation.
- Tactical movement now follows the resolved hex route one tile at a time at the same 0.5-second cadence used on world maps.
- Sword/axe swings, spear/lance thrusts, bow releases, unarmed strikes and staff-conjuring gestures originate at the acting figure before projectile or impact effects resolve.
- Character Editor supports optional weapon-specific animation chains with at most five steps. Authors can copy the base mesh pose to step 1, copy the previous step forward or use the local Copy/Paste pose clipboard.
- Item Designer explicitly associates a weapon with its fight-animation family, including custom spears and staffs.
- **Project Dashboard** provides project metrics, readiness and a recommended next action using the same authoring order as the sidebar.
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

- 92 automated domain and simulation tests passed, including visual-asset serialization, smooth pose interpolation, persistent casualty roster/max-HP, isolated attack-window, defensive consolidation and twelve-character army-formation regressions.
- One hundred tactical fights all resolved: 57 Good wins and 43 Evil wins, with no draws and a 4.08-round average.
- Ten complete Ravenwood simulations produced eight Good and two Evil victories, all within 100 turns.
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

- File: `Strategy-RPG-Game-Maker-0.2.0-beta.11.zip`
- Size: 983,862 bytes
- SHA-256: `13DF3982A39D187CF8A479C39CFD2421F069D628621551C67B17D2D5920935A5`
