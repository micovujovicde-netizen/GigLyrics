# Vosk ARM-only install test

- Version 1.42 beta.
- Keeps Vosk English integration unchanged.
- Limits packaged native ABIs to arm64-v8a and armeabi-v7a only.
- Removes x86/x86_64/mips/mips64/legacy armeabi native payloads from the generated APK.
- No tracker, MIC, scroll, UI, package name, or signing changes.
