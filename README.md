# LA Tennis Court Finder — Build 17 map focus

Build 17 restores **Show on map** as a close, clear map-view action.

## Show on map

Selecting **Show on map** from either the court list or facility drawer now:

1. closes the court-list sheet;
2. closes the facility drawer;
3. expands the map to its full available area;
4. zooms directly to the facility at zoom 18 on small phones and 18.5 on
   larger screens;
5. briefly highlights the selected pin and displays the facility name.

Clicking the colored map pin still opens the complete facility-details drawer.

## Clearer imagery

- Satellite imagery receives a subtle contrast and saturation enhancement.
- The map supports half-step zoom levels.
- The facility photo uses a closer geographic crop and a 1000 × 570 export.

## Preserved behavior

- Desktop layout remains unchanged.
- Mobile court-list and facility bottom sheets remain available.
- Orange, blue, and purple category clusters remain intact.
- Weather planner and Google Maps activity link remain intact.
- Background facility mapping remains intact.

## Deploy

Replace the repository root with:

- `index.html`
- `courts.csv`
- `CNAME`
- `.nojekyll`
- `README.md`

Confirm the loading screen says `Build 17`.
