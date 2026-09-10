# FFX-2 Djose Machina Tracker

A single-page tracker for **Final Fantasy X-2** Djose Temple — *The Experiment* digging minigame.

Tap parts as you dig them: **A = 1**, **S = 3**, **Z = 5**. Each of Attack, Defense, and Special needs **38 points** to reach **Lv. 5** (114 points total). Progress is saved in the URL hash and in `localStorage`, so a refresh or a shared link keeps your counts.

Defeat Experiment once **before** all three stats hit Lv. 5 if you want Episode Complete.

Live site (after the first successful Actions deploy): `https://<your-username>.github.io/<repo-name>/`

## Push to a new GitHub repository

Create an empty GitHub repo (no README), then from this folder:

```bash
git init
git add .
git commit -m "Initial commit: FFX-2 Djose Machina Tracker for GitHub Pages"
git branch -M main
git remote add origin https://github.com/<your-username>/<repo-name>.git
git push -u origin main
```

Replace `<your-username>` and `<repo-name>` with your GitHub username and repository name.

The workflow in `.github/workflows/deploy.yml` deploys to **GitHub Pages** on every push to `main`. You do not need to set a branch source in repository settings: after the first run, Pages is served from GitHub Actions.

If Pages is not enabled yet, open **Settings → Pages**, set **Source** to **GitHub Actions**, and re-run the **Deploy to GitHub Pages** workflow.

## Add to your phone’s home screen (standalone app)

The page is a full-screen standalone web app (no browser chrome).

**iPhone / iPad (Safari)**

1. Open the live Pages URL in Safari.
2. Tap **Share** → **Add to Home Screen**.
3. Tap **Add**. Launch it from the home screen like a native app.

**Android (Chrome)**

1. Open the live Pages URL in Chrome.
2. Tap the menu (⋮) → **Add to Home screen** / **Install app**.
3. Confirm. The shortcut opens full-screen.

Progress stays on the device (`localStorage`) and in the URL (`#atk=&def=&spc=`), so you can share a link with your current counts.
