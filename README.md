# 500 Secret Recipes — Landing Page

A single-page site for the "500 Secret Recipes" ebook. Pure HTML/CSS/JS, no build step, no framework.

## What's inside
```
index.html          page structure
styles.css           all styles
script.js             cursor glow, stat counters, FAQ accordion
favicon.ico            browser tab icon (multi-size)
favicon.svg             browser tab icon (vector)
assets/cover.jpg          ebook cover, used in the hero
assets/dossier-1.jpg        interior sample page, used in the hero stack
assets/dossier-2.jpg          interior sample page, used in the hero stack
README.md
```

## Deploy to GitHub + Vercel

1. **Create a GitHub repo**
   - Go to github.com → New repository (e.g. `500-secret-recipes`).
   - Upload everything in this folder, keeping the same structure (including the `assets/` folder), then commit.
   - Or, from your terminal in this folder:
     ```bash
     git init
     git add .
     git commit -m "Initial site"
     git branch -M main
     git remote add origin https://github.com/<your-username>/500-secret-recipes.git
     git push -u origin main
     ```

2. **Import into Vercel**
   - Go to vercel.com → Add New → Project → Import the GitHub repo you just created.
   - Framework preset: choose **Other** (this is a static site, no build command needed).
   - Leave the build command and output directory blank — Vercel serves the files as-is.
   - Click **Deploy**.

3. **Done** — Vercel gives you a live `*.vercel.app` URL. Add a custom domain later from the Vercel project's Domains tab.

## Notes
- The "Unlock the full vault" button links to your Payhip checkout: https://payhip.com/b/xUJVN
- To change the price, edit the `.price-old` / `.price-new` / `.price-save` values in `styles.css` and the matching text in `index.html` near `id="get-book"`.
- To swap an image, replace the file in `assets/` with a same-named file (or update the `src` path in `index.html` if the filename changes).
- The Google Fonts link in `index.html`'s `<head>` needs an internet connection to load — this is normal and will work automatically once the site is live.


