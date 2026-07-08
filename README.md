# Hôtel Mozart Bruxelles — Website

A single-page site for Hôtel Mozart, a 17th-century boutique hôtel behind the Grand Place in Brussels.

- Plain HTML/CSS/JavaScript — no build step, no dependencies, no npm required.
- Trilingual: English / French / Dutch, with automatic browser-language detection and a manual switcher in the nav.
- The "Reserve" section submits directly to the real booking engine at direct-book.com.

## Running locally

No server is strictly required — you can open `index.html` directly in a browser. For best results (in case your browser restricts `file://` requests), serve it locally instead:

```bash
# Python 3
python -m http.server 8000

# or Node
npx serve .
```

Then visit `http://localhost:8000`.

## Deploying

This is a static site, so it deploys as-is to any static host:

- **GitHub Pages**: push this repo, then enable Pages in the repo Settings → Pages → set source to the `main` branch, root folder.
- **Vercel**: import the GitHub repo at [vercel.com/new](https://vercel.com/new) — no build command or framework preset needed ("Other" / static).
- **Netlify**: drag-and-drop this folder onto [app.netlify.com/drop](https://app.netlify.com/drop), or connect the GitHub repo.

## Structure

```
index.html      — the entire site (HTML + CSS + JS inline)
images/         — photography used across the site
```

## Notes

- Room names (Mirror Hall, Gilded Chamber, Composer's Study) and the postal address are intentionally left untranslated across all three languages.
- Photos are edited from originals sourced from the hotel's own site (hotel-mozart.be).
