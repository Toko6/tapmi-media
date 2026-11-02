# Reel 11 — „Do przeczytania”: what's new since your last visit (planned Fri 13 Nov 2026, 10:00)

Status: requested 2026-11-02

Hook idea: „Nie masz czasu czytać wszystkich ocen?” Motion in second 1 (tap on „X nowe oceny od ostatniej wizyty”). Show the „Do przeczytania” view and the day summaries only as the app really shows them.

## Specs (all clips)
* MP4 (H.264), 30 fps, vertical 1080×1920, no audio
* No browser chrome, address bar, tabs, cursor or notifications
* Polish UI; owner dashboard in dark mode
* Demo data only (fake venue "Bistro Pod Lipą", fake staff Zosia, Kuba, Łucja, Michał, fake comments). No real data; send no real email or push.
* Render at 3× pixel density (360×640 viewport). Deliver to `raw/reel11/` and change the status line to `Status: delivered <date>` with a "Delivered" section.

## Shots
* `a-new-since.mp4` (~3 s): 0.0–0.3 s top of dashboard with „N nowe oceny od ostatniej wizyty”; 0.3 s tap it (or „Oceny” in the jump bar if the pill isn't tappable) → jump to „Oceny gości”, tab „Do przeczytania” with the „N nowe” badge; hold 1.5 s with 3–4 rated comments readable (mix of 5★, 4★ and one 2★).
* `b-day-summary.mp4` (~3 s): scroll slowly down „Do przeczytania” past a day divider / day summary (whatever the app shows between days, e.g. „Wcześniej” or a per-day summary line); hold 1 s on it.
* `c-all-tab.mp4` (~2 s): tap „Wszystkie” → full list; hold 1 s. Then tap a star filter (2★) → list narrows; hold 0.8 s.
* If day summaries don't exist as described, record what the app shows and note it in Delivered. Don't fake UI.
