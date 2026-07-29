# LA Tennis Court Finder — mandatory launch calibration

## Launch behavior

Every new page launch opens a five-location detector setup.

For each location:

1. Pan or zoom to the visible courts.
2. Place one pin at the center of every individual tennis court.
3. Complete all five locations.

The pin sets are converted into appearance, scale, orientation, and approximate
court-layout references. Facility address mapping continues while the user
works through the five locations.

Choosing **Skip setup and disable court detection** opens the site but disables
court-layout detection for that visit.

## Public feedback

The former manual-correction interface has been removed. After a layout is
detected, the only public detector-feedback action is **Report false positive**.
It opens a prefilled GitHub Issue for review.

## Map details

Facility details now open in a side drawer on desktop and a bottom drawer on
mobile. The map physically resizes, so the card does not cover the courts.

## Detection progress

Court detection uses a compact status pill near the lower edge of the map,
with a thin progress line and a small cancel control.

## Deploy

Upload all files to the repository root and commit to `main`.

GitHub Pages:

- Source: Deploy from a branch
- Branch: main
- Folder: / (root)
