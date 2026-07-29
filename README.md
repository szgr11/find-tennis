# LA Tennis Court Finder — Build 12

This is a clean static GitHub Pages court finder. Court detection, calibration,
layout recognition, detector progress bars, and manual tuning have been
removed.

## Main features

- Dark tennis-themed interface
- Full-color Esri satellite map
- Background address mapping for all 165 facilities
- Search, area, category, lighting, court-count, distance, and nearby filters
- Facility side drawer that preserves map space
- Prominent Directions and Court information buttons
- Seven-day hourly weather planner using Open-Meteo
- Temperature, apparent temperature, rain chance, precipitation, wind, gusts,
  humidity, UV, cloud cover, visibility, sunrise, sunset, and suggested playing
  windows
- Short Finding tennis courts launch slideshow
- Google Maps link for live or typical activity when Google displays it

## Google activity limitation

Google Maps Platform's official Place data fields do not expose Popular Times
or live busyness. This build therefore links directly to the court in Google
Maps, where Google may display live and typical activity. It does not scrape
or invent activity data.

## Deploy

Upload every file and the `assets` folder to the repository root and commit to
`main`.

GitHub Pages:

- Source: Deploy from a branch
- Branch: main
- Folder: / (root)
