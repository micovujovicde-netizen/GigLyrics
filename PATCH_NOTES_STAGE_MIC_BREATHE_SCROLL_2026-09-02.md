# Stage MIC breathe + calm 2/3 scroll — 2026-09-02

- SpeechRecognizer restart is requested only from onResults/onError.
- No restart from onEndOfSpeech.
- Normal restart cooldown: 700 ms.
- BUSY/CLIENT recovery: recreate after 1000 ms.
- Lyric position is preserved across recognizer cycles.
- Reader stays still while highlighted line moves down the visible page.
- At about 2/3 viewport height, page gently animates upward by about 1/4 viewport.
- No scroll-to-top behavior.
