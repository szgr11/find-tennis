# LA Tennis Court Finder

GitHub Pages package for `find.tenniscourt.io`.

## Fixes in this build

- Every facility card has a **Show on map** button.
- The 10 embedded coordinates appear immediately.
- Remaining facilities are address-matched gradually in the background.
- Successful background matches appear as dots without reloading.
- Background matches are stored only for the browser session.
- Clicking **Show on map** gives an unmapped facility a priority lookup.
- Nearby search cancels an unrelated court-layout attempt.
- The scale/rotation line-ratio scan has a strict CPU deadline and cannot
  remain indefinitely at 89%.
- Dark interface retained with a tennis-ball lime and court-green theme.
- Clearer primary actions and mapping-status feedback.

## Deploy

Upload all files to the GitHub repository root and commit to `main`.

In **Settings → Pages** choose:

- Source: Deploy from a branch
- Branch: main
- Folder: / (root)

The included `CNAME` file preserves `find.tenniscourt.io`.
