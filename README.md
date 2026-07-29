# LA Tennis Court Finder — Build 15 category clusters

Build 15 restores the earlier orange, blue, and purple marker-cluster map.

## Critical mapping fix

The previous build converted blank latitude and longitude strings to numeric
zero and therefore reported every facility as mapped. Build 15 treats blank
coordinates as missing. The map begins with the ten verified facilities and
then adds resolved facilities progressively.

The detector-era coordinate mapper has been restored:

- two background workers;
- exact address lookup followed by facility-name fallback;
- Southern California coordinate validation;
- session and persistent cache support;
- priority lookup when **Show on map** is selected;
- markers appear without reloading.

Only the broken Build 14 cache namespace is removed. Earlier valid coordinate
caches are preserved.

## Map colors

- Orange: pay courts
- Blue: open play
- Purple: clubs

Each category has its own colored cluster layer.

## Typography

- Barlow Condensed: athletic headings
- Manrope: controls, data, buttons, addresses, and list content
- Source Serif 4: limited to loading and descriptive narrative text

## Deploy

Replace the repository root with:

- `index.html`
- `courts.csv`
- `CNAME`
- `.nojekyll`
- `README.md`

Confirm the launch screen says `Build 15`.
