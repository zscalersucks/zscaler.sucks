# zscaler.sucks

A parody site. The headlines agree with every complaint about Zscaler; the answers explain, with great sympathy, why each complaint is technically wrong. The site owner actually likes the product. This is a love language.

## Structure

Plain static site — no build step, no dependencies.

- `index.html` — the whole site (styles inline, light/dark aware)
- `CNAME` — custom domain for GitHub Pages
- `.nojekyll` — skips Jekyll processing

## Deploying to GitHub Pages

1. Push this repo to GitHub.
2. Repo → Settings → Pages → Source: **Deploy from a branch**, branch `main`, folder `/ (root)`.
3. DNS for `zscaler.sucks` (apex domain) — add A records pointing to GitHub Pages:
   - `185.199.108.153`
   - `185.199.109.153`
   - `185.199.110.153`
   - `185.199.111.153`
   - (optional AAAA: `2606:50c0:8000::153` … `2606:50c0:8003::153`)
4. Back in Settings → Pages, set custom domain `zscaler.sucks` and enable **Enforce HTTPS** once the cert issues.

Local preview: just open `index.html` in a browser.
