# Cited

Static landing page for Cited — a Nottingham AI-citation studio. Single-file site: `index.html` at the repository root.

Default GitHub Pages URL after Pages is enabled: `https://jaycooledge85-lgtm.github.io/Cited/`

## Enable GitHub Pages

Pages is not enabled on this repository until you turn it on:

1. Open [Settings → Pages](https://github.com/jaycooledge85-lgtm/Cited/settings/pages).
2. Under **Build and deployment**, set **Source** to **Deploy from a branch**.
3. Set **Branch** to `main` and the folder to `/ (root)`.
4. Click **Save**.
5. Wait a minute, then open `https://jaycooledge85-lgtm.github.io/Cited/`.

The live site is the `index.html` on `main`. Merge this change into `main` before expecting Pages to serve it.

## Custom subdomain

To serve the same site on a custom subdomain (for example `www.yourdomain.com` or `go.yourdomain.com`):

1. In the repo root, add a `CNAME` file whose only line is the hostname (no `https://`).
2. In [Settings → Pages](https://github.com/jaycooledge85-lgtm/Cited/settings/pages), set **Custom domain** to that hostname and save.
3. At your DNS host, add a `CNAME` record from the subdomain to `jaycooledge85-lgtm.github.io`.
4. Wait for DNS to propagate, then tick **Enforce HTTPS** once the certificate is ready.

Apex domains use `A`/`AAAA` records to GitHub’s Pages IPs instead of a `CNAME` — see [GitHub’s custom-domain docs](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site).

## Local preview

```bash
python3 -m http.server 8080
```

Then open `http://localhost:8080/`.
