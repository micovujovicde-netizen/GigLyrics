# GigLyrics — BLANK PAPER tracking reset

All experimental NEXT LINE / Stage GPS tracking code was removed.

Removed:
- continuous stage SpeechRecognizer tracking
- line matching/scoring logic
- local forward/backward search windows
- automatic highlighted-next-line state
- tracking-specific MIC/MIC ON control and SM58 drawing
- tracking-specific RECORD_AUDIO permission
- tracking-specific per-line LazyColumn/click-to-reposition behavior

The rest of GigLyrics is restored to the pre-tracking reader behavior.
Existing Local/Web voice search remains intact.

Version: 1.35-beta-blank-paper (versionCode 35)
