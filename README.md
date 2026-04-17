# Ireland Trip Planner

A static website for our family Ireland trip, August 29 – September 6, 2026. The site is organized by region (Dublin, Galway, Killarney, Return to Dublin), with a trip-wide timeline on the landing page and a full activity review hub for each region that's been planned in detail. Hostable on GitHub Pages.

## Architecture

- `regions_data.js` — the list of regions/legs of the trip. Add a new entry here to generate a new timeline node and region hub page.
- `activity_data.js` — per-activity data used by the region hubs.
- `website_generator.js` — the single static-site generator that reads both.

## Files

- `index.html` — trip overview + timeline of all regions (arrival → departure)
- `dublin.html` — Dublin region hub (12 activity cards, reviewed in depth)
- `galway.html`, `killarney.html`, `dublin-return.html` — scaffolded region hubs ready to expand
- `itinerary.html` — recommended 3-day Dublin plan
- 12 activity pages (one per Dublin activity)
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
