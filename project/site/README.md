# Omnia — iGaming Platform Landing

A single self-contained `index.html` (no build step, no external dependencies). Works offline and on GitHub Pages.

## Deploy to GitHub Pages

From inside this `site/` folder:

```bash
git init
git add .
git commit -m "Omnia landing page"
git branch -M main
git remote add origin https://github.com/<your-username>/example.git
git push -u origin main
```

(If the `example` repo already exists and has commits, clone it instead, copy `index.html` + `.nojekyll` in, then commit & push.)

Then enable Pages:

1. Repo → **Settings** → **Pages**
2. **Build and deployment → Source:** *Deploy from a branch*
3. **Branch:** `main`, **Folder:** `/ (root)` → **Save**
4. Wait ~1 minute. Your site goes live at:
   `https://<your-username>.github.io/example/`

## Files
- `index.html` — the landing page (everything inlined)
- `.nojekyll` — tells Pages to serve files as-is (skip Jekyll processing)
