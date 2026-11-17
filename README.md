# HTML Games

<p align="center">

[Chomp](#chomp) · [Sky Glide](#sky-glide) · [Sunset Sprint](#sunset-sprint) · [Casino Land](#casino-land)

</p>

Four browser games. Each one is a single HTML file with no build step and nothing to install.

| Game | File | What it is |
| --- | --- | --- |
| [Chomp](#chomp) | [`chomp.html`](chomp.html) | Maze game: eat every pellet and avoid the four ghosts |
| [Sky Glide](#sky-glide) | [`sky-glide.html`](sky-glide.html) | One-button flyer: tap to fly through the gaps between columns |
| [Sunset Sprint](#sunset-sprint) | [`sunset-sprint.html`](sunset-sprint.html) | Pseudo-3D road racer: three laps against the clock |
| [Casino Land](#casino-land) | [`casino-land.html`](casino-land.html) | Roulette, blackjack and Texas Hold'em for play money |

### How to play

Download a file and open it in any modern browser, or serve the folder locally:

```bash
python3 -m http.server 8000
```

Then go to `http://localhost:8000/` and pick a game.

High scores and saves stay in your browser's `localStorage`. They don't leave your machine.

---

## Chomp

A small maze game drawn in chunky pixel art. Eat every pellet to clear the level while four ghosts chase you.

**File:** [`chomp.html`](chomp.html) (about 20 KB)

### Gameplay

- Eat every pellet in the maze to clear the level. Each pellet is worth **10** points.
- The four flashing **power pellets** are worth **50** points and turn the ghosts blue for a few seconds. While they're blue you can eat them for **200, 400, 800 and 1600** points in a row.
- The ghosts take turns roaming to their corners and then chasing you, and each one hunts in its own way.
- The tunnels at the sides wrap around to the other side, and the ghosts slow down inside them.
- You start with **3 lives**. On each new level you and the ghosts get faster and the blue time gets shorter.

### Controls

| Action | Keyboard | Touch |
| --- | --- | --- |
| Move | Arrow keys or WASD | Swipe on the maze, or use the on-screen D-pad |
| Play again after Game Over | Space or Enter | Tap the maze |

### Notes

- Your high score is saved in your browser (`localStorage` key `chomp-best`).
- The *Press Start 2P* font loads from Google Fonts. Offline, the game falls back to a monospace font.
- On narrow screens the score panel moves below the maze.

<p align="right"><a href="#html-games">↑ Back to top</a></p>

---

## Sky Glide

A one-button flying game. Keep your flyer in the air and steer it through the gaps between the columns.

**File:** [`sky-glide.html`](sky-glide.html) (about 94 KB, art built in)

### Gameplay

- Gravity pulls you down all the time. Each tap gives you a lift.
- Fly through the gaps between pairs of columns. You score a point for each pair you pass.
- Hitting a column or the ground ends the run.
- The hitbox is slightly smaller than the sprite, so near misses count.

### Controls

| Action | Keyboard | Mouse / Touch |
| --- | --- | --- |
| Flap / start / retry | Space or Up arrow | Click or tap anywhere |

### Notes

- Your best score is saved in your browser (`localStorage` key `skyglide_best`).
- The game is built for portrait screens. On wider windows it shows more of the world rather than stretching the picture.
- All art is built into the file, so it works offline.

<p align="right"><a href="#html-games">↑ Back to top</a></p>

---

## Sunset Sprint

A pseudo-3D road racer. Race three laps against the clock and get past a field of rival cars.

**File:** [`sunset-sprint.html`](sunset-sprint.html) (about 9 MB, all art built in)

### Gameplay

Before each race you pick a circuit and how tough the rivals are. Finish three laps before time runs out.

#### Circuits

| Circuit | Character |
| --- | --- |
| **Sunset Coast** | Seaside at dusk, fast sweeping bends |
| **Jungle Run** | Dirt road, river bridge, tight turns |
| **Giza Desert** | Long straights, dune crests, pyramids |

#### Rivals

| Difficulty | Field | Score multiplier |
| --- | --- | --- |
| **Easy** | 10 slow rivals that move aside | x1 |
| **Normal** | 14 rivals at mixed speeds | x1.5 |
| **Hard** | 20 fast rivals that block you | x2 |

### Controls

| Action | Keyboard | Touch |
| --- | --- | --- |
| Gas | Up arrow, W or Space | Hold **Gas** |
| Brake | Down arrow or S | **Brake** button |
| Steer | Left / Right arrows or A / D | ◀ ▶ buttons |
| Pause | P | |
| Fullscreen | F | |
| Leave fullscreen | Esc | |

### Notes

- Best scores and your last choices are saved in your browser (`localStorage`).
- The display fonts (*Bungee*, *Chakra Petch*) load from Google Fonts. Offline, it falls back to system fonts.

<p align="right"><a href="#html-games">↑ Back to top</a></p>

---

## Casino Land

Three casino table games in one page: **Roulette**, **Blackjack** and **Texas Hold'em**.

> **Play money only.** There's no real-money gambling and nothing to buy.

**File:** [`casino-land.html`](casino-land.html) (about 3.4 MB, fonts and sounds built in)

### Tables

| Table | Rules |
| --- | --- |
| **Roulette** | European single zero · $1 minimum · $5,000 limit |
| **Blackjack** | Blackjack pays 3:2 · dealer stands on soft 17 · insurance, double, split and surrender |
| **Hold'em Poker** | No-limit · six seats · blinds $5 / $10 |

You start with a **$10,000** bankroll. If your balance drops below $10, you can claim a free **$1,000** comp from the lobby.

### Controls

Everything works with the mouse or touch. Keyboard shortcuts:

| Where | Keys |
| --- | --- |
| Lobby | `1` `2` `3` open a table · `S` stats · `O` settings |
| Roulette | `Space` spin · `Backspace` undo · `C` clear · `D` double bets · `R` rebet · `1`–`6` pick a chip value |
| Blackjack | `Space` deal · `H` hit · `S` stand · `D` double · `P` split · `R` surrender · `?` hint · `I` / `N` insurance yes / no |
| Hold'em | `Enter` sit down · `F` fold · `C` check / call · `R` raise |
| Anywhere | `F1` help · `Esc` back · `F11` fullscreen |

### Notes

- Your bankroll, lifetime stats per game and settings are saved in your browser (`localStorage` key `casino-land.save.v1`). **Settings → Reset bankroll** starts over.
- Cards, chips and tables are drawn in code, and the sounds are generated in code too, so nothing loads from the network.
- Embedded fonts (*Cinzel Decorative*, *Playfair Display SC*, *Lato*) are used under the SIL Open Font License 1.1.

<p align="right"><a href="#html-games">↑ Back to top</a></p>

