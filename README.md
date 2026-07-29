# LA Tennis Court Finder — Build 14 clean mapper

Build 14 replaces the corrupted coordinate layer with the mapping workflow from
the last working detector-era release.

## Mapping behavior

- The ten verified embedded coordinates appear immediately.
- Remaining facilities are mapped gradually with the proven two-worker ArcGIS
  address queue.
- Newly resolved pins appear without reloading.
- Clicking **Show on map** gives that facility a priority lookup.
- A facility is never opened until its coordinate passes:
  - Southern California geographic bounds
  - California region validation
  - address-type validation
  - ZIP or city consistency checks
- Failed matches remain unpinned instead of opening an incorrect location.

Build 14 clears old coordinate-cache formats once because the previous release
had accepted corrupted locations and grouped many facilities at an incorrect
point.

## Drawer

The right-hand facility drawer now includes its own **Show on map** button.

## Satellite imagery

The map can zoom to level 19, but imagery is upscaled from native level 17 to
avoid Esri's repeated `Map data not yet available` placeholder at unsupported
native zooms.

## Deploy

Replace the repository root with:

- `index.html`
- `courts.csv`
- `CNAME`
- `.nojekyll`
- `README.md`

Confirm that the loading screen says `Build 14`.
