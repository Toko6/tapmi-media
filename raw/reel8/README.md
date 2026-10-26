# Reel 8 — guest rates in their own language (planned Tue 3 Nov 2026, 10:00)

Status: requested

Hook idea: „Gość nie mówi po polsku? Oceni i tak.” Motion in second 1 (language switch). Show only what the guest page really does (PL / UK / EN). Every guest sees the Google button, whatever the rating.

## Specs (all clips)
* MP4 (H.264), 30 fps, vertical 1080×1920, no audio
* No browser chrome, address bar, tabs, cursor or notifications
* Guest page as a guest sees it on a phone (light, demo venue colours); Polish UI as the starting language
* Demo data only (fake venue "Bistro Pod Lipą", fake staff). No real venue, guest or staff data.
* Render at 3× pixel density like reel3/reel6. Deliver to `raw/reel8/` and change the status line to `Status: delivered <date>` with a short "Delivered" section (timings + any app limitations).

## Shots
* `a-lang-switch.mp4` (~5 s): guest rating page for the demo venue in Polish; 0.0–0.5 s hold; 0.5 s tap the language switch → Ukrainian (УКР / UK); page text changes; 2.0 s tap 5 stars; 2.5–4.0 s optional comment typed in Ukrainian (e.g. „Дуже смачно, дякуємо!”); 4.0 s send; hold on the thank-you screen with the Google review button visible 1 s.
* `b-lang-en.mp4` (~3 s, optional): same page, switch to English, tap 4 stars, thank-you screen with the Google review button.
* `c-dashboard-comment.mp4` (~3 s): owner dashboard (dark mode, Polish UI) showing the new rating with the Ukrainian comment as it arrives in „Oceny gości”. If the dashboard shows a translation or a language tag, show it; if it shows nothing extra, just the comment.
* If the guest page has no language switch (or only follows the phone's language), write that in the Delivered section and record the page opened with Ukrainian phone language instead. Don't fake UI.
