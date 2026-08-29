# Install and test Strategy RPG Game Maker Beta Preview

## Requirements

- Windows 10 or 11
- Current Chrome or Microsoft Edge
- Current [Node.js LTS](https://nodejs.org/), version 22.13 or newer
- Internet access during the first setup only

## Installation

1. Open the public [`0.2.0-beta.15` package](downloads/Strategy-RPG-Game-Maker-0.2.0-beta.15.zip).
2. Download `Strategy-RPG-Game-Maker-0.2.0-beta.15.zip` using GitHub's download button.
3. In File Explorer, right-click the downloaded ZIP and choose **Extract All…**.
4. Extract the complete folder somewhere writable, such as Documents. Do not launch it from inside the ZIP preview.
5. Install Node.js LTS from nodejs.org with the standard choices if `node --version` is unavailable or older than 22.13.
6. Open the extracted folder and double-click `Start Strategy RPG Game Maker Beta.cmd`.
7. Wait while the first-time setup installs the local runtime. The editor normally opens at `http://localhost:3000`.
8. Keep the launcher window open while editing or playing. Close it when finished.

Later starts and ordinary editor/game use work without internet access because the runtime remains in the extracted folder.

## Recommended Ravenwood test

1. Confirm that **Ravenwood Pass** opens and reports 36 × 28.
2. Open **Project Dashboard** to see the complete Game Setup & Rules → Maps & Locations → Content Studio → Story, Quests & Dialogues workflow, then use **Help & Guide** for detailed instructions.
3. Open **Content Studio**. Confirm that Characters & Creatures lists formations from all project maps, Items & Equipment opens Item Designer and Visual Assets opens the articulated visual editor.
4. Zoom with the wheel, pan with left-drag and orbit around the pointed hex with middle-drag. Right-click must open Hex Actions without rotating the map. Hover the Old Raven Inn, Whispering Cavern, Northwatch Tower and Ashen Banner Keep to inspect their landmark information.
5. Select a dirt or stone road mesh. Ctrl/Shift-click two suitable endpoint hexes, right-click and use **Connect first and last selected hex**. Confirm that bends rotate correctly and water crossings receive bridges.
6. Open **Map Browser** and inspect Ravenwood Pass, The Old Raven Inn and Whispering Cavern. Check that each doorway/cave link works in both directions.
7. Choose **Start New Game**. Keep the default human Good side and AI Evil side for the first playthrough.
8. Complete the opening dialogue, left-click the Wardens and confirm highlighted destinations appear. Right-click one, choose **Move to this hex** and confirm the formation travels one tile at a time to that destination.
9. Follow the Broken Oath quest journal: investigate the inn, choose hero paths, decide how to use supplies and the Hope Gem, cooperate with the militia, break the two anchors and confront Grimfang.
10. Verify that dialogue choices have visible consequences, loose items can be collected/distributed and the ending reflects optional objectives.
11. Select one or more world hexes, right-click, change **Battle map for selection**, inspect the miniature preview and then use **Apply battle map**. The selection alone must not alter the assigned map.
12. In Map Browser, create a tactical map from a battle template—or retag a custom small map as **Battle**—paint its terrain and obstacles, and confirm that it appears with its actual layout in the same preview selector.
13. Right-click an occupied editor hex, choose **Edit character…**, expand **Optional fight animations**, copy the base mesh pose to step 1 and copy the previous pose into a later step. Save and verify the custom chain survives reopening the project.
14. In a tactical battle, verify sequential half-second tile-by-tile movement and singular initiative actions: one character is marked in gold, completes one action with its animation and foreground sound, and then yields to the next available character. Higher-level/quick-race characters may act again through surplus AP. Confirm that damage flashes the target row red once, Good deploys left with green health and Evil deploys right with red health.
15. In the panels below the tactical map, confirm that each side's opening maximum HP remains fixed after a casualty and that the fallen character stays in the list at 0 HP with red row text.
16. In an AI-only world simulation, inspect Latest world event for decisions to strike before reinforcements arrive, consolidate against a reinforced enemy or form a multi-group army.
17. Save a project with **Save Project As…**, reopen it with **Open**, and confirm that maps, links, story, rotations, Visual Assets and animation poses remain intact.
18. Optionally start a second game with all controllers set to AI and watch the spectator simulation. Music starts off and can be enabled with the music icon.
19. In editor mode, right-click a tile and verify Clear tile plus the alternating Hide tile/Show tile action. Hide must make the complete tile black; Show must restore its authored content.

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

