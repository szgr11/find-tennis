# LA + Orange County Tennis Court Finder — Build 23

## Quarter-mile court focus

**Show on map** now frames an approximately **1/4 mile by 1/4 mile** ground-distance area around the selected court.

The responsive `fitBounds` behavior remains in place, so desktop and mobile show comparable real-world coverage even though their screen shapes differ.

## Detailed imagery

The high-resolution ArcGIS satellite export still covers the full visible map after the tighter viewport settles.

## Mobile accessibility

Build 22's mobile accessibility improvements are retained, including 44-pixel touch targets, dialog semantics, focus trapping, focus return, visible keyboard focus, reduced-motion support, and no horizontal overflow at 320- and 390-pixel widths.

## Deploy

Replace the repository root with:

- `index.html`
- `courts.csv`
- `README.md`
- `CNAME` and `.nojekyll` if already used by the deployment

Confirm the loading screen says `Build 23`.
