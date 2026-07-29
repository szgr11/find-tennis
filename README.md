# LA + Orange County Tennis Court Finder — Build 18

## Direct Show on map

**Show on map** no longer waits for a marker-cluster callback. It now:

1. closes the list and facility drawer;
2. calls Leaflet `setView` directly;
3. centers the selected facility at zoom 19;
4. briefly highlights the facility;
5. requests a 1500-1800 pixel ArcGIS satellite export around the court.

Standard satellite tiles remain visible if the detailed export is unavailable.

## Orange County expansion

Added 28 official Orange County facilities across Anaheim, Brea,
Buena Park, Fountain Valley, Laguna Niguel, Irvine, Huntington Beach, Costa
Mesa, Newport Beach, Fullerton, Tustin, and Mission Viejo.

The combined dataset now contains 193 facilities.

## View controls

- **Fit to view** fits all currently filtered mapped facilities.
- **Reset** clears filters, nearby radius, selected facility, and detailed
  imagery, then fits the combined LA and Orange County map.

## Deploy

Replace the repository root with:

- `index.html`
- `courts.csv`
- `CNAME`
- `.nojekyll`
- `README.md`

Confirm the loading screen says `Build 18`.
