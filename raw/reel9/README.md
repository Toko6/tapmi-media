# Reel 9 — low rating handled: note + „Załatwione” (planned Thu 5 Nov 2026, 10:00)

Status: delivered 2026-10-27

Hook idea: „Niska ocena. Co dalej?” → owner adds a note and marks it handled; the team sees what was done. Motion in second 1 (tap on the alert / rating).

## Specs (all clips)
* MP4 (H.264), 30 fps, vertical 1080×1920, no audio
* No browser chrome, address bar, tabs, cursor or notifications
* Polish UI; owner dashboard in dark mode
* Demo data only (fake venue "Bistro Pod Lipą", fake staff Zosia, Kuba, Łucja, Michał, fake comments). No real data; send no real email or push.
* Render at 3× pixel density. Deliver to `raw/reel9/` and change the status line to `Status: delivered <date>` with a "Delivered" section.

## Shots
* `a-open-low.mp4` (~3 s): dashboard „Wymaga reakcji” section; 0.0–0.3 s hold; 0.3 s tap a 2★ rating with a comment (e.g. „Długo czekaliśmy na rachunek.”); it opens/expands, comment fully readable.
* `b-note-done.mp4` (~5 s): 0.0 s tap „Dodaj notatkę”; 0.4–2.5 s type „Przeprosiliśmy, kawa na koszt lokalu.” letter by letter; 2.8 s save; 3.3 s tap „Załatwione”; hold 1.5 s on the rating now marked „załatwione” with the note visible.
* `c-counter.mp4` (~3 s, optional): the „Wymaga reakcji” counter going down by one (e.g. 3 → 2), or the „Ten tydzień … załatwione: N” line updated. Only if the app really updates it.

## Delivered

* Demo data only (fake venue „Bistro Pod Lipą”, fake staff Zosia, Kuba, Łucja, Michał, fake comments); app run locally from nfc-reviews with a throwaway SQLite database and dummy secrets, all non-local requests blocked; no email or push was sent. 1080×1920, H.264, 30 fps, no audio, faststart, no browser chrome or cursor. Rendered at exactly 3× (360×640 viewport, captured frame by frame at device pixels).
* App behaviour to know: alerts in „Wymaga reakcji” are always shown fully (comment readable), tapping a card doesn't expand it. The note has no separate „save” — it's saved with the „Załatwione” tap. After „Załatwione” the alert slides out of „Wymaga reakcji” and a „Załatwione · Cofnij” bar shows; the „załatwione — note” status is shown in „Oceny gości” (clip d). „Ten tydzień … załatwione: N” only updates on the next page load.
* `a-open-low.mp4` (3.2 s): 0.0–0.3 s top of dashboard („3 oceny czekają na Twoją reakcję. Zobacz →”); 0.3 s tap „Zobacz →” → jumps to „Wymaga reakcji 3”; 0.9–3.2 s hold with Kuba 2★ „Długo czekaliśmy na rachunek.” at the top (tap on it at 1.4 s, nothing changes — no expand), Michał 3★ and Łucja 1★ below.
* `b-note-done.mp4` (5.8 s): 0.0–0.3 s hold on Kuba's alert; 0.3 s tap „Dodaj notatkę” → field opens; 0.8–3.0 s „Przeprosiliśmy, kawa na koszt lokalu.” typed letter by letter (single-line field, so the start of the text scrolls out on the left near the end); 3.8 s tap „Załatwione” → card fades out, counter 3 → 2, „Załatwione · Cofnij” bar at the bottom; 4.1–5.8 s hold.
* `c-counter.mp4` (3.0 s): top area with „Alerty 3”, „3 oceny czekają na Twoją reakcję” and „Wymaga reakcji 3” all in frame; 0.6 s tap „Załatwione” on Kuba's alert → ~0.9 s all three change to 2 („2 oceny czekają…”), the card leaves, undo bar shows; hold to 3.0 s. „Ten tydzień … załatwione: 2” stays until reload.
* `d-resolved-in-list.mp4` (3.0 s, extra, static): after clip b, dashboard reopened, „Oceny gości” filtered to 2★: Kuba · 2★ · „Długo czekaliśmy na rachunek.” · „✓ załatwione — Przeprosiliśmy, kawa na koszt lokalu.” Use as the end card for „marked załatwione with the note visible”.
