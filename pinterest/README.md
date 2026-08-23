# Pinterest bulk-upload setup

This repository is the public media host for the Next Comes Calm Pinterest test.

## Current batch
- 22 prepared Pins = 11 days at 2 Pins/day.
- Target cadence: 9:00 a.m. and 4:00 p.m. Eastern.
- Pinterest bulk creation supports up to 200 image/video Pins per CSV.
- The `Publish date` timestamps in the draft are written in UTC: 13:00 and 20:00 correspond to 9:00 a.m. and 4:00 p.m. EDT.

## Files
- `pins-master.csv` = source-of-truth working metadata.
- `bulk-upload-DRAFT_DO_NOT_UPLOAD.csv` = Pinterest-format CSV, intentionally blocked by placeholders until the listings are live and the two existing board names are inserted.
- `../images/` = public JPEG assets. Pinterest will fetch these through `raw.githubusercontent.com`.

## Before uploading to Pinterest
1. Confirm all expected JPEGs exist in `images/`.
2. Replace `REPLACE_WITH_EXISTING_SCHOOL_BOARD` with the exact name of the existing school/visual-support board.
3. Replace `REPLACE_WITH_EXISTING_GENERAL_BOARD` with the exact name of the existing broader calm-routines board.
4. Replace each `REPLACE_WITH_LIVE_ETSY_URL` with the matching live Etsy listing or bundle URL.
5. Rename the completed CSV to `bulk-upload-READY.csv`.
6. On desktop Pinterest Business: Settings → Import content → Upload .csv or .txt file → Upload.

## Pinterest CSV columns
Pinterest's current bulk creation format uses:
- `Title` (required, max 100 chars)
- `Media URL` (required; public direct image/video URL)
- `Pinterest board` (required)
- `Thumbnail` (required only for video; blank for image Pins)
- `Description` (optional, max 500 chars)
- `Link` (optional but required for this traffic test)
- `Publish date` (future timestamp schedules the Pin; Pinterest expects UTC when a time is included)
- `Keywords` (comma-separated search terms)

## Variation rule
Create variants when the buyer hook changes materially, not when only one or two words change. Preferred recurring angles:
- pain point / hard moment
- benefit / calmer routine
- no-printer-required
- phone / tablet / iPad use
- what's included
- bundle/value
- direct cover-led product Pin

Do not upload the DRAFT CSV while placeholder board names or Etsy URLs remain.
