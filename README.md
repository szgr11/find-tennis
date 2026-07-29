# LA Tennis Court Finder — Build 13

This fixes the two Build 12 regressions.

## Slideshow fix

All five aerial images are embedded directly inside `index.html` as compressed
JPEG data. No `assets` folder is required, and the slideshow cannot break
because of an omitted folder or relative path.

The loading screen visibly says:

```text
LA court map · Build 13
```

## Mapping fix

Build 13 restores compatibility with every coordinate-cache key used by the
last working mapper:

- `la-tennis-fast-v1`
- `la-tennis-exact-v1`, `v2`, and `v3`
- `la-tennis-runtime-point-v1`
- `precise-v3`
- `geo`
- Build 12's `la-tennis-coordinate-v3`

Previously mapped facilities therefore reappear immediately in browsers that
used the working version. New mappings are saved in both the new and legacy
formats.

The proven ArcGIS address matcher and two-worker background mapping queue have
also been restored. New dots appear without a page reload.

## Deploy

Upload these four visible files, plus the hidden `.nojekyll`, to the repository
root:

- `index.html`
- `courts.csv`
- `CNAME`
- `README.md`
- `.nojekyll`

No image folder is needed.
