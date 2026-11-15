# MUST UNION — Шөнийн 7

Movie night voting site, designed for GitHub Pages. No ChatGPT sign-in is required for visitors.

## Publish
In repository **Settings → Pages**, select **Deploy from a branch**, **main**, **/(root)**, then Save.

## Edit
Edit `src/App.tsx` and `style.css`. Run `npm install` and `npm run build` after editing the React source, then commit `app.js` alongside the source. The committed bundle runs directly on GitHub Pages.

## Voting
The frontend calls the existing hosted `/api/votes` endpoint using CORS restricted to `https://pzjswn89hg-lab.github.io`. Votes are stored centrally in Cloudflare D1, not only in the browser. A browser-local random ID allows changing one vote without adding another. Clearing browser storage or changing devices can create another voter; this is a casual poll, not an identity-verified election. No API keys or secrets are included.

## Movies
The Conjuring (2013), Talk to Me (2023), [REC] (2007), The Descent (2005), Host (2020), Barbarian (2022), Sinister (2012).

Poster artwork remains owned by the respective film rights holders.
