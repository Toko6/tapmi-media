# Reel 13 — one waiter's view: tap a name, see only their ratings (planned Fri 20 Nov 2026, 10:00)

Status: requested

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
