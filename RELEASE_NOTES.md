# Release notes — 0.2.0-beta.3

Released: 24 August 2026

## Highlights

- Ravenwood Pass is now a complete editable three-map reference campaign.
- Smart Route Builder creates continuous roads, chooses bend variants and inserts bridges across water.
- Quest Journal shows prioritized objectives, descriptions and recommended next actions, with later acts revealed through prerequisites.
- Dialogue events are presented sequentially so an unanswered conversation cannot be replaced by another event.
- AI rotates limited formation activations fairly, plans toward visible strategic objectives through fog and follows story targets through linked maps.
- Wood-floor interiors support characters and combat correctly.
- Built-in Help & Guide documents seamless routes, quest sequencing and Ravenwood play.

## Ravenwood campaign

The Wardens begin on the western road. Players may search the Old Raven Inn, explore the optional Whispering Cavern, recover useful equipment and consumables, meet Alden Reed's militia and prepare for the assault on Grimfang at Ashen Banner Keep. Choices can change supplies, mana or temporary combat strength.

Ravenwood is setting-neutral and may be inspected and modified as a Game Maker example.

## Verification performed

- 71 automated domain and simulation tests passed.
- Production build, server-rendered shell and lint passed.
- Ten deterministic Ravenwood skirmish simulations produced victories for both Good and Evil within 100 turns.
- Additional full-project simulations produced both Good and Evil campaign victories.
- 200 × 200 and diagnostic 512 × 512 map performance tests passed without excessive memory use.
- The source-free package was extracted separately, installed with zero reported runtime vulnerabilities and returned HTTP 200.

## Known limitations

- This is a Beta Preview, not a finished AAA commercial release.
- Broader human playtesting is still needed to confirm visual quality, accessibility, campaign length and balance across hardware.
- Chrome and Edge on Windows are the supported browsers.
- Initial setup requires internet access to install the local runtime.
- The client build reports a non-blocking large JavaScript chunk advisory.

## Package integrity

- File: `Strategy-RPG-Game-Maker-0.2.0-beta.3.zip`
- Size: 902,685 bytes
- SHA-256: `A58637C35992BBEBB48337E55C26B0A48CD54AF222B335086431F0C1B2FE9957`

