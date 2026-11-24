# Reel 18 — „3× zimna zupa w tym miesiącu?” — search + star filter on comments (planned Fri 4 Dec 2026, 10:00)

Status: delivered 2026-11-24

Hook idea (Reel #9 pattern): a repeating complaint. Owner types „zup” in the comment search, results highlight the word, then taps 1★ + 2★ to keep only the low ones. Motion in second 1 (typing).

## Specs (all clips)
* MP4 (H.264), 30 fps, vertical 1080×1920, no audio
* No browser chrome, address bar, tabs, cursor or notifications (a tap indicator dot is fine)
* Polish UI; owner dashboard in dark mode
* Demo data only (fake venue "Bistro Pod Lipą", fake staff Zosia, Kuba, Łucja, Michał, fake comments). No real venue, guest or staff data; send no real email or push.
* Render at 3× pixel density (360×640 viewport) like reel8–reel15. Deliver to this folder and change the status line to `Status: delivered <date>` with a short "Delivered" section (timings + any app limitations).
* If a part doesn't exist as described, record what the app shows and note it in Delivered. Don't fake UI. Never use raw/reel2/a-tap.mp4.
* Seed ratings dated within the last 7 days of the recording day (so dates on screen look current).
* Seed in the last 30 days: 3 low ratings (1–2★, different days and staff) with comments containing „zupa” (e.g. „Zupa była zimna.”, „Zupa letnia, długo czekaliśmy.”, „Zimna zupa pomidorowa.”) and 1–2 good ratings mentioning „zupa” (e.g. 5★ „Świetna zupa dnia!”). Use the LIGHT theme for this shot if the dark-mode active chip is still unreadable (bug from raw/reel14) and say so in Delivered.

## Shots
* `a-search-zup.mp4` (~3.5 s): „Oceny gości”, 30 dni; 0.3 s tap the search field; 0.5–1.3 s type „zup” and press Enter; 1.5–3.5 s hold on the results with „zup” highlighted and „Pasujące: N”.
* `b-low-only.mp4` (~3 s): continue from a: 0.3 s tap 1★, 0.9 s tap 2★ → only the 3 low „zupa” comments remain; hold to 3.0 s with all three cards readable (dates + staff names visible).

## Delivered

* Demo data only (fake venue „Bistro Pod Lipą”, fake staff Zosia, Kuba, Łucja, Michał, fake comments); app run locally from nfc-reviews (master 50a1523) with a throwaway SQLite database and dummy secrets, all non-local requests blocked; no email or push sent. 1080×1920, H.264, 30 fps, no audio, faststart, no browser chrome or cursor, dark mode, rendered at exactly 3× (360×640 viewport). Taps shown with a grey tap dot; page reloads after link taps are cut.
* Seed: 110 ratings, all dated 18–24 Nov 2026 (last 7 days); Kuba 32 ratings, average 4,4; one open low rating; 36 Google transitions.
* `a-search-zup.mp4` (3.6 s): „Oceny gości (Ostatnie 30 dni)”, view „Do przeczytania”; 0.3 s tap the search field; 0.5–1.0 s type „zup”; ~1.2 s Enter (reload cut) → 1.2–3.6 s hold: „Pasujące: 5”, „zup” highlighted in „Zupa była zimna.” (1★ Zosia), „Świetna zupa dnia!” (5★ Kuba), third card partly visible.
* `b-low-only.mp4` (4.8 s): continues from a; 0.3 s tap „1★” → „Pasujące: 2”; ~1.4 s tap „2★” → „Pasujące: 3” (both chips on, multi-select); 2.3–2.6 s short scroll; 2.6–4.8 s hold with all three cards readable: 1★ Zosia 22.11.2026 19:12 „Zupa była zimna.”, 2★ Michał 20.11.2026 18:27 „Zupa letnia, długo czekaliśmy.”, 1★ Łucja 18.11.2026 13:41 „Zimna zupa pomidorowa.” (all „załatwione — Omówione z kuchnią.”).
* Dark mode used: the active 1★/2★ chips are readable (coloured pill, dark text). The reel14 dark-mode bug affects only the „Z komentarzem” chip, which is not used here.
