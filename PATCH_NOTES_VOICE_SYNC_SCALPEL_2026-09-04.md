# GigLyrics Voice Sync — scalpel pass (2026-09-04)

Scope deliberately limited to lyric-match selection. No UI, scroll, Vosk lifecycle,
language detection, model download, grammar construction, or CURRENT/NEXT/NEXT+1
window changes.

## Problem found
The tracker checked CURRENT, NEXT, NEXT+1 in order and accepted the first candidate
that passed a permissive fuzzy boolean. A weak accidental match on CURRENT could
therefore hide a substantially better match on NEXT (especially through the Polish-ear
MontPoland adapter).

## Change
- Keep exactly the three-candidate local window.
- Compute a match score for each candidate.
- Advance only to the strongest candidate when it clears a confidence threshold and
  beats the runner-up by a small margin.
- MontPoland keeps its existing one-advance-per-Vosk-segment lock.
- English and MontPoland still use their existing models and grammar.

This is intentionally a cuckoo-clock patch: improve one decision, add no architecture.
