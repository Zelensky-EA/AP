# Anatomy & Physiology Course Navigator

A responsive, dependency-free course website generated from the **Anatomy & Physiology Navigator Framework** workbook.

## Preview locally

From this folder, run:

```bash
python -m http.server 8080
```

Then open `http://localhost:8080`.

## Content model

- `data.js` contains the 82 framework topics, BIOZONE Anatomy & Physiology 3rd Edition activity/page mappings, Crash Course alignments, system vocabulary, and saved Navigator entries.
- `app.js` renders the homepage, Daily Navigator, course atlas, all 13 unit/system guides, resource page, and global search.
- The Daily Navigator attempts to read the published Google Sheet CSV at page load. If that request is blocked by the host or browser, the site displays the saved framework schedule and clearly labels it as such.

## Deploy

The folder is ready for any static host: Google Sites embed, GitHub Pages, Netlify, Cloudflare Pages, or a school web server. No build command is required.

When the framework workbook changes, regenerate `data.js` from the workbook before redeploying to refresh the topic data.
