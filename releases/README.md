# Releases — install the track & kart in Assetto Corsa

Everything you need is in this folder. Both files are ready-to-install packages —
no build step, no other files, nothing to download from anywhere else.

| File | What it is | Size |
|---|---|---|
| `lemans_lakeside-R001.acz` | **Le Mans Lakeside** track (Dandenong South VIC) — 581 m, 13 corners | ~37 MB |
| `praga_rtk_lakeside-R001.acz` | **Praga RTK Rental – Lakeside** kart (calibrated to the venue) | ~82 MB |

Both are free for personal use, made by a karter, and not affiliated with the venue.

## Requirements

- **Assetto Corsa** (Steam app 244210)
- **Custom Shaders Patch** (the track's night lighting and the kart use CSP)
- **Content Manager** (optional but easiest — see below)

## Easiest: Content Manager (one drag and drop)

1. Open Content Manager.
2. Drag `lemans_lakeside-R001.acz` onto the window → the track installs.
3. Drag `praga_rtk_lakeside-R001.acz` onto the window → the kart installs.

You're done.

## Manual: copy/paste (no Content Manager)

1. Unzip each `.acz` (it's a normal zip — the extension is just for Content Manager).
   You get one folder per file: `lemans_lakeside/` and `praga_rtk_lakeside/`.
2. Find your AC content folders:
   Steam → right-click Assetto Corsa → **Manage → Browse local files** → `content`.
3. Copy the track folder into `content\tracks\`:
   ```
   ...assettocorsa\content\tracks\lemans_lakeside\
   ```
4. Copy the kart folder into `content\cars\`:
   ```
   ...assettocorsa\content\cars\praga_rtk_lakeside\
   ```
5. There must be **no `data.acd`** inside the kart folder — if one is present, AC loads
   the packed physics instead of the `data/` folder. (It's not in these releases.)

Start the game: the track shows as **Le Mans Lakeside**, the car as
**Praga RTK Rental – Lakeside** (class `kart`).

## In game

- **Steering:** 180° lock-to-lock — set your wheel to ~180–360° rotation if you use one.
- **FFB:** the kart is a rigid chassis with no suspension travel. If it feels jittery,
  lower the FFB gain and leave CSP *Real Feel* off.
- **What to expect:** top speed ~65 km/h (GX270 governor down the straight); single
  speed (centrifugal clutch, no shifting); **rear-only brakes** (brake in a straight line
  and the rear steps out); it should **push** on entry — the chicane / Bus Stop need a lift.
- Target lap: ~34–35 s (the venue's real best is 33.995 s).

## Uninstall

- Track: delete `content\tracks\lemans_lakeside\`
- Kart: delete `content\cars\praga_rtk_lakeside\`

## What's in the packages

- **Track:** full `lemans_lakeside` build — geometry, CC0 textures, kerbs, anti-cut
  blocks, pit lane, CSP night lighting. No satellite imagery (used only as a ruler).
- **Kart:** calibrated rental-kart physics (donor visual model, our `data/`). The
  visual model is a placeholder; the physics is the part that's been tuned to the venue.
