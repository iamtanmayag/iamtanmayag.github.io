# Tanmay Agrawal — Engineering Portfolio

Production AI, backend and cloud engineering portfolio. Built as an accessible, dependency-free static site with six detailed case studies.

## GitHub Pages deployment

1. Create the **public** repository `iamtanmayag.github.io` under `iamtanmayag`.
2. Upload/commit the **contents of this directory to the repository root** (`index.html`, `assets/`, `work/`, `.nojekyll`, etc.). Do not upload the ZIP itself as a single file.
3. Open **Settings → Pages → Build and deployment** and select **Deploy from a branch → main → /(root)**. Save.
4. When deployed, visit `https://iamtanmayag.github.io/`. GitHub may need a few minutes to publish.
5. On a future custom domain, add it in **Settings → Pages** before configuring your domain's DNS; update `SITE_URL` in `src/build_site.py` and regenerate site URLs.

## Development

No installation or build required. Preview locally:

```bash
python -m http.server 8000
```

Visit http://localhost:8000/ and navigate all six case studies. The HTML/CSS/JS are at repository root, `assets/`, and `work/`. To regenerate pages after content edits, modify `src/build_site.py` and run `python src/build_site.py`; you can also edit generated HTML directly, but later regeneration will overwrite direct edits.

The current social links target [GitHub](https://github.com/iamtanmayag) and [LinkedIn](https://www.linkedin.com/in/tanmay-agrawal-23102320a/).

## Security and privacy

This is a **public** website and public source repository. It contains no proprietary source code, access credentials, internal customer data, or unredacted company diagrams. Case studies describe generalized engineering work. The included PDF résumé contains personal contact information; review it before making the repository public.

GitHub Pages serves this site as static files. GitHub Pages does not support Cloudflare's `_headers` file, so it is intentionally omitted from this package. `.nojekyll` tells Pages to serve the files as-is.
