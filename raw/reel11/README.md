# Reel 11 — „Do przeczytania”: what's new since your last visit (planned Fri 13 Nov 2026, 10:00)

Status: delivered 2026-11-03

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

## Delivered

* Demo data only (fake venue „Bistro Pod Lipą”, fake staff Zosia, Kuba, Łucja, Michał, fake comments); app run locally from nfc-reviews with a throwaway SQLite database and dummy secrets, all non-local requests blocked; no email or push was sent. 1080×1920, H.264, 30 fps, no audio, faststart, no browser chrome or cursor. Rendered at exactly 3× (360×640 viewport, device pixels captured; motion frames ~25–30 fps, encoded at 30).
* Dates on screen are real recording dates (ratings dated 1–2.11.2026), which will look a week old by the posting date.
* App behaviour to know: the „4 nowe oceny od ostatniej wizyty” pill isn't tappable, so clip a taps „Oceny” in the jump bar instead. „Do przeczytania” shows ratings with a comment or 1–3★; a „Wcześniej” divider marks where your last visit was. Between days the app shows one summary line per day for the good ratings without a comment („Wczoraj · 3 dobre oceny bez komentarza”, 5★/4★ split and bar); tapping it expands those ratings. „Wszystkie” and the star chips reload the page and scroll to the list; those reloads are cut out (jump cuts in clip c).
* `a-new-since.mp4` (3.7 s): 0.0–0.3 s top of dashboard with „4 nowe oceny od ostatniej wizyty”; 0.3 s tap „Oceny” → jump (~0.3–1.4 s) to „Oceny gości”; 1.4–2.0 s small scroll so the „Do przeczytania · 4 nowe” tab sits under the jump bar; 2.0–3.7 s hold: Zosia 5★ „Piękny ogródek pod lipą, a szarlotka jak u babci!”, Michał 4★ „Smaczny żurek, tylko trochę długo czekaliśmy na rachunek.”, Kuba 2★ „Kotlet był zimny, a kelner się nie pojawiał.” (✓ załatwione + note) fully readable; Łucja 5★ only partly in view at the bottom (no room for a 4th full card).
* `b-day-summary.mp4` (5.2 s): 0.0–0.4 s hold; 0.4–2.8 s slow scroll past the 4th new rating and the „WCZEŚNIEJ” divider (~1.3–1.8 s), older ratings, to the „Wczoraj · 3 dobre oceny bez komentarza” summary line; 2.8–3.8 s hold on it; 3.8 s tap → expands to the three 5★ ratings without a comment; hold to 5.2 s.
* `c-all-tab.mp4` (3.1 s): 0.0–0.3 s „Do przeczytania”; 0.3 s tap „Wszystkie” → cut at ~0.4 s to the full list („Pasujące: 48”), hold ~1.1 s; ~1.6 s tap the 2★ chip → cut at ~1.7 s to „Pasujące: 2” (Kuba 2★ „Kotlet był zimny…”, Łucja 2★, both załatwione with notes); hold to 3.1 s.
