# Reel 15 — „Ilu gości przeszło do Google?” — transitions per star rating (planned Fri 27 Nov 2026, 10:00)

Status: delivered 2026-11-17

Hook idea: „Ilu gości po ocenie przeszło do Google?” Motion in second 1 (scroll in „Statystyki”). Show the card „Przejścia do opinii wg oceny” (columns OCENY / GOOGLE, rows 5★…1★) exactly as the app shows it — it must be visible that guests with every rating can go to Google (e.g. a 2★ row with a transition). Never imply any filtering.

## Specs (all clips)
* MP4 (H.264), 30 fps, vertical 1080×1920, no audio
* No browser chrome, address bar, tabs, cursor or notifications (a tap indicator dot is fine)
* Polish UI; owner dashboard in dark mode
* Demo data only (fake venue "Bistro Pod Lipą", fake staff Zosia, Kuba, Łucja, Michał, fake comments). No real venue, guest or staff data; send no real email or push.
* Render at 3× pixel density (360×640 viewport) like reel8–reel13. Deliver to this folder and change the status line to `Status: delivered <date>` with a short "Delivered" section (timings + any app limitations).
* If a part doesn't exist as described, record what the app shows and note it in Delivered. Don't fake UI. Never use raw/reel2/a-tap.mp4.
* Seed the last 7 days so that the card has non-zero Google transitions in at least the 5★, 4★ and one low (1–2★) row.

## Shots
* `a-stats-scroll.mp4` (~3.5 s): 0.0 s top of „Statystyki” (Średnia ocena card); 0.3–1.5 s smooth scroll down past „Rozkład gwiazdek” to „Przejścia do opinii wg oceny”; hold 2 s with the whole card (header + all 5 rows) in the upper two thirds of the screen.
* `b-guest-google.mp4` (~3 s): guest page, fresh session; 0.4 s tap the 2nd star → thank-you with „Oceń nas w Google”; ~1.4 s tap „Oceń nas w Google” — cut BEFORE any external Google page loads (no real Google page or real venue on screen); hold on the tap moment 1 s.
* `c-card-closeup.mp4` (~2 s, optional): after shot b, reload the dashboard (cut the reload) and hold on „Przejścia do opinii wg oceny” with the 2★ row's Google count increased by 1.

## Delivered

* Demo data only (fake venue „Bistro Pod Lipą”, fake staff, fake comments); app run locally from nfc-reviews with a throwaway SQLite database and dummy secrets, all non-local requests blocked; the Google button's link was a dummy address and no external page was opened; no email or push sent. 1080×1920, H.264, 30 fps, no audio, faststart, no browser chrome or cursor, dashboard in dark mode, rendered at exactly 3× (360×640 viewport). Taps shown with a grey tap dot.
* Seed (last 7 days): card „Przejścia do opinii wg oceny” reads 5★ 11 → Google 7 (64%), 4★ 5 → 3 (60%), 3★ 2 → 0, 2★ 2 → 1 (50%), 1★ 2 → 0.
* `a-stats-scroll.mp4` (3.5 s): 0.0 s top of „Statystyki” (range pills, „Średnia ocena” 4,0, 11 przejść / 22 oceny); 0.30–1.50 s smooth scroll past „Oceny dziennie” and „Rozkład gwiazdek”; 1.50–3.50 s hold with the whole card (header OCENY / GOOGLE + rows 5★…1★) in the upper half of the screen.
* `b-guest-google.mp4` (2.4 s): guest page (fresh session, light — the guest page has no dark mode), „Bistro Pod Lipą — Jak oceniasz swoją wizytę?”; 0.40 s tap the 2nd star → 2 stars filled, „Dziękujemy za opinię!”, „Podzielisz się opinią także publicznie?” with „Oceń nas w Google” (same buttons as for every rating); 1.40 s tap „Oceń nas w Google” (the tap was counted by the app); hold on the tap 1.4–2.4 s; cut before anything external loads.
* `c-card-closeup.mp4` (2.0 s): dashboard after shot b (reload cut), same framing as the end of shot a: 2★ row now 3 ratings → Google 2 (67%) (was 1 (50%)); other rows unchanged.
* Note: the alert badge on the jump bar goes from 1 to 2 between a and c (the new 2★ rating is an open low rating) — app behaviour.

