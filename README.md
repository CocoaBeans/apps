# apps

Static support and privacy pages for Kevin Ross's apps, served via GitHub Pages.

Published at **https://cocoabeans.github.io/apps/**

The portfolio of all apps now lives at the site root, https://cocoabeans.github.io/
(repo [CocoaBeans/cocoabeans.github.io](https://github.com/CocoaBeans/cocoabeans.github.io)).
This repo's `index.html` just redirects there; the support and privacy pages below
keep their URLs, since app listings and other links point to them.

## Sites

| App | Support | Privacy |
|-----|---------|---------|
| Sesh Time | [/seshtime/](https://cocoabeans.github.io/apps/seshtime/) | [/seshtime/privacy.html](https://cocoabeans.github.io/apps/seshtime/privacy.html) |
| MetaSort | [/metasort/](https://cocoabeans.github.io/apps/metasort/) | [/metasort/privacy.html](https://cocoabeans.github.io/apps/metasort/privacy.html) |

## Structure

```
index.html       redirect to the portfolio at https://cocoabeans.github.io/
seshtime/
  index.html     support / landing page
  privacy.html   privacy policy
  style.css      per-app stylesheet (theme-aware, self-contained)
metasort/
  index.html     support / landing page
  privacy.html   privacy policy
  style.css      per-app stylesheet (theme-aware, self-contained)
404.html         fallback page
```

Each page is self-contained — no external fonts, scripts, or CDNs — and uses
relative links so the tree can move under a custom domain later without edits.

## Local preview

Any static server works, e.g.:

```sh
python3 -m http.server 8000
# then open http://localhost:8000/seshtime/
```
