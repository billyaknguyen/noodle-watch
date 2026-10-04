# NOODLE WATCH — Don't Let Her Eat 🍜

A complete first-person 3D horror/management game in a single `index.html` (Three.js via CDN), ready to upload to itch.io.

## What's in the game

- **First-person controls** — mouse look (pointer lock) + WASD movement, Shift to sprint
- **Two-story house** — bedroom upstairs, staircase, kitchen downstairs, all explorable
- **The Girl (AI NPC)** — starts in her bedroom, periodically sneaks downstairs toward the kitchen. Slow, deliberate, glowing red eyes when she's on the move. If she reaches the ramen on the kitchen table → **GAME OVER**
- **Shock gun** — click to fire. A hit sends her stumbling back to her bedroom. 1.8s recharge to prevent spam (HUD shows charge bar)
- **Math terminal** — equations (+, −, ×) shown in the HUD and on the 3D monitor in your room. Type digits, Backspace to fix, Enter to submit. +100 pts per correct answer
- **HUD** — score, best (saved in localStorage), equation + answer box, gun cooldown, status warnings ("SHE'S DOWNSTAIRS — STOP HER!")
- **Difficulty ramp** — she gets faster and waits less between attempts the longer you survive
- **Horror atmosphere** — fog, flickering kitchen light, film vignette, procedural drone/zap/slurp audio (WebAudio, no files needed)
- **Game over screen** — final score, time survived, restart button

## How to upload to itch.io

1. Go to https://itch.io/game/new (log in if needed)
2. Fill in title, e.g. **"NOODLE WATCH — Don't Let Her Eat"**
3. Under **Uploads**, upload **`noodle-watch-itch.zip`**
4. Check **"This file will be played in the browser"**
5. Set **Embed options → Viewport dimensions** to `960 × 640` (or `1280 × 720`)
6. Set **Kind of project → HTML**
7. Write a short description, add a cover image (screenshot the menu in-game), set visibility, and hit **Save & view page**

Note: the game loads Three.js from a CDN, so it needs internet access when played — fine on itch.io.

## Controls (show these on your itch page)

| Input | Action |
|---|---|
| WASD / arrows | Move |
| Mouse | Look (click START to lock) |
| Left click | Fire shock gun |
| 0–9, Backspace, Enter | Answer math terminal |
| Shift | Sprint |

## Files

- `index.html` — the entire game (single file)
- `../noodle-watch-itch.zip` — the itch.io upload bundle (index.html at zip root, as itch requires)
