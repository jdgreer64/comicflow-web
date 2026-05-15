# comicflow-web

Public static-asset host for [ComicFlow](https://github.com/jdgreer64/comicflow)
(the iOS app's main repo is private, so this exists only to serve files
GitHub Pages can't serve from a private repo on the free plan).

Currently hosts:

- `ebay-callback.html` — OAuth bridge that catches eBay's HTTPS redirect
  and forwards to the app via the `comicflow://` custom URL scheme.
  See HANDOFF §26.13 in the main repo for context.
