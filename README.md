# mariewoodson-apex-redirect

Apex redirect only. The GitHub Pages A records (185.199.108-111.153) on
`mariewoodson.com` point here, and every request is bounced to `https://www.mariewoodson.com`, which is
the Cloudflare Pages site.

DNS for this domain lives at Wix. **MX is IONOS (mx00/mx01.ionos.com) and must never be touched.**

Both `index.html` and `404.html` carry the same redirect: GitHub Pages serves
`index.html` only for `/`, so without `404.html` every deep link into the apex
would land on GitHub's own 404 page instead of the site.
