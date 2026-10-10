# galangajisusanto.github.io

GitHub Pages **user site** — served at the root of `https://galangajisusanto.github.io/`.

It exists for one reason: AdMob and Play verify ad sellers by fetching
`https://<developer-website-domain>/app-ads.txt` at the **domain root**. Project sites like
`/glabs-legal/` are sub-paths and are never crawled, so the file has to live here.

- `app-ads.txt` — IAB app-ads.txt listing the AdMob publisher ID. One line per ad network.
  The snippet comes from AdMob → Apps → View all apps → app-ads.txt.
- `index.html` — minimal landing page linking to the legal site.
- `.nojekyll` — serve files verbatim.

The developer website entered in Play Console (Store settings → Developer page / Store
listing → Website) must be on this domain, e.g. `https://galangajisusanto.github.io`.
After changing `app-ads.txt`, press "Check for updates" in AdMob; crawling takes up to 24 h.
