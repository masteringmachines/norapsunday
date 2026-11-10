# No Rap Sunday — Glass Edition

A single-file, no-build music player. A backlit glass-block wall is the hero and a live 15-band equalizer, a phosphor "broadcast" globe reacts below it, and every track is pressed into a vintage soda label.

- Three house blends are generated live with the Web Audio API, so it works with no files.
- Drop your own MP3 / WAV / FLAC files anywhere on the page. Nothing is uploaded.
- Space = play/pause · ← → = skip · ↑ ↓ = volume. Hover a glass block to read its band; click glass to ripple; drag the globe; click it to jam the signal.

## Run
Open `index.html` in a browser, or `python3 -m http.server 8000`.

## Deploy on GitHub Pages
Push this folder to a repo, then Settings → Pages → Deploy from branch `main`, folder `/ (root)`.

```bash
git init && git add . && git commit -m "No Rap Sunday — glass edition"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/REPO-NAME.git
git push -u origin main
```

Fonts: Fraunces, Yellowtail, DM Mono, Instrument Sans (Google Fonts). 3D: Three.js r128 (cdnjs).
