# Bloxxer

A pixel-art puzzle platformer about a tiny knight and a lot of crates. Carry them, throw them, push them and stack them to climb your way out of 15 dungeon rooms full of pressure plates, timed gates, arrow traps, crumbling floors, springs, conveyor belts and the things that live down there.

The whole game is one HTML file with no build step and no dependencies. Open `index.html` in a browser to play. The pixel fonts load from Google Fonts when you're online and fall back to a system monospace font offline.

## Controls

| Key | Action |
| --- | --- |
| ← → (or A D) | Move |
| W (or ↑) | Jump |
| Space | Grab / throw |
| S (or ↓) | Put down |
| Shift | Shield bash |
| R | Retry the level |
| Esc | Back to the title screen |

Jump, grab, put down and bash can be changed from the settings on the title screen. Progress, deaths and time are saved in the browser.

## Under the hood

- Canvas 2D at 320×192 with 16px tiles, scaled up with pixel-perfect rendering
- Sprites, tiles and torch lighting are generated in code
- Fixed 60 Hz simulation
- Sound effects and the soundtrack are synthesized live with the Web Audio API. There are no audio files.
