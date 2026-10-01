# Founder Freedom · Funnel 1: The Freedom Audit

A VSL-led lead magnet funnel for Founder Freedom (James Clanfield). Cold traffic opts in, completes a one-page audit across the six PILLAR pillars, sees a personalised result with a VSL, and books a free Clarity Call.

## Funnel steps

| # | Page | Purpose |
|---|------|---------|
| 1 | Ads | Four ad hooks pointing to the opt-in page |
| 2 | Opt-in page | Headline and short form: first name, email, optional mobile |
| 3 | Audit form | 12 statements grouped by pillar, plus a short "About you" section |
| 4 | Results + VSL | Freedom Score, weakest pillar, first move and the results VSL |
| 5 | Book a call | Day and time picker for the Clarity Call |
| 6 | Call booked | Confirmation video and pre-call questions |

Use the bar at the bottom of the page to move between steps. **Notes & script** shows each page's purpose, target metric and the full VSL script. **Present** hides the preview tools.

## View it

- Open `index.html` in a browser, or
- Serve the folder locally: `python -m http.server 8080`, then open http://localhost:8080, or
- Turn on GitHub Pages (Settings → Pages → Deploy from branch → `main` / root).

## Add the videos

Set the two video slots in `videos.js`:

```js
"audit-results": "https://www.youtube.com/watch?v=...",  // Results page VSL
"audit-booked":  "https://vimeo.com/..."                 // Call booked video
```

YouTube, Vimeo, Loom and Wistia links work, or put a file in `videos/` and use `"videos/your-file.mp4"`. You can also click **Add video** on any video card to try a video in your own browser.

## Files

- `index.html`: all funnel pages, copy and audit logic
- `assets/ff.js`, `assets/ff.css`: page router, video cards, preview bar and notes panel
- `videos.js`: video settings
