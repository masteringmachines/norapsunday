# The Sunday Gazette — No Rap Sunday

A single-page, no-build interactive music player styled as a black-and-white Art Deco 2000s newspaper. Drop in your own MP3/WAV/FLAC files and a WebGL "orb" reacts to the real audio in your browser — nothing is uploaded anywhere.

**[Live demo →](https://YOUR-USERNAME.github.io/REPO-NAME/)** *(update this link after enabling Pages — see below)*

## Features
- Real audio playback via the Web Audio API — drag & drop your own tracks
- Audio-reactive WebGL visualizer (Three.js) — bass warps the sphere, treble scatters the particles
- Decoded waveform seek bar drawn from your actual file
- Shuffle, repeat, keyboard shortcuts (Space / ← → / ↑ ↓)
- Every loaded track becomes an illustrated "record" card in the vault below
- 100% client-side — no backend, no build step, no dependencies to install

## Run it locally
Just open `index.html` in a browser. That's it — no npm install, no server required (Chrome/Edge/Firefox all work; Safari needs a user click before audio starts, which the UI already requires).

If you want a local server anyway (some browsers restrict `file://` audio decoding):
```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploy to GitHub Pages
1. Create a new repo on GitHub and push this folder to it (see below).
2. In the repo, go to **Settings → Pages**.
3. Under "Build and deployment", set **Source** to `Deploy from a branch`, branch `main`, folder `/ (root)`.
4. Save — your site will be live at `https://YOUR-USERNAME.github.io/REPO-NAME/` within a minute or two.

## Push this folder to GitHub
```bash
cd no-rap-sunday-repo
git init
git add .
git commit -m "Initial commit: No Rap Sunday player"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/REPO-NAME.git
git push -u origin main
```

## Project structure
```
.
├── index.html      # entire app: markup, styles, and JS in one file
├── README.md
└── .gitignore
```

## Credits
Fonts: Limelight, Poiret One, Playfair Display, IBM Plex Mono (Google Fonts).
3D: Three.js r128 (via cdnjs).
