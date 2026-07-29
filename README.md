# LA + Orange County Tennis Court Finder — Build 22

## Half-mile court focus

**Show on map** now frames an approximately 0.5-mile by 0.5-mile ground-distance area around the selected facility instead of using a fixed zoom level. The visible map may include additional context in one direction depending on screen aspect ratio.

The map repeats the fit after the court list or facility drawer finishes closing, preserving the final view on desktop and mobile.

## High-resolution imagery

The ArcGIS detailed satellite export now uses the full visible map bounds and a responsive 1200–2048 pixel image size. This keeps the entire focused viewport sharp rather than loading only a high-resolution patch around the pin.

## Mobile accessibility

- Mobile controls use 44-pixel minimum touch targets.
- The Courts button is exposed correctly to assistive technology.
- The mobile court browser is announced as a dialog and traps keyboard focus while open.
- Closing the browser returns focus to the Courts button.
- Search and filter controls have accessible labels.
- Map, loading, imagery, and toast status messages are announced.
- Visible keyboard focus outlines and reduced-motion support are included.
- Layout was checked at 320 px and 390 px widths with no horizontal overflow.

## Deploy

Replace the repository root files with:

- `index.html`
- `courts.csv`
- `README.md`

Confirm the loading screen says **Build 22**.
