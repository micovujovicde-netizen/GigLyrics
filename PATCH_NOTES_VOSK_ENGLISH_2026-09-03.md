# GigLyrics 1.41 — Vosk English stage test

- NEXT LINE stage listener now uses local/offline Vosk instead of Android SpeechRecognizer.
- English model ships through the Vosk English model dependency.
- Vosk listens continuously; no start/stop/restart loop between lyric lines.
- Recognition grammar is restricted to valid lyric lines from the open song plus [unk].
- Existing simple linear NEXT LINE progression and 2/3 gentle scrolling are preserved.
- Added a large setup gear. Setup contains the language area; English is installed/live and the other official Vosk mobile-language choices are listed as the future download slots.
