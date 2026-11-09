# apps

Static support and privacy pages for Kevin Ross's apps, served via GitHub Pages.

Published at **https://cocoabeans.github.io/apps/**

The root [/](https://cocoabeans.github.io/apps/) is a small portfolio hub linking
to each app page plus the external product sites
([PingPoint](https://pingpoint.io), [Twenty-Four Mountains](https://24mountains.com)).

## Sites

| App | Support | Privacy |
|-----|---------|---------|
| Sesh Time | [/seshtime/support.html](https://cocoabeans.github.io/apps/seshtime/support.html) (home: [/seshtime/](https://cocoabeans.github.io/apps/seshtime/)) | [/seshtime/privacy.html](https://cocoabeans.github.io/apps/seshtime/privacy.html) |
| MetaSort | [/metasort/](https://cocoabeans.github.io/apps/metasort/) | [/metasort/privacy.html](https://cocoabeans.github.io/apps/metasort/privacy.html) |

## Structure

```
index.html       portfolio hub (links to each app + external product sites)
seshtime/
  index.html     product landing page (hero, screenshots, features, privacy)
  support.html   contact + FAQ
  privacy.html   privacy policy
  style.css      per-app stylesheet (theme-aware, self-contained; palette and
                 hero art match the App Store headers)
  media/         icon, favicons, share image and web-sized screenshots
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
