# KD Barbell website

The public pages Google Play asks for, for the KD Barbell Android app
(package `com.fitledger.fitledger`): the privacy policy, the account-deletion
page and support. Plain HTML and CSS; no build step, no JavaScript, no
analytics, no third-party resources.

Published with GitHub Pages at <https://keatondavis23.github.io/kd-barbell-site/>.

| Page | Purpose | Where the URL goes |
|---|---|---|
| `index.html` | Short introduction and links | Play Console › Store listing › Contact details › Website (optional) |
| `privacy.html` | Privacy policy | Play Console › App content › Privacy policy; the Health apps declaration; the Data safety form |
| `delete-account.html` | Account deletion, in the app and by email | Play Console › App content › Data safety › Account deletion URL |
| `support.html` | Contact and how to report a problem | Linked from the app's Help and from the store listing's support email |
| `404.html` | Not-found page (GitHub Pages serves it for unknown paths; it uses absolute paths under `/kd-barbell-site/` because it is served for nested paths too) | — |
| `styles.css`, `favicon.svg` | Shared stylesheet and icon | — |
| `.nojekyll` | Tells GitHub Pages to publish the files as they are, without Jekyll | — |

## Publishing

1. Repository **Settings › Pages**: *Build and deployment › Source* =
   **Deploy from a branch**, branch `main`, folder `/ (root)`. Save.
2. Once the first deployment finishes, tick **Enforce HTTPS** on the same
   page (it appears after the certificate is issued, usually within minutes).
3. Every push to `main` republishes the site within about a minute.

## Editing

Each page carries its own "Last updated" date in the `.meta` line under the
heading; change it whenever the text changes. Navigation links are
relative, so the site works at any base path. Keep the pages free of
scripts and external resources so that the privacy policy's statement
about this website stays true.

The policy text describes the app as built; a change to what the app
stores, reads or sends must be reflected here before the corresponding app
release goes out.
