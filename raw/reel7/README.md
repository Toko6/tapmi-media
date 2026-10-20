# Reel 7 — Monday weekly summary (planned Thu 29 Oct 2026, 10:00)

Status: delivered 2026-10-20

raw/reel4/c-weekly.mp4 is one static email screen (6 s): too thin for a Reel. This adds motion. Do NOT show anything the email doesn't contain (no best/worst day, no team ranking in the email).

## Specs (all clips)
* MP4 (H.264), 30 fps, vertical 1080×1920, no audio
* No browser chrome, address bar, tabs, cursor or notifications from other apps
* Polish UI; dashboard in dark mode (email itself light, as sent)
* Demo data only (fake venue "Bistro Pod Lipą", fake staff, fake comments). No real data; send no real email.
* Render at 3× pixel density. Deliver to `raw/reel7/` and change the status line to `Status: delivered <date>` with a "Delivered" section.

## Shots
* `a-email-scroll.mp4` (~6 s): the real „Twój tydzień” summary email for the demo venue at phone width, zoomed so text fills the frame width; 0–0.5 s top of the email (subject/heading visible); 0.5–4.5 s slow, smooth scroll through: ratings count, average + change, clicks to review, „Niskie oceny: X, z tego załatwione: X”, the two guest quotes; hold 1.5 s on the „Otwórz panel” button.
* `b-open-panel.mp4` (~5 s): tap „Otwórz panel” (or start on the button) → owner dashboard loads (dark mode) with average and weekly trend visible; hold 2 s.

## Delivered

* Demo data only (fake venue "Bistro Pod Lipą", fake staff and comments), app run locally with a throwaway database; no email or push was sent. 1080×1920, H.264, 30 fps, no audio, faststart, no browser chrome or cursor. Rendered at ~3.3× pixel density on a 330×587 viewport so the email text is bigger than at normal phone width.
* The email is the real „Twój tydzień” HTML produced by the app's own weekly-summary code for the demo venue, shown light (as sent). Only addition: two lines above it with the sender „Od: TapMi” and the email's real subject („Twój tydzień — Bistro Pod Lipą: 54 oceny · średnia 4,3★ · 15 przejść do opinii”), since the subject isn't part of the email body. Email content this week: 54 oceny · 4,3★ with „▲ 0,3 względem poprzedniego tygodnia” · 15 przejść do opinii · „Niskie oceny: 10, z tego załatwione: 7.” · quotes „Domowa lemoniada rewelacja.” and „Pyszny żurek, wrócimy!” · „Otwórz panel”. No best/worst day and no team line this week (the email shows a top person only with a clear 0,2+ lead).
* `a-email-scroll.mp4` (6.1 s): 0–0.5 s top (subject, TapMi logo, „Twój tydzień” heading); 0.5–4.5 s slow smooth scroll through the tiles, low-ratings line and the two quotes to the bottom; 4.5–6.1 s hold with „Otwórz panel” in the middle of the frame. The email is only a bit taller than the screen, so the scroll is short (~190 px of page); the tiles and quotes are on screen the whole time.
* `b-open-panel.mp4` (5.8 s): starts on the email bottom with „Otwórz panel”; 0.7 s tap; 1.5 s owner dashboard (dark) loads: „Bistro Pod Lipą”, „Dzień dobry”, „3 oceny czekają na Twoją reakcję”, „Ten tydzień: 54 oceny · średnia 4,3★ · 15 przejść do opinii · załatwione: 7”; 2.4–3.7 s smooth scroll to the „Średnia ocena” card; 3.7–5.8 s hold: ring 4,3, „↗ 0,3 względem: poprzednie 7 dni”, tiles 15 przejść do opinii / 54 oceny. At this width the last jump-bar item („Oceny”) is cut at the right edge.
