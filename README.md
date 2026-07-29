# LA + Orange County Tennis Court Finder — Build 21

## High-resolution court focus

Build 21 improves image quality after **Show on map** zooms to a selected facility.

- Removed the old native-zoom-17 cap that forced Leaflet to stretch blurry satellite tiles.
- The basemap now requests native ArcGIS imagery through zoom 20 and uses retina tiles on high-density displays.
- Selected facilities now focus at zoom 19.
- The detailed satellite export is framed more tightly around the facility and requests an 1800–2048 pixel image at 95% JPEG quality.
- The normal satellite tiles remain available if the detailed export cannot load.
- The Build 20 Show on map repair remains intact for both the left results list and right facility drawer.

## Deploy

Replace the repository root files with:

- `index.html`
- `courts.csv`
- `README.md`

Confirm the loading screen says `Build 21`.
