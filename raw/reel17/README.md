# Reel 17 — „1 skarga na Kubę. I co?” — one complaint vs the person's numbers (planned Wed 2 Dec 2026, 10:00)

Status: delivered 2026-11-24

Hook idea (Reel #9 pattern: concrete problem moment + owner action): a fresh 2★ complaint about Kuba sits in „Wymaga reakcji”; the owner checks Kuba's numbers before judging (per-waiter angle, fair comparison from 15 ratings). Motion in second 1.

## Specs (all clips)
* MP4 (H.264), 30 fps, vertical 1080×1920, no audio
* No browser chrome, address bar, tabs, cursor or notifications (a tap indicator dot is fine)
* Polish UI; owner dashboard in dark mode
* Demo data only (fake venue "Bistro Pod Lipą", fake staff Zosia, Kuba, Łucja, Michał, fake comments). No real venue, guest or staff data; send no real email or push.
* Render at 3× pixel density (360×640 viewport) like reel8–reel15. Deliver to this folder and change the status line to `Status: delivered <date>` with a short "Delivered" section (timings + any app limitations).
* If a part doesn't exist as described, record what the app shows and note it in Delivered. Don't fake UI. Never use raw/reel2/a-tap.mp4.
* Seed ratings dated within the last 7 days of the recording day (so dates on screen look current).
* Seed: Kuba ≥ 30 ratings in the last 30 days with average ~4,4; one open 2★ for Kuba with comment „Długo czekaliśmy na rachunek.” in „Wymaga reakcji”.

## Shots
* `a-complaint.mp4` (~3 s): 0.0 s dashboard top with the orange banner „1 ocena czeka na Twoją reakcję”; 0.3 s tap „Zobacz →” (or „Alerty” in the jump bar) → jump to „Wymaga reakcji”; 1.2–3.0 s hold on the card Kuba · 2★ · „Długo czekaliśmy na rachunek.”.
* `b-tap-kuba.mp4` (~4 s): 0.0 s jump bar „Obsługa” → team table; 0.8 s tap „Kuba” → dashboard filtered („Tylko: Kuba”); ~2.0 s tap „Statystyki” → hold to 4.0 s on Kuba's average and rating count. (If the name on the rating card is tappable, start from the card instead and note it.)
* `c-kuba-row.mp4` (~2 s, optional): static hold on the team table with Kuba's row (Oceny / Średnia / vs zespół / % niskich) readable.

## Delivered

* Demo data only (fake venue „Bistro Pod Lipą”, fake staff Zosia, Kuba, Łucja, Michał, fake comments); app run locally from nfc-reviews (master 50a1523) with a throwaway SQLite database and dummy secrets, all non-local requests blocked; no email or push sent. 1080×1920, H.264, 30 fps, no audio, faststart, no browser chrome or cursor, dark mode, rendered at exactly 3× (360×640 viewport). Taps shown with a grey tap dot; page reloads after link taps are cut.
* Seed: 110 ratings, all dated 18–24 Nov 2026 (last 7 days); Kuba 32 ratings, average 4,4; one open low rating; 36 Google transitions.
* `a-complaint.mp4` (3.3 s): 0.0 s dashboard top, orange banner „1 ocena czeka na Twoją reakcję. Zobacz →”; 0.3 s tap „Zobacz →” → smooth jump to „Wymaga reakcji”; 1.2–3.3 s hold on the card Kuba · 2★ · 24.11.2026 · „Długo czekaliśmy na rachunek.” (with „Dodaj notatkę” / „Załatwione”).
* `b-tap-kuba.mp4` (6.7 s): starts where a ends (jump bar pinned); 0.15 s tap „Obsługa” → the app's smooth scroll to „Oceny obsługi” takes ~1.4 s, then a short scroll to show Kuba's row; ~3.0 s tap „Kuba” → dashboard with „Tylko: Kuba — pokaż wszystkich” (3.3 s); ~4.3 s tap „Statystyki” → 4.8–6.7 s hold: „Średnia ocena 4,4”, „32 Oceny”, „7 Przejścia do opinii”, person picker „Kuba”. Longer than ~4 s because the app's own scroll to the team section is slow; trim the scroll if needed.
* `c-kuba-row.mp4` (2.0 s): static team table, header OSOBA / OCENY / ŚREDNIA / VS ZESPÓŁ (TE SAME GODZINY) / % NISKICH and rows Zosia 28 · 4,6 · +0,1 · 7%, Łucja 24 · 4,5 · +0,0 · 8%, Michał 26 · 4,6 · +0,0 · 8%, Kuba 32 · 4,4 · −0,1 · 9% (Kuba last row, with his open-alert badge „1”).
* Limitations: the name on the rating card is not tappable (plain text), so b starts from the jump bar. The stats card says „Za mało ocen do porównania” because the seed has no ratings in the previous 7 days (kept so all dates look current). Kuba is only −0,1 vs the team in the fair comparison — fits the „one complaint, numbers fine” story. The trend column („TR…”) is cut at the right edge of the table on a phone.
