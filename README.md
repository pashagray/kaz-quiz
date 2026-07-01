# How Kazakh Are You? 🇰🇿

A fun pop-art quiz for a team-building session — 12 questions, fun facts after every
answer, an animated score, a hand-drawn radar chart of your "Kazakhstani DNA", confetti,
sound, and AI-generated pop-art personas.

Everything is a single self-contained `index.html` (no build step, no external JS libraries —
confetti and the radar chart are hand-written, so it works even offline). Only the web
fonts load from Google Fonts.

## Run locally

Just open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

## Deploy

### Vercel (recommended)
```bash
npx vercel login      # one-time, pick GitHub
npx vercel --prod --yes
```
Or drag the whole `kaz-quiz` folder onto https://vercel.com/new — it auto-detects a static site.

### GitHub Pages
Push this folder to a public repo and enable Pages (Settings → Pages → Deploy from branch → `main` / root).

## Structure
```
index.html            # the whole app
assets/img/*.png       # AI-generated pop-art mascot + 5 result personas
```

## Credits
Persona art generated with OpenAI `gpt-image-1.5`. Built for the team, pop-art edition. 💛💙
