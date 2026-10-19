# Reel 6 — comment search (planned Mon 26 Oct 2026, 10:00)

Status: requested 2026-10-19 (Content Studio)

Hook idea: „Ktoś narzekał na pierogi? Znajdziesz to w 2 sekundy.” Motion in second 1 (typing in the search box).

## Specs (all clips)
* MP4 (H.264), 30 fps, vertical 1080×1920, no audio
* No browser chrome, address bar, tabs, cursor or notifications
* Polish UI; owner dashboard in dark mode
* Demo data only (fake venue "Bistro Pod Lipą", fake staff Zosia, Kuba, Łucja, Michał, fake comments). No real venue, guest or staff data.
* Render at 3× pixel density like reel3/reel4. Deliver to `raw/reel6/` and change the status line to `Status: delivered <date>` with a short "Delivered" section (timings + any app limitations).
* Make sure the demo data has 3–4 comments that mention one dish (e.g. „pierogi”: two positive, one negative like „Pierogi trochę zimne”, one neutral) so the search returns several results.

## Shots
* `a-search.mp4` (~7 s): dashboard, scroll to the comment search (or open it); 0.0–0.5 s cursor in the empty search field; 0.5–2.0 s type „pierogi” letter by letter; results filter live (or after Enter); 2.5–4.5 s slow scroll through the 3–4 matching comments with stars, date and staff name visible; hold 2 s on the negative one.
* `b-search-empty.mp4` (~3 s, optional): clear the field and type a second word (e.g. „czekaliśmy”) to show it works for any word; hold 1 s on results.
* If the app has no comment search, write that in the Delivered section instead of faking it.
