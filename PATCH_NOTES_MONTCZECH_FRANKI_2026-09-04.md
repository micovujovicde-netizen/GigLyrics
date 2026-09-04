# MontCzech Franki — 2026-09-04

Surgical swap only.

- English/Cecil lane untouched.
- Montenegrin hidden Vosk ear changed from Polish small model to Czech `vosk-model-small-cs-0.4-rhasspy` (~44 MB).
- Same continuous Vosk microphone lifecycle.
- Same CURRENT / NEXT / NEXT+1 tracker and strongest-match scalpel.
- Same one-advance-per-speech-segment guard.
- Visible lyrics untouched.
- Hidden BCS→Czech acoustic adapter: `nj→ň`, `đ→ď`, `ć→č`, `h→ch`; Czech-native `č/š/ž/c/j` stay unchanged.
- No new architecture. No chunking. No restart loop.
