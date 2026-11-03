# Reel 10 — average + weekly trend (planned Tue 10 Nov 2026, 10:00)

Status: delivered 2026-11-03

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

## Delivered

* Demo data only (fake venue „Bistro Pod Lipą”, fake staff Zosia, Kuba, Łucja, Michał, fake comments); app run locally from nfc-reviews with a throwaway SQLite database and dummy secrets, all non-local requests blocked; no email or push was sent. 1080×1920, H.264, 30 fps, no audio, faststart, no browser chrome or cursor. Rendered at exactly 3× (360×640 viewport, device pixels captured; motion frames ~25–30 fps, encoded at 30).
* Dates on screen are real recording dates (ratings dated 1–2.11.2026), which will look a week old by the posting date.
* App behaviour to know: the weekly trend is not a chart of weekly averages — it's the arrow on the „Średnia ocena” card („↘ 0,3 względem: poprzednie 7 dni”, i.e. last 7 days vs the 7 days before; demo data 4,5 → 4,2). The „Oceny dziennie” chart shows rating counts per day, not averages. In the team table the „Trend” column (last 30 days vs 30 days before) is off-screen to the right on a phone; clip b2 swipes the table to show it. Tapping a name doesn't open a per-person ratings list; it reloads the whole dashboard filtered to that person („Tylko: Kuba — pokaż wszystkich”).
* `a-stats.mp4` (4.1 s): 0.0–0.3 s top of dashboard („Dzień dobry”, „4 nowe oceny od ostatniej wizyty”); 0.3 s tap „Statystyki” → smooth jump (~0.3–0.9 s); 0.9–4.1 s hold on „Średnia ocena 4,2” ring with „↘ 0,3 względem: poprzednie 7 dni”, plus 14 przejścia do opinii and 48 ocen.
* `b-staff.mp4` (5.2 s): 0.15 s tap „Obsługa” → jump (~0.2–1.1 s) to „Oceny obsługi (ostatnie 30 dni)”: fairness chart and the table (Osoba / Oceny / Średnia / vs zespół (te same godziny) / % niskich / Trend…), Kuba and Michał rows in view; 1.5 s tap „Kuba” → page reloads (~2.0 s) to the dashboard filtered to Kuba („Tylko: Kuba”); ~2.9 s tap „Statystyki” → Kuba's numbers: average 4,2, „Za mało ocen do porównania” (only 6 ratings this week), 3 przejścia, 6 ocen; hold to 5.2 s. Cut at ~2.0 s if you only want the table.
* `b2-staff-trend.mp4` (3.6 s, extra): team table with all four people (Kuba 35 · 4,3 · +0,1 · 20%, Michał 51 · 4,4, Łucja 48 · 4,4, Zosia 46 · 4,3); 0.6–1.8 s table swiped left to show „Trend”: Kuba ↘ 0,2, Michał ≈ bez zmian, Łucja ≈ bez zmian, Zosia ↘ 0,3; hold to 3.6 s.
* `c-weekly-line.mp4` (2.0 s, static): close-up of the „Dzień dobry” block, rendered sharp at 9× and centred on the dashboard background (no zoomed crop): „Wszystko załatwione. Goście oceniają Was średnio na 4,2★ w tym tygodniu.”, „4 nowe oceny od ostatniej wizyty”, „Ten tydzień: 48 ocen · średnia 4,2★ · 14 przejść do opinii · załatwione: 12”.

## Edit note (3 Nov)
Use the full-width Reel layout from the repo README („Reel layout”). Don't use the small card.
