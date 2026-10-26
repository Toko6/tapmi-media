# Reel 9 — low rating handled: note + „Załatwione” (planned Thu 5 Nov 2026, 10:00)

Status: requested

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
