<p align="center">

**Home** · [Chomp](docs/chomp.md) · [Sky Glide](docs/sky-glide.md) · [Sunset Sprint](docs/sunset-sprint.md) · [Casino Land](docs/casino-land.md)

</p>

---

# HTML Games

Four browser games. Each one is a single HTML file with no build step and nothing to install.

| Game | File | What it is |
| --- | --- | --- |
| [Chomp](docs/chomp.md) | [`chomp.html`](chomp.html) | Maze game: eat every pellet and avoid the four ghosts |
| [Sky Glide](docs/sky-glide.md) | [`sky-glide.html`](sky-glide.html) | One-button flyer: tap to fly through the gaps between columns |
| [Sunset Sprint](docs/sunset-sprint.md) | [`sunset-sprint.html`](sunset-sprint.html) | Pseudo-3D road racer: three laps against the clock |
| [Casino Land](docs/casino-land.md) | [`casino-land.html`](casino-land.html) | Roulette, blackjack and Texas Hold'em for play money |

## How to play

Download a file and open it in any modern browser, or serve the folder locally:

```bash
python3 -m http.server 8000
```

Then go to `http://localhost:8000/` and pick a game.

High scores and saves stay in your browser's `localStorage`. They don't leave your machine.
