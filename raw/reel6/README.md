# Reel 6 — comment search (planned Mon 26 Oct 2026, 10:00)

Status: delivered 2026-10-20

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

## Delivered

* Screen recordings of the real app, run locally with a throwaway database and demo data only (fake venue "Bistro Pod Lipą", fake staff Zosia, Kuba, Łucja, Michał, fake comments). No email or push sent. 1080×1920, H.264, 30 fps, no audio, faststart. Rendered at 3× pixel density (360×640 viewport), no browser chrome or cursor. Owner dashboard, dark mode, Polish UI.
* App note: the comment search is real („Szukaj w komentarzach…” box in „Oceny gości”, reached via „Oceny” in the jump bar). It filters **after Enter** (page reloads), not live while typing. It ignores case and Polish accents, and the matched word is highlighted in the results. The jump bar (Alerty / Statystyki / Obsługa / Oceny) stays pinned at the top of the frame.
* `a-search.mp4` (7.4 s): 0.0–0.6 s „Oceny gości” with the empty search box; 0.6 s tap (orange focus ring, text caret); 0.65–2.1 s „pierogi” typed letter by letter; 2.15 s Enter; 2.7 s results „Pasujące: 4”, word „pierogi” highlighted; 3.25–5.25 s slow scroll through the 4 results: 5★ Zosia 19.10 „Pierogi ruskie jak u babci, wrócimy!”, 5★ Michał 18.10 „Najlepsze pierogi z mięsem w okolicy.”, 3★ Kuba 17.10 „Pierogi w porządku, ale obsługa trochę wolna.” (załatwione), 2★ Łucja 16.10 „Pierogi trochę zimne.” (załatwione — „Przeprosiliśmy, deser na koszt lokalu.”); 5.25–7.4 s hold with the negative one fully visible at the bottom.
* `b-search-empty.mp4` (4.0 s, optional): starts on the „pierogi” results; 0.4 s tap, text selected and deleted; 0.85–2.0 s „czekaliśmy” typed; 2.15 s Enter; 2.7–4.0 s hold on „Pasujące: 2”: 3★ Kuba „Dobre jedzenie, ale długo czekaliśmy.” and 2★ Zosia „Czekaliśmy 40 minut na danie.” (both załatwione).
