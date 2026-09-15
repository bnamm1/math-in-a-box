# Math in a Box — website

A single self-contained page (`index.html`). No build step, no dependencies beyond Google Fonts.

## Publish on GitHub Pages

1. Create a repo (e.g. `math-in-a-box-site`) and push these files to its `main` branch.
2. Settings → Pages → Source: "Deploy from a branch", branch `main`, folder `/ (root)`.
3. The site goes live at `https://<username>.github.io/math-in-a-box-site/` within a minute or two.

## Custom domain

1. Buy the domain (Cloudflare Registrar, Porkbun, Namecheap — any registrar works).
2. Replace the contents of `CNAME` with the bare domain, e.g. `mathinabox.org` (one line, no `https://`).
3. At the registrar add DNS records:
   - `A` records for the apex (`@`) → `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - `CNAME` record for `www` → `<username>.github.io`
4. Settings → Pages → Custom domain: type the domain, save, wait for the DNS check, then tick "Enforce HTTPS".

## Editing

Everything is in `index.html`: styles at the top, then one `<section>` per part of the site
(story, what's inside, the year, history, team, partners, get involved, contact).
The contact address is in the `#contact` section.
