# Next Comes Calm — Pinterest Assets

Public asset host for Next Comes Calm Pinterest bulk-upload images and scheduling metadata.

## Structure
- `images/` — public JPEG pin assets used by Pinterest bulk creation.
- `pinterest/` — bulk-upload CSVs and working metadata.
- `encoded/` — temporary source payloads used by the repository workflow to reconstruct JPEG assets.

The image files are intentionally public so Pinterest can fetch them through `raw.githubusercontent.com` URLs.

Generated for the NCC launch test. Current cadence target: **2 Pins/day**.
