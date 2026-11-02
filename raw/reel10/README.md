# Reel 10 — average + weekly trend (planned Tue 10 Nov 2026, 10:00)

Status: requested 2026-11-02

Hook idea: „Średnia spada, a Ty dowiesz się za miesiąc?” Motion in second 1 (tap into Statystyki). Show only what the dashboard really shows (average, weekly trend, per-staff numbers).

## Specs (all clips)
* MP4 (H.264), 30 fps, vertical 1080×1920, no audio
* No browser chrome, address bar, tabs, cursor or notifications
* Polish UI; owner dashboard in dark mode
* Demo data only (fake venue "Bistro Pod Lipą", fake staff Zosia, Kuba, Łucja, Michał, fake comments). No real venue, guest or staff data; send no real email or push.
* Render at 3× pixel density (360×640 viewport) like reel8/reel9. Deliver to `raw/reel10/` and change the status line to `Status: delivered <date>` with a short "Delivered" section (timings + any app limitations).

## Shots
* `a-stats.mp4` (~4 s): 0.0–0.3 s top of dashboard; 0.3 s tap „Statystyki” in the jump bar → smooth jump; 1.2–4.0 s hold on the average with the weekly trend (chart or arrow, whatever the app shows), all numbers readable. Demo data should give a visible change week to week (e.g. 4,5 → 4,2) so the trend is visible.
* `b-staff.mp4` (~3 s): 0.0 s tap „Obsługa” in the jump bar → team table (Osoba / Oceny / Średnia / Trend); 1.0–3.0 s hold. If a staff name is tappable and opens that person's ratings, tap Kuba at 1.5 s and hold on the result.
* `c-weekly-line.mp4` (~2 s, optional): close-up of the „Ten tydzień: … ocen · średnia …” line in „Dzień dobry”, static hold.
* If any part above doesn't exist in the app, write that in the Delivered section and skip it. Don't fake UI.
