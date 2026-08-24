# Install and test Strategy RPG Game Maker Beta Preview

## Requirements

- Windows 10 or 11
- Current Chrome or Microsoft Edge
- Current [Node.js LTS](https://nodejs.org/), version 22.13 or newer
- Internet access during the first setup only

## Installation

1. Open the [0.2.0-beta.3 release](https://github.com/MikaelFredman/strategy-rpg-game-maker-alpha/releases/tag/v0.2.0-beta.3).
2. Download `Strategy-RPG-Game-Maker-0.2.0-beta.3.zip`.
3. In File Explorer, right-click the downloaded ZIP and choose **Extract All…**.
4. Extract the complete folder somewhere writable, such as Documents. Do not launch it from inside the ZIP preview.
5. Install Node.js LTS from nodejs.org with the standard choices if `node --version` is unavailable or older than 22.13.
6. Open the extracted folder and double-click `Start Strategy RPG Game Maker Beta.cmd`.
7. Wait while the first-time setup installs the local runtime. The editor normally opens at `http://localhost:3000`.
8. Keep the launcher window open while editing or playing. Close it when finished.

Later starts and ordinary editor/game use work without internet access because the runtime remains in the extracted folder.

## Recommended Ravenwood test

1. Confirm that **Ravenwood Pass** opens and reports 36 × 28.
2. Open **Help & Guide**, then review **Start here**, **Build maps**, **Story & quests** and **Play & simulate**.
3. Zoom, pan and orbit. Hover the Old Raven Inn, Whispering Cavern, Northwatch Tower and Ashen Banner Keep to inspect their landmark information.
4. Select a dirt or stone road mesh. Ctrl/Shift-click two suitable endpoint hexes, right-click and use **Connect first and last selected hex**. Confirm that bends rotate correctly and water crossings receive bridges.
5. Open **Map Browser** and inspect Ravenwood Pass, The Old Raven Inn and Whispering Cavern. Check that each doorway/cave link works in both directions.
6. Choose **Start New Game**. Keep the default human Good side and AI Evil side for the first playthrough.
7. Follow the quest journal: investigate the inn, decide how to use supplies, optionally recover the Hope Gem, cooperate with the militia and defeat Grimfang.
8. Verify that dialogue choices have visible consequences, loose items can be collected/distributed and tactical encounters use the selected battle map.
9. Save a project with **Save Project As…**, reopen it with **Open**, and confirm that maps, links, story and rotations remain intact.
10. Optionally start a second game with all controllers set to AI and watch the spectator simulation. Music starts off and can be enabled with the music icon.

## What to report

For bugs, include the Beta version, Windows/browser version, new or migrated project, exact steps, map and selected hex, expected result, actual result and screenshots when useful.

For Ravenwood balance, include difficulty, winning side, approximate real play time, ending turn, optional objectives completed and encounters that felt too easy, too hard or repetitive.

Use the [structured issue forms](https://github.com/MikaelFredman/strategy-rpg-game-maker-alpha/issues/new/choose).

## Troubleshooting

- **Node.js missing:** install current Node.js LTS, close the launcher and try again.
- **Runtime installation fails:** confirm internet access, then rerun the launcher from the extracted folder.
- **Browser does not open:** keep the launcher running and manually open `http://localhost:3000` in Chrome or Edge.
- **Address already in use:** close an older Strategy RPG launcher or another local service using port 3000.
- **Old Ravenwood content appears:** open Map Browser and choose **Load demo project** after saving anything you want to keep.
- **Blank or stale page:** press Ctrl+F5 once while the launcher is running.

Keep backup copies of important projects. This remains a Beta Preview and migrations may change.

