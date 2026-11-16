# Reel 14 — filters: only low ratings with a comment, in two taps (planned Wed 25 Nov 2026, 10:00)

Status: requested 2026-11-16

Hook idea: „Tylko skargi z komentarzem? Dwa tapnięcia.” Motion in second 1 (tap on a star chip). Show the star filter chips (1★…5★) and „Z komentarzem” in „Oceny gości” exactly as the app shows them.

## Specs (all clips)
* MP4 (H.264), 30 fps, vertical 1080×1920, no audio
* No browser chrome, address bar, tabs, cursor or notifications (a tap indicator dot is fine)
* Polish UI; owner dashboard in dark mode
* Demo data only (fake venue "Bistro Pod Lipą", fake staff Zosia, Kuba, Łucja, Michał, fake comments). No real venue, guest or staff data; send no real email or push.
* Render at 3× pixel density (360×640 viewport) like reel8–reel13. Deliver to this folder and change the status line to `Status: delivered <date>` with a short "Delivered" section (timings + any app limitations).
* If a part doesn't exist as described, record what the app shows and note it in Delivered. Don't fake UI. Never use raw/reel2/a-tap.mp4.
* Seed so that the last 7 days contain a mix: several 4–5★ (some without comment) and 3–4 ratings of 1–2★, at least 2 of them with a comment (e.g. „Długo czekaliśmy.”, „Zupa była zimna.”).

## Shots
* `a-filter-low.mp4` (~4 s): 0.0 s „Oceny gości” in view (tab „Wszystkie”, chips 1★–5★ and „Z komentarzem” visible, list full of mixed ratings); 0.4 s tap „1★”; ~0.9 s tap „2★” (if chips are single-select, tap only „2★” and note it); ~1.5 s tap „Z komentarzem” → list narrows to low ratings with comments; hold 2 s.
* `b-clear.mp4` (~2.5 s, optional): from the filtered state, tap the active chips off again → full list back; hold 1 s.
