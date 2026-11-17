<p align="center">

[Home](../README.md) · **Chomp** · [Sky Glide](sky-glide.md) · [Sunset Sprint](sunset-sprint.md) · [Casino Land](casino-land.md)

</p>

---

# Chomp

A small maze game drawn in chunky pixel art. Eat every pellet to clear the level while four ghosts chase you.

**File:** [`chomp.html`](../chomp.html) (about 20 KB)

## Gameplay

- Eat every pellet in the maze to clear the level. Each pellet is worth **10** points.
- The four flashing **power pellets** are worth **50** points and turn the ghosts blue for a few seconds. While they're blue you can eat them for **200, 400, 800 and 1600** points in a row.
- The ghosts take turns roaming to their corners and then chasing you, and each one hunts in its own way.
- The tunnels at the sides wrap around to the other side, and the ghosts slow down inside them.
- You start with **3 lives**. On each new level you and the ghosts get faster and the blue time gets shorter.

## Controls

| Action | Keyboard | Touch |
| --- | --- | --- |
| Move | Arrow keys or WASD | Swipe on the maze, or use the on-screen D-pad |
| Play again after Game Over | Space or Enter | Tap the maze |

## Notes

- Your high score is saved in your browser (`localStorage` key `chomp-best`).
- The *Press Start 2P* font loads from Google Fonts. Offline, the game falls back to a monospace font.
- On narrow screens the score panel moves below the maze.
