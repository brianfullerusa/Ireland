# Dublin Trip Planner

A static website outlining Dublin activity options for our family trip August 29–31, 2026. Each activity has a dedicated page with a travel-agent panel review. Hostable on GitHub Pages.

## Files

- `index.html` — landing page with all activity cards
- `itinerary.html` — the recommended three-day plan
- `*.html` — one page per activity (12 total)
- `styles.css` — shared stylesheet

## Deploy to GitHub Pages

1. Create a new public repository on GitHub (e.g., `ireland-trip`).
2. Copy or drag all files in this folder into the repository (preserving the flat structure).
3. Commit and push. From the command line:

   ```sh
   cd "Dublin Website"
   git init
   git add .
   git commit -m "Dublin trip planner site"
   git branch -M main
   git remote add origin https://github.com/YOUR-USERNAME/ireland-trip.git
   git push -u origin main
   ```

4. In the repository on GitHub, go to **Settings → Pages**.
5. Under **Source**, choose **Deploy from a branch**.
6. Choose **main** branch and **/ (root)** folder. Save.
7. Wait ~1 minute. Your site will be live at `https://YOUR-USERNAME.github.io/ireland-trip/`.

## Alternatives

- **Netlify Drop** — drag this whole folder onto https://app.netlify.com/drop for instant hosting, no account needed.
- **Local preview** — double-click `index.html` to open it in a browser. Everything works offline.
