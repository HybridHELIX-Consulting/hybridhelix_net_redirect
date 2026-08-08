# hybridhelix-net-redirect

GitHub Pages site that redirects `hybridhelix.net` → `https://hybridhelix.consulting`.

## Purpose

The primary HybridHELIX website lives at `hybridhelix.consulting`. This repo provides a clean HTTPS redirect from the `.net` domain via GitHub Pages' free SSL provisioning.

## Files

| File | Purpose |
|------|--------|
| `index.html` | Branded redirect page with logo, company name, and tagline |
| `404.html` | Catches all subpaths and redirects them |
| `CNAME` | Tells GitHub Pages this site serves `hybridhelix.net` |
| `logo.png` | HybridHELIX logo displayed on the redirect page |

## DNS Requirements

For the site to work, the following DNS records must be set for `hybridhelix.net`:

- Four **A records** for `@`: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
- **CNAME** for `www` → `hybridhelix-consulting.github.io`
- **Enforce HTTPS** enabled in GitHub Pages settings
