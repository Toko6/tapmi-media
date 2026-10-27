# Reel 8 — guest rates in their own language (planned Tue 3 Nov 2026, 10:00)

Status: delivered 2026-10-27

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

## Delivered

* Demo data only (fake venue „Bistro Pod Lipą”, fake staff Zosia, Kuba, Łucja, Michał, fake comments); app run locally from nfc-reviews with a throwaway SQLite database and dummy secrets, all non-local requests blocked; no email or push was sent. 1080×1920, H.264, 30 fps, no audio, faststart, no browser chrome or cursor. Rendered at exactly 3× (360×640 viewport, captured frame by frame at device pixels).
* **App limitation: the guest page has no language switch.** It follows the phone's language (Accept-Language: PL / UK / EN, fallback EN; a `?lang=uk` link parameter also exists for demos). So, as the brief says, the clips are the page opened on a phone set to Ukrainian / English — no switch tap and no PL→UK change on screen. Every guest sees the Google button after rating, whatever the stars.
* `a-lang-switch.mp4` (5.0 s), Ukrainian phone: 0.0–0.5 s hold („Як пройшов ваш візит?”, 5 empty stars); 0.5 s tap 5 stars → „Дякуємо за відгук!”, private-note link and „Оцініть нас у Google” appear; 1.3 s tap „+ Додати приватне повідомлення для команди”; 1.65–3.6 s „Дуже смачно, дякуємо!” typed letter by letter; 3.65 s „Надіслати”; 3.7–5.0 s hold on „Дякуємо — передали.” with „Оцініть нас у Google” and „Ні, дякую — це все” visible.
* `b-lang-en.mp4` (3.2 s), English phone: 0.0–0.5 s hold („How was your experience?”); 0.5 s tap 4 stars; 0.6–3.2 s hold on „Thanks for letting us know!” with „Review us on Google”.
* `c-dashboard-comment.mp4` (3.2 s), owner dashboard dark, Polish: 0.0–0.4 s top of dashboard („2 nowe oceny od ostatniej wizyty”); 0.4 s tap „Oceny” in the jump bar → smooth jump to „Oceny gości”; 1.4–3.2 s hold: top row 5★ · Zosia · „Дуже смачно, дякуємо!” with the new-rating dot, „Do przeczytania 2 nowe”, „Wcześniej” divider below. The comment is the real one sent in clip a. The dashboard shows no translation and no language tag — just the comment as written. It doesn't update live; the new rating shows on the next open (as here).
