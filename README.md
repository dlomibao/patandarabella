# Pat & Arabella — Wedding Card

A single-page animated wedding card. A flock of birds (boids — separation, alignment, cohesion) wheels across a dusk sky, then settles into a heart, then re-arranges to spell **Congratulations Pat & Arabella**.

Pure HTML + Canvas, no dependencies, no build step.

## View locally

Open `index.html` in a browser, or:

```sh
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploy to GitHub Pages

1. Create a new GitHub repo (e.g. `patandarabella`).
2. Push this directory:
   ```sh
   git remote add origin git@github.com:<you>/patandarabella.git
   git push -u origin main
   ```
3. In the repo, **Settings → Pages → Build and deployment → Source: Deploy from a branch → `main` / `(root)`**.
4. Wait ~1 minute. Card lives at `https://<you>.github.io/patandarabella/`.

## Tweaking

All in `index.html`:

- `PHASE_TIMINGS` (seconds per phase: free flock → morph to heart → hold heart → morph to text → hold).
- `N` — bird count, auto-scaled to viewport.
- `drawText` — change the names or wording.
- Sky gradient is in the `#sky` CSS rule.
