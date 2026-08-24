# Exploring Context — Tomer Weller's old portfolio (2013)

A reconstruction of [tomerweller.com](http://www.tomerweller.com) ("Exploring Context"),
originally built in 2013, hosted on Heroku, and taken down in 2023. Recovered in August 2026
from the [Wayback Machine](https://web.archive.org/web/20211207122908/http://www.tomerweller.com/)
and republished via GitHub Pages.

## What was recovered

- The full single-page site: HTML, CSS, JS, fonts, favicon, and all 40 images, pulled from
  their original archived snapshots (2015–2021 captures; the page was unchanged from 2016 on).
- jQuery 2.0.3 (`bower_components/jquery/jquery.min.js`) was not archived, so it was
  re-vendored from code.jquery.com to keep the CDN-fallback path working.
- Absolute links (`/#play`, `/anydo`, …) were rewritten as relative so the site works
  under the GitHub Pages project subpath. That is the only change to the original markup.

## What was lost

The Wayback Machine only ever captured the homepage and its assets, so these Heroku
server routes are gone:

- Project detail pages: `/anydo`, `/cyclo`, `/hp`, `/huji`, `/intel`, `/logicalls`,
  `/oulu`, `/paradroid`, `/seer`, `/shenkar`, `/social_urinal`
  (their summary cards on the homepage survive in full)
- The CV PDF (`/tomerweller_cv_november_2013.pdf`)

A `404.html` redirects those dead links back to the homepage.

Everything else — including the Google Analytics snippet and the self-deprecating
"WARNING: THIS IS AN OLD WEBSITE" banner — is preserved as-is.
