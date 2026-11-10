# Reel 13 — one waiter's view: tap a name, see only their ratings (planned Fri 20 Nov 2026, 10:00)

Status: delivered 2026-11-10

Hook idea: „Który kelner zbiera najlepsze oceny? Jeden tap.” Motion in second 1 (tap on a staff name). Show the per-person filter and the fairness numbers exactly as the app shows them.

## Specs (all clips)
* MP4 (H.264), 30 fps, vertical 1080×1920, no audio
* No browser chrome, address bar, tabs, cursor or notifications
* Polish UI; owner dashboard in dark mode
* Demo data only (fake venue "Bistro Pod Lipą", fake staff Zosia, Kuba, Łucja, Michał, fake comments). No real data; send no real email or push. Seed demo data so that at least one person has ≥15 ratings and one person has <15 this week (to show „Za mało ocen do porównania”).
* Render at 3× pixel density (360×640 viewport). Deliver to `raw/reel13/` and change the status line to `Status: delivered <date>` with a "Delivered" section.

## Shots
* `a-tap-michal.mp4` (~4 s): 0.0 s „Oceny obsługi” table already in view (Osoba column visible, all four names); 0.4 s tap „Michał” → page reloads filtered („Tylko: Michał — pokaż wszystkich”; cut the reload); then tap „Oceny” in the jump bar → Michał's ratings list with comments; hold 1.5 s.
* `b-fair-chart.mp4` (~2.5 s, static/slow scroll): close-up of the fairness chart at the top of „Oceny obsługi” (bars per person, „vs zespół (te same godziny)” values) with the explanation text „Porównujemy każdą osobę z zespołem w tych samych dniach i godzinach… Porównujemy dopiero od 15 ocen…” readable; hold.
* `c-too-few.mp4` (~2.5 s): filtered to the person with <15 ratings, „Statystyki” card showing „Za mało ocen do porównania”; hold 1.5 s.
* If a part doesn't exist as described, record what the app shows and note it in Delivered. Don't fake UI.

## Delivered

* Demo data only (fake venue „Bistro Pod Lipą”, fake staff Zosia, Kuba, Łucja, Michał, fake comments); app run locally from nfc-reviews with a throwaway SQLite database and dummy secrets, all non-local requests blocked; no email or push was sent. 1080×1920, H.264, 30 fps, no audio, faststart, no browser chrome or cursor, dark mode. Rendered at exactly 3× (360×640 viewport, device pixels captured); recorded in 3× slow motion and played back at real speed for smooth motion.
* Seed (last 30 days): Zosia 34 ratings (+0,4 vs zespół, crown), Michał 24 (+0,0), Kuba 28 (−0,1), Łucja 7 → shown as „7/15”. Note: the team table and chart always use the last 30 days (not „this week”), so „under 15” is counted over 30 days.
* `a-tap-michal.mp4` (4.0 s): 0.0 s „Oceny obsługi” table (Osoba column; Zosia, Michał, Kuba, Łucja all visible); 0.4 s tap „Michał”; cut at ~0.55 s (reload removed) → top of dashboard with „Tylko: Michał — pokaż wszystkich” (range „7 dni”, person picker shows Michał); ~1.35 s tap „Oceny” in the jump bar → fast smooth scroll down past stats and the team table (~1.35–2.0 s) to „Oceny gości”; 2.4–4.0 s hold on Michał's ratings with comments („Bardzo uprzejmy kelner, polecamy.” 5★, „Pomylone zamówienie.” 2★ załatwione, next one partly visible). The jump scroll is the app's anchor jump, timed by the recorder (~0.65 s) so it renders smoothly.
* `b-fair-chart.mp4` (2.8 s): „Oceny obsługi (ostatnie 30 dni)” with the full explanation („Porównujemy każdą osobę z zespołem w tych samych dniach i godzinach — sobotni wieczór z sobotnim wieczorem. Porównujemy dopiero od 15 ocen, żeby jeden wieczór nikogo nie przekreślał.”), the bar chart (Zosia +0,4, Michał +0,0, Kuba −0,1, Łucja 7/15) and the table header „vs zespół (te same godziny)” with Zosia's row; hold 0–1.1 s, slow 40 px scroll 1.1–2.0 s, hold to 2.8 s.
* `c-too-few.mp4` (2.6 s): filtered to Łucja („Tylko: Łucja — pokaż wszystkich”, 7 dni); 0.3–1.0 s small scroll; 1.0–2.6 s hold on the „Średnia ocena” card: 3,3, „Za mało ocen do porównania”, „Ostatnie 7 dni”, plus 1 przejście do opinii / 4 oceny.
* Limitations: on the Statystyki card „Za mało ocen do porównania” means the week-vs-previous-week comparison needs more ratings (venue rule: 20) — it is not the per-person fairness rule; for Łucja the per-person „under 15” shows as „7/15” in the team chart/table (visible in clip b). The greeting line „Ten tydzień: 31 ocen…” above the filter stays venue-wide even when filtered (app behaviour). Dates on screen are the recording date (ratings up to 10.11.2026).
