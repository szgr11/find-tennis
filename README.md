# LA Tennis Court Finder — Learning detector

## Detection fixes

- The visible map is scanned first at high resolution.
- The facility center is scanned at court-readable resolution.
- Offset facilities use eight smaller high-resolution park tiles instead of
  one large blurry image.
- Court-line scanning yields to the browser every few milliseconds.
- Every scan is cancellable and has a hard deadline.
- The progress interface cannot freeze at 86%.

## Manual tuning

Open a facility and choose **Tune layout manually**.

1. Click four corners of each individual court.
2. Repeat for every court.
3. Choose **Finish and tune detector**.

The layout and appearance descriptors are stored in the browser and loaded on
future visits.

**Submit tuning on GitHub** opens a prefilled Issue in
`szgr11/latenniscourts`. A static GitHub Pages site cannot safely write to the
repository directly without exposing credentials.

Reviewed Issue data can be added to `community_tuning.json`, allowing approved
tuning to benefit every visitor.

## Typography

- Barlow Condensed for athletic headings
- Manrope for controls
- Source Serif 4 for addresses, weather details, tune-up copy, and supporting
  editorial text

Long labels were shortened and components wrap safely.

## Deploy

Upload every file to the repository root and commit to `main`.

GitHub Pages:

- Source: Deploy from a branch
- Branch: main
- Folder: / (root)
