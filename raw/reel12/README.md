# Reel 12 — guest flow: rate in 5 seconds, Google button for every guest (planned Wed 18 Nov 2026, 10:00)

Status: delivered 2026-11-10

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

## Delivered

* Demo data only (fake venue „Bistro Pod Lipą”, fake staff Zosia, Kuba, Łucja, Michał, fake comments); app run locally from nfc-reviews with a throwaway SQLite database and dummy secrets, all non-local requests blocked; no email or push was sent. 1080×1920, H.264, 30 fps, no audio, faststart, no browser chrome or cursor. Rendered at exactly 3× (360×640 viewport, device pixels captured). Interactions were recorded in 3× slow motion and played back at real speed, so motion is smooth (~35 captured frames/s); server responses therefore look slightly snappier than on a real phone.
* App behaviour to know: the comment field is folded behind a button „+ Dodaj prywatną wiadomość dla zespołu” (with the hint „Trafi prosto do zespołu, a nie na publiczny portal z opiniami…”), so each clip has one extra tap before typing. The thank-you text „Dziękujemy za opinię!”, „Podzielisz się opinią także publicznie?” and the „Oceń nas w Google” button appear immediately after the star tap — before and after the comment, identical for 5★ and 2★. After sending, the comment box turns into „Dziękujemy — przekazane.” There is no separate thank-you page (the „Nie, dziękuję — to wszystko” button would lead to one, not tapped).
* `a-rate-5.mp4` (3.8 s): 0.0 s guest page („Bistro Pod Lipą”, „Jak oceniasz swoją wizytę?”); 0.4 s tap 5th star → thank-you + Google button; ~0.75 s tap „+ Dodaj prywatną wiadomość…”; 0.9–2.2 s typing „Świetna obsługa, wrócimy!”; ~2.4 s tap „Wyślij”; 2.5–3.8 s hold on „Dziękujemy — przekazane.” with „Oceń nas w Google” fully visible.
* `b-rate-2.mp4` (3.4 s, fresh browser session): 0.4 s tap 2nd star → same thank-you + Google button; ~0.75 s open the message box; 0.9–1.8 s typing „Długo czekaliśmy.”; ~1.95 s „Wyślij”; 2.1–3.4 s hold — Google button in the same place and look as after 5★.
* `c-owner-sees.mp4` (2.6 s, dark mode): 0.0–0.8 s top of „Oceny gości” (Do przeczytania) with Zosia's 5★ „Świetna obsługa, wrócimy!” from shot a on top; cut at 0.8 s (reload removed) → Kuba 2★ „Długo czekaliśmy.” with „Otwarte” tag is now first, and „Alerty 1” appears in the jump bar; hold 1.8 s.
* Dates on screen are the recording date (10.11.2026).
