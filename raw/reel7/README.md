# Reel 7 — Monday weekly summary (planned Thu 29 Oct 2026, 10:00)

Status: requested 2026-10-19 (Content Studio)

raw/reel4/c-weekly.mp4 is one static email screen (6 s): too thin for a Reel. This adds motion. Do NOT show anything the email doesn't contain (no best/worst day, no team ranking in the email).

## Specs (all clips)
* MP4 (H.264), 30 fps, vertical 1080×1920, no audio
* No browser chrome, address bar, tabs, cursor or notifications from other apps
* Polish UI; dashboard in dark mode (email itself light, as sent)
* Demo data only (fake venue "Bistro Pod Lipą", fake staff, fake comments). No real data; send no real email.
* Render at 3× pixel density. Deliver to `raw/reel7/` and change the status line to `Status: delivered <date>` with a "Delivered" section.

## Shots
* `a-email-scroll.mp4` (~6 s): the real „Twój tydzień” summary email for the demo venue at phone width, zoomed so text fills the frame width; 0–0.5 s top of the email (subject/heading visible); 0.5–4.5 s slow, smooth scroll through: ratings count, average + change, clicks to review, „Niskie oceny: X, z tego załatwione: X”, the two guest quotes; hold 1.5 s on the „Otwórz panel” button.
* `b-open-panel.mp4` (~5 s): tap „Otwórz panel” (or start on the button) → owner dashboard loads (dark mode) with average and weekly trend visible; hold 2 s.
