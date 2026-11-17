<p align="center">

[Home](../README.md) · [Chomp](chomp.md) · [Sky Glide](sky-glide.md) · [Sunset Sprint](sunset-sprint.md) · **Casino Land**

</p>

---

# Casino Land

Three casino table games in one page: **Roulette**, **Blackjack** and **Texas Hold'em**.

> **Play money only.** There's no real-money gambling and nothing to buy.

**File:** [`casino-land.html`](../casino-land.html) (about 3.4 MB, fonts and sounds built in)

## Tables

| Table | Rules |
| --- | --- |
| **Roulette** | European single zero · $1 minimum · $5,000 limit |
| **Blackjack** | Blackjack pays 3:2 · dealer stands on soft 17 · insurance, double, split and surrender |
| **Hold'em Poker** | No-limit · six seats · blinds $5 / $10 |

You start with a **$10,000** bankroll. If your balance drops below $10, you can claim a free **$1,000** comp from the lobby.

## Controls

Everything works with the mouse or touch. Keyboard shortcuts:

| Where | Keys |
| --- | --- |
| Lobby | `1` `2` `3` open a table · `S` stats · `O` settings |
| Roulette | `Space` spin · `Backspace` undo · `C` clear · `D` double bets · `R` rebet · `1`–`6` pick a chip value |
| Blackjack | `Space` deal · `H` hit · `S` stand · `D` double · `P` split · `R` surrender · `?` hint · `I` / `N` insurance yes / no |
| Hold'em | `Enter` sit down · `F` fold · `C` check / call · `R` raise |
| Anywhere | `F1` help · `Esc` back · `F11` fullscreen |

## Notes

- Your bankroll, lifetime stats per game and settings are saved in your browser (`localStorage` key `casino-land.save.v1`). **Settings → Reset bankroll** starts over.
- Cards, chips and tables are drawn in code, and the sounds are generated in code too, so nothing loads from the network.
- Embedded fonts (*Cinzel Decorative*, *Playfair Display SC*, *Lato*) are used under the SIL Open Font License 1.1.
