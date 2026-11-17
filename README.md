# Illinois Land Index legacy dashboard redirect

This small GitHub Pages site sends visitors from `dashboard.illinoislandindex.com` to `https://illinoislandindex.com/parcel-dashboard/`.

- `index.html` handles the root address.
- `404.html` provides the same transition for old login links and other retired paths.
- The fixed destination drops old paths, query parameters, and fragments.
- The page contains no analytics, cookies, forms, parcel records, or credentials.
- Browser navigation uses `location.replace`, with a meta-refresh and visible link as fallbacks. This is not an HTTP 301 redirect.
- DNS uses GitHub Pages A records so the existing Google verification TXT record can stay at the same hostname.

The public parcel dashboard continues to live in the separate `plummer92/illinois-land-index` repository. Do not change its custom domain.
