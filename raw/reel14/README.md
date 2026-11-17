# Reel 14 — filters: only low ratings with a comment, in two taps (planned Wed 25 Nov 2026, 10:00)

Status: delivered 2026-11-17

Hook idea: „Tylko skargi z komentarzem? Dwa tapnięcia.” Motion in second 1 (tap on a star chip). Show the star filter chips (1★…5★) and „Z komentarzem” in „Oceny gości” exactly as the app shows them.

## Specs (all clips)
* MP4 (H.264), 30 fps, vertical 1080×1920, no audio
* No browser chrome, address bar, tabs, cursor or notifications (a tap indicator dot is fine)
* Polish UI; owner dashboard in dark mode
* Demo data only (fake venue "Bistro Pod Lipą", fake staff Zosia, Kuba, Łucja, Michał, fake comments). No real venue, guest or staff data; send no real email or push.
* Render at 3× pixel density (360×640 viewport) like reel8–reel13. Deliver to this folder and change the status line to `Status: delivered <date>` with a short "Delivered" section (timings + any app limitations).
* If a part doesn't exist as described, record what the app shows and note it in Delivered. Don't fake UI. Never use raw/reel2/a-tap.mp4.
* Seed so that the last 7 days contain a mix: several 4–5★ (some without comment) and 3–4 ratings of 1–2★, at least 2 of them with a comment (e.g. „Długo czekaliśmy.”, „Zupa była zimna.”).

## Shots
* `a-filter-low.mp4` (~4 s): 0.0 s „Oceny gości” in view (tab „Wszystkie”, chips 1★–5★ and „Z komentarzem” visible, list full of mixed ratings); 0.4 s tap „1★”; ~0.9 s tap „2★” (if chips are single-select, tap only „2★” and note it); ~1.5 s tap „Z komentarzem” → list narrows to low ratings with comments; hold 2 s.
* `b-clear.mp4` (~2.5 s, optional): from the filtered state, tap the active chips off again → full list back; hold 1 s.

## Delivered

* Demo data only (fake venue „Bistro Pod Lipą”, fake staff Zosia, Kuba, Łucja, Michał, fake comments); app run locally from nfc-reviews with a throwaway SQLite database and dummy secrets, all non-local requests blocked; no email or push sent. 1080×1920, H.264, 30 fps, no audio, faststart, no browser chrome or cursor, dark mode, rendered at exactly 3× (360×640 viewport). Taps shown with a grey tap dot; page reloads after each chip tap are cut (each chip is a link that reloads the list) and the chips stay at the same screen position.
* Seed (last 7 days): 22 ratings — 11× 5★, 5× 4★ (most without a comment), 2× 3★, 2× 2★ („Długo czekaliśmy.” + one without comment), 2× 1★ („Zupa była zimna.” + one without comment).
* `a-filter-low.mp4` (4.0 s): 0.0 s „Oceny gości (Ostatnie 7 dni)”, tab „Wszystkie”, chips 1★–5★ and „Z komentarzem”, „Pasujące: 22” with mixed list; 0.40 s tap „1★” (list → 2 × 1★); 0.90 s tap „2★” (chips are multi-select: 1★ and 2★ both on, „Pasujące: 4”); 1.50 s tap „Z komentarzem” → „Pasujące: 2”: „Długo czekaliśmy.” (2★, Kuba, Otwarte) and „Zupa była zimna.” (1★, Michał, załatwione); hold 2.0–4.0 s.
* `b-clear.mp4` (2.4 s): from the filtered state, 0.30 s tap „Z komentarzem” off, 0.70 s „2★” off, 1.10 s „1★” off → full list („Pasujące: 22”); hold 1.4–2.4 s.
* **App bug visible in dark mode:** when „Z komentarzem” is active, the chip is unreadable — dark text on a dark background (style.css line 936 `html[data-theme="dark"] .chip.on { color: #111827; }`; the comment chip has no `--star` colour, so its active background is also #111827). Recorded as the app shows it (not faked). Fallback: `a-filter-low-light.mp4` (4.0 s, same timings, light mode) where the active chip is readable (dark pill, white text). Once the CSS is fixed the dark clip can be re-recorded — set Status back to requested.

