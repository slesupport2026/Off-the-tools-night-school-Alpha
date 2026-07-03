# Off the Tools Night School — Camp Hub Site

Static site for the Night School cohort hub and Quick Wins Academy.

## Structure

```
/
├── index.html          Camp Alpha Hub (front door, loads at your root URL)
├── academy.html        Quick Wins Academy (10K in 10 Days)
├── sle-logo-red.png    YOU MUST ADD THIS (used by index.html)
└── sle-logo-gold.png   YOU MUST ADD THIS (used by academy.html)
```

## Before you push

Drop the two logo PNGs into the repo root with those exact filenames. The pages reference them relatively, so if they are missing the brand marks will show as broken images.

## Deploy to Netlify

1. Push this folder to your GitHub repo (all files at the root, not inside a subfolder)
2. In Netlify: Add new site, Import an existing project, pick the repo
3. Build command: leave empty. Publish directory: leave as root
4. Deploy. Your root URL serves the Camp Alpha Hub, and /academy takes them to Quick Wins Academy via the on-page links

No build step, no config files needed. Any push to main auto-redeploys.

## Duplicating for Camp Bravo later

Per the note in the CSS: copy index.html to bravo.html, change the two --camp color vars (Bravo blue is #2657D9), the title tag, and the hero camp name. Then add a link between camps if you want them cross-navigable.

## Notes

- Both pages have noindex meta tags, so search engines stay out. Good for a partner-only hub.
- Filenames were changed from "Camp Alpha Hub.html" and "Quick Wins Academy.html" to index.html and academy.html. All cross-links between the two pages were updated to match.
