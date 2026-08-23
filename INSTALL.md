# Install and start the Windows alpha

## What you need

- Windows 10 or 11
- Current Chrome or Microsoft Edge
- Current [Node.js LTS](https://nodejs.org/) release; the runtime requires Node.js 22.13 or newer
- Internet access during the first setup only

## Installation

1. Open the [Alpha 2 release](https://github.com/MikaelFredman/strategy-rpg-game-maker-alpha/releases/tag/v0.1.0-alpha.2).
2. Download `Strategy-RPG-Game-Maker-0.1.0-alpha.2.zip`.
3. In File Explorer, right-click the downloaded ZIP and choose **Extract All…**.
4. Extract the complete folder somewhere writable, such as your Documents folder. Do not launch it from inside the ZIP preview.
5. Install Node.js LTS from nodejs.org with its standard installation choices if it is not already installed.
6. Open the extracted folder and double-click `Start Strategy RPG Game Maker Alpha.cmd`.
7. Wait while the first-time setup installs the local runtime. The editor then opens at `http://localhost:3000`.
8. Keep the launcher window open while editing or playing. Close it when finished.

Later starts and normal editor use can work without internet access.

## First test

1. Confirm that **Ravenwood Pass** is visible.
2. Open **Help & Guide** and read **Start here**, **Build maps**, and **Play & simulate**.
3. Select a rotatable mesh and a hex, then right-click it. Confirm that **Rotate +60°** cycles through stored values 0–5 and that all six exact angles are available.
4. Select **Start New Game** and start the ready-made two-team simulation.
5. Save a test project with **Save Project As…**, then reopen it with **Open Project**.

## Troubleshooting

- If the launcher reports that Node.js is missing, install the current Node.js LTS release and start again.
- If setup cannot download packages, check the internet connection and retry.
- If the browser does not open, keep the launcher running and manually open `http://localhost:3000` in Chrome or Edge.
- If the address is already in use, close another local server or old Strategy RPG launcher before starting again.
- Keep backups: alpha project formats may change.

Report reproducible problems through the [structured issue forms](https://github.com/MikaelFredman/strategy-rpg-game-maker-alpha/issues/new/choose). Include the alpha version, Windows version, browser, exact steps, expected result, actual result, and screenshots when useful.

