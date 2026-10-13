# Reel 3 — low-rating alert (planned Thu 22 Oct)

Status: delivered 2026-10-13

## Specs (all clips)
* MP4 (H.264), 30 fps, vertical 1080×1920, no audio, no browser chrome or cursor
* Polish UI; dashboard in dark mode
* Demo data only (fake venue, staff, comments). No real venue, guest or staff data.

## Shots
* `b-guest-low.mp4` (~6 s): guest page loads, guest taps 2★, types a short comment (e.g. „Długo czekaliśmy na danie”), thank-you screen with the Google button still visible, hold 1 s.
* `c-alert.mp4` (~8 s): owner dashboard; the new 2★ rating with the comment appears (low-rating highlight / "Do przeczytania"), hold 2 s on it. If the app shows an in-panel alert or banner for low ratings, show it.

## Delivered

* Both clips: screen recordings of the app run locally with demo data only (fake venue "Bistro Pod Lipą", fake staff Zosia, Kuba, Łucja, Michał, fake comments). 1080×1920, H.264, 30 fps, no audio, faststart. Rendered at 3× pixel density (sharp text, not upscaled).
* `b-guest-low.mp4` (6.6 s): guest page (light, the guest page has no dark mode) loads; 0.1 s page visible; 1.4 s tap on the 2nd star (2★ saved); 2.4 s tap „+ Dodaj prywatną wiadomość dla zespołu”; 2.9–4.8 s types „Długo czekaliśmy na danie”; 4.9 s „Wyślij” → „Dziękujemy — przekazane.”; „Oceń nas w Google” stays visible the whole time (no review gating); hold to 6.6 s.
* `c-alert.mp4` (7.4 s): owner dashboard, dark mode. 0–2.0 s before: green „Wszystko załatwione…”; 2.0 s refresh (no live update in the app, it shows after reload) → „Alerty 1” in the top bar, orange banner „1 ocena czeka na Twoją reakcję. Zobacz →” and the „Wymaga reakcji 1” box; 3.7–4.6 s short scroll; 4.6–7.4 s hold on the card: Kuba · 2★ · „Długo czekaliśmy na danie” with „Dodaj notatkę” / „Załatwione”.
* Limitations: the in-panel signal is the orange banner + „Wymaga reakcji” box (there is no pop-up). Phone push and email alerts were not recorded (switched off in this demo setup so nothing leaves the sandbox).

