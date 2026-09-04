# GigLyrics 1.37 stage tracker polish

- Keep the current linear tracker and current line index.
- SpeechRecognizer now rests 100 ms after results/errors, then restarts while MIC ON.
- Restart does not reset the song to the first line.
- Reader no longer scrolls the highlighted line to the top on every match.
- Highlight walks downward through visible lyrics; the page scrolls only when the target leaves the viewport, placing it low on screen.
