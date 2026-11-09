# Reel 12 — guest flow: rate in 5 seconds, Google button for every guest (planned Wed 18 Nov 2026, 10:00)

Status: requested

Hook idea: „Gość ocenia w 5 sekund. Bez aplikacji.” Motion in second 1 (finger taps a star). Second half: the Google review button appears after a 5★ AND after a 2★ — same screen, so it's visible that nobody is filtered by rating. Show only what the guest page really shows.

## Specs (all clips)
* MP4 (H.264), 30 fps, vertical 1080×1920, no audio
* No browser chrome, address bar, tabs, cursor or notifications (a tap indicator dot is fine if the app/recorder adds one)
* Polish UI. Guest page is light (venue colours, no dark mode) — record it as it is. If a dashboard shot is needed, dark mode.
* Demo data only (fake venue "Bistro Pod Lipą", fake staff Zosia, Kuba, Łucja, Michał, fake comments). No real venue, guest or staff data; send no real email or push.
* Render at 3× pixel density (360×640 viewport) like reel8–reel11. Deliver to `raw/reel12/` and change the status line to `Status: delivered <date>` with a short "Delivered" section (timings + any app limitations).

## Shots
* `a-rate-5.mp4` (~4 s): 0.0 s guest page already open (as after an NFC tap/QR scan; venue name visible); 0.4 s tap the 5th star; 0.8–2.5 s type a short comment „Świetna obsługa, wrócimy!” (only if the page has a comment field); ~2.6 s tap send; 2.8–4.0 s hold on the thank-you screen with the Google review button fully visible.
* `b-rate-2.mp4` (~3.5 s): same page, fresh session; 0.4 s tap the 2nd star; 0.8–2.0 s type „Długo czekaliśmy.”; ~2.1 s send; 2.3–3.5 s hold on the thank-you screen — the Google review button must be visible exactly as after 5★.
* `c-owner-sees.mp4` (~2.5 s, optional): owner dashboard (dark mode), top of „Oceny gości”, the 2★ rating from shot b appears at the top (reload is fine, cut it out); hold 1.5 s.
* If the comment field, button or thank-you screen look different from this description, record what the app shows and write it in Delivered. Don't fake UI. Never use raw/reel2/a-tap.mp4.
