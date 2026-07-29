# LA + Orange County Tennis Court Finder — Build 19

## Reliable Show on map

Both **Show on map** buttons now use the same delegated click handler.

- The left result-card button remains functional after the results list is re-rendered.
- The right facility-drawer button closes the drawer before Leaflet recalculates the map size.
- The map flies to the selected court and then locks the exact center at zoom 19.
- The selected court receives the existing focus pulse and detailed satellite overlay.
- A failed map action now restores the button instead of leaving it stuck on **Opening map...**.

## Deploy

Replace the existing root `index.html` with the Build 19 file. The included `courts.csv` is unchanged from the uploaded dataset.
