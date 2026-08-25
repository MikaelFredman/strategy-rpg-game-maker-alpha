# Strategy RPG Game Maker - Beta Preview Community

This repository is the public download, testing and feedback hub for **Strategy RPG Game Maker Beta Preview 0.2.0-beta.11**.

Strategy RPG Game Maker is an offline-first, board-game-like 3D hex editor and game-authoring system for turn-based Strategy RPGs. It combines map building, linked world/interior/dungeon maps, teams, characters, groups and armies, items and equipment, dialogue and quests, tactical battle maps, configurable AI, victory rules and spectator simulation.

## Current release

- [Download Strategy RPG Game Maker 0.2.0-beta.11](downloads/Strategy-RPG-Game-Maker-0.2.0-beta.11.zip)
- Read [RELEASE_NOTES.md](RELEASE_NOTES.md) before testing.
- Follow [INSTALL.md](INSTALL.md) for installation and the recommended first test.
- Keep backup copies of projects that matter to you. Project conversion exists, but this is still a preview build.

The commercial engine source code is kept in a separate private repository. This public repository contains the distributable runtime, documentation, issue forms and community material.

## Included test game: Ravenwood Pass

Ravenwood Pass is an editable, setting-neutral reference campaign built entirely with the same Game Maker tools available to users.

- A 36 × 28 outdoor world map with mountains, forests, a continuous river, connected roads and bridges.
- The linked 20 × 15 **Old Raven Inn** interior and **Whispering Cavern** dungeon.
- An opening Broken Oath story, prerequisite-driven quest journal and editable dialogue choices that carry consequences into later events.
- Four permanent hero-progression choices, 18 campaign items, staged encounters and complete, costly or evil endings.
- The Wardens of Ravenwood, allied militia, wildlife, patrols, a cavern guardian and Grimfang's Ashen Banner forces.
- Optional exploration, equipment and consumables, tactical battles and asymmetric Good/Evil victory outcomes.
- Ten generic tactical arenas plus support for creating, tagging, previewing and assigning your own battle maps.
- A guided Project Dashboard and matching sidebar that follow Game Setup & Rules → Maps & Locations → Content Studio → Story, Quests & Dialogues → Validation → Playtest.
- A unified Content Studio for project-wide Characters & Creatures, Items & Equipment and reusable Visual Assets.
- A lightweight articulated Visual Asset editor with Humanoid, Quadruped, Winged and Static / Item templates, materials, joints, smooth pose animation and gameplay-event timing.
- Editable starting templates for outdoor regions, strongholds, caves and five common tactical battle layouts.
- Weapon-aware tactical gestures for swords, spears, bows, staffs and unarmed attacks, with optional five-step pose chains in Character Editor.
- Sequential half-second tactical movement: one character completes its route before the next begins, followed by protected effect windows for visible arrows, fireballs and damage text.
- Persistent tactical casualty summaries: each side keeps its complete opening roster and opening maximum HP; fallen characters remain visible at 0 HP with red row text.
- Standard camera controls: left-drag pans, middle-drag orbits around the pointed hex, wheel zooms and right-click opens Hex Actions.
- Tactical role AI evaluates expected effect, resistances, target threat, defence timing and useful potion charges instead of relying on one generic attack rule.
- Strategic AI compares route time, projected battle duration and enemy reinforcement time. It attacks exposed weaker formations, consolidates when the window is unsafe and can form multi-group armies.

The intended human play session is approximately 40–70 minutes, but this estimate is part of the beta test and should be reported if it differs substantially.

## Install on Windows

1. Download [`Strategy-RPG-Game-Maker-0.2.0-beta.11.zip`](downloads/Strategy-RPG-Game-Maker-0.2.0-beta.11.zip) from this repository.
2. Right-click the ZIP and choose **Extract All…**. Do not run it from inside the ZIP preview.
3. Install the current [Node.js LTS](https://nodejs.org/) if Node.js is not already installed. Node.js 22.13 or newer is required.
4. Open the extracted folder and double-click **Start Strategy RPG Game Maker Beta.cmd**.
5. Keep the launcher window open. The first start installs the local runtime and therefore needs internet access; later starts and ordinary editing/play work offline.

The editor normally opens at `http://localhost:3000` in Chrome or Microsoft Edge. Built-in **Help & Guide** is available in both editing and simulation mode.

## Give feedback

- Use **Bug report** for reproducible failures.
- Use **AI or balance problem** when AI stalls, loops, ignores an objective or produces consistently unfair results.
- Use **Feature request** for workflow or gameplay improvements.
- Use **Discussions** for questions, design ideas, screenshots and showcases.

Please search existing reports first. Include version `0.2.0-beta.11`, Windows version, browser, map name/size, exact reproduction steps and screenshots when useful. For Ravenwood balance feedback, also include chosen difficulty, winning side, approximate play time and the turn on which the game ended.

## Supported environment and preview limits

- Windows 10 or 11.
- Current Chrome or Microsoft Edge.
- Desktop/laptop layout; mobile and non-Chromium browsers are not supported yet.
- First setup requires internet; normal use is offline afterwards.
- Visual assets, balance and save migrations may change during the preview.
- This release passed 92 automated domain tests, build, lint, server-rendering, balance and large-map performance checks. The source-free package was also installed separately, audited with zero reported vulnerabilities and smoke-tested over HTTP. Broader human visual and interaction testing is still needed.

## Sharing created games

Only share projects and media that you created or have permission to distribute. Do not upload executables or copyrighted third-party worlds, names, music, artwork or stories without permission. Public project-file sharing will be expanded only after validation and moderation are ready.

See [CONTRIBUTING.md](CONTRIBUTING.md), [COMMUNITY_GUIDELINES.md](COMMUNITY_GUIDELINES.md) and [SECURITY.md](SECURITY.md) before participating.

