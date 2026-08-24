# Exploring Context — Tomer Weller's old portfolio (2013)

A reconstruction of [tomerweller.com](http://www.tomerweller.com) ("Exploring Context"),
originally built in 2013, hosted on Heroku, and taken down in 2023. Recovered in August 2026
from the Wayback Machine and republished via GitHub Pages.

## Sources

- Homepage and assets: archived captures of `www.tomerweller.com`
  ([2015–2022 snapshots](https://web.archive.org/web/20211207122908/http://www.tomerweller.com/);
  the page was unchanged from April 2016 on). `css/custom.css` is taken from the
  October 2017 capture — the June 2017 capture still had `filter: blur(5px)` on the
  hero image, which was later commented out.
- Project detail pages (`anydo`, `cyclo`, `hp`, `huji`, `intel`, `logicalls`, `oulu`,
  `paradroid`, `seer`, `shenkar`, `social_urinal`) and the CV PDF: these Heroku routes
  were never archived under the custom domain, but a
  [October 2022 crawl of `tomerweller.herokuapp.com`](https://web.archive.org/web/20221024024731/https://tomerweller.herokuapp.com/)
  captured all of them.
- jQuery 2.0.3 (`bower_components/jquery/jquery.min.js`) was not archived, so it was
  re-vendored from code.jquery.com to keep the CDN-fallback path working.

## Changes from the original

- Absolute links (`/#play`, `/anydo`, …) were rewritten as relative so the site works
  under the GitHub Pages project subpath, and the server routes (`/anydo`) became flat
  files (`anydo.html`, served extensionless by GitHub Pages).
- A `404.html` was added.

Everything else — including the Google Analytics snippet and the self-deprecating
"WARNING: THIS IS AN OLD WEBSITE" banner — is preserved as-is.
