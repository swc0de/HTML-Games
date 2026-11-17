<p align="center">

[Home](../README.md) · [Chomp](chomp.md) · **Sky Glide** · [Sunset Sprint](sunset-sprint.md) · [Casino Land](casino-land.md)

</p>

---

# Sky Glide

A one-button flying game. Keep your flyer in the air and steer it through the gaps between the columns.

**File:** [`sky-glide.html`](../sky-glide.html) (about 94 KB, art built in)

## Gameplay

- Gravity pulls you down all the time. Each tap gives you a lift.
- Fly through the gaps between pairs of columns. You score a point for each pair you pass.
- Hitting a column or the ground ends the run.
- The hitbox is slightly smaller than the sprite, so near misses count.

## Controls

| Action | Keyboard | Mouse / Touch |
| --- | --- | --- |
| Flap / start / retry | Space or Up arrow | Click or tap anywhere |

## Notes

- Your best score is saved in your browser (`localStorage` key `skyglide_best`).
- The game is built for portrait screens. On wider windows it shows more of the world rather than stretching the picture.
- All art is built into the file, so it works offline.
