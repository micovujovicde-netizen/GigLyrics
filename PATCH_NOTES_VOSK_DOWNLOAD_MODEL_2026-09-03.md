# v1.43 beta — Vosk model after install

- Removed the English Vosk model from the APK dependencies.
- APK keeps only the Vosk/JNA engine.
- On first app launch, English small model downloads from the official Vosk model host into app-private storage.
- Download is one-time; after installation the English listener works fully offline.
- Setup language list remains the home for future language downloads; English can retry download if needed.
- Existing linear NEXT LINE tracker and gentle 2/3-page scroll were not changed.
