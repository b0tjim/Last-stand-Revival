# Last Stand: Revival

A top-down zombie survival browser game built entirely in HTML5 and vanilla JavaScript — no frameworks, no dependencies. Loot crates, fight zombies, and extract before you're overrun.

## Gameplay

- Navigate through multiple maps: Warehouse, Office Complex, Shopping Mall, Parking Garage, Apartment Building
- Loot randomized crates and storage containers for weapons and supplies
- Fight off zombies that spawn on timers from set spawn points
- Reach the extraction zone to advance to the next map
- Visit the shop between maps to spend your wallet on better gear and health items
- Health and inventory persist across maps — manage your resources carefully

## Features

- **A\* Pathfinding** — zombies navigate obstacles intelligently to find the player
- **Weapon system** — melee weapons and firearms, each with unique stats, magazine sizes, and reload times
- **Randomized loot tables** — crates contain different items each run
- **Multiple maps** — 5 unique environments with different layouts and obstacle configurations
- **Shop system** — spend extracted loot on weapons and health between maps
- **Sound effects** — gunshots, melee, looting, zombie audio, and background music
- **Optimized collision detection** — AABB pre-check + spatial culling for smooth performance

## Controls

| Input | Action |
|-------|--------|
| WASD / Arrow Keys | Move |
| Mouse | Aim |
| Left Click | Attack / Shoot |
| R | Reload |
| 1–4 | Switch weapons |
| E | Loot (near container) |
| F | Interact |

## Setup

1. Clone or download the repo
2. Create a `sounds/` folder in the same directory as `last_stand_revival.html`
3. Add the required MP3 files (see below)
4. Open `last_stand_revival.html` in a browser (Chrome recommended)

### Required Sound Files

Place these MP3s in a `sounds/` folder:

```
sounds/
├── punch.mp3
├── melee.mp3
├── pistol.mp3
├── shotgun.mp3
├── smg.mp3
├── reload.mp3
├── looting.mp3
├── zombie1.mp3
├── zombie2.mp3
├── zombie3.mp3
├── zombie4.mp3
├── zombie5.mp3
└── background.mp3
```

The game runs without sounds if the folder is missing — you'll just see console errors.

## File Structure

```
last-stand-revival/
├── last_stand_revival.html   # Entire game (~3,300 lines)
├── sounds/                   # Audio files (not included)
└── README.md
```

## Tech Stack

- Pure HTML5 / CSS / JavaScript
- HTML5 Canvas for rendering
- Web Audio API for sound
- No external libraries or frameworks

## Troubleshooting

**Sounds not playing** — check that file names in `sounds/` match exactly (case-sensitive) and click the page once to unblock browser autoplay.

**Performance issues** — close other tabs, ensure hardware acceleration is enabled in browser settings.
