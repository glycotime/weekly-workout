# Hybrid Athlete Plan — 2026

A personal workout tracker running from **March 30 to December 31, 2026**.  
3 lifts + 3 runs per week, repeating every week. Checkboxes persist in your browser via `localStorage`.

## Features

- Week-by-week navigation (← → arrow keys or buttons)
- Checkboxes for every exercise — checked off state saves automatically in your browser
- Daily progress pill showing how many exercises you've completed
- Weekly progress bar across the top
- Today is automatically highlighted and the current week loads on open
- Past weeks dim slightly so you can still look back

## Deploy to GitHub Pages (5 minutes)

### Option A — New repo from scratch

1. Go to [github.com](https://github.com) → **New repository**
2. Name it anything, e.g. `workout-tracker` — keep it **Public**
3. Don't add a README yet
4. Once created, click **uploading an existing file**
5. Drag and drop `index.html` → **Commit changes**
6. Go to **Settings → Pages**
7. Under *Source*, select **Deploy from a branch**
8. Branch: `main` · Folder: `/ (root)` → **Save**
9. Wait ~60 seconds, then open `https://YOUR_USERNAME.github.io/workout-tracker/`

### Option B — GitHub CLI

```bash
# In the folder containing index.html
git init
git add index.html
git commit -m "init workout tracker"
gh repo create workout-tracker --public --push --source=.

# Then enable Pages in the repo settings (Settings → Pages → main branch)
```

## Notes

- **Checks are saved per browser.** They won't sync between devices — this is by design, no account needed.
- The plan runs 40 weeks total. Week 40 ends Thursday Dec 31 (partial week).
- All workout data is embedded in `index.html` — no internet connection needed once loaded.
- To reset a week, open browser DevTools → Application → Local Storage → clear keys starting with `hab:`.
