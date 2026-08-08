# hybridhelix-net-redirect

Temporary GitHub Pages site that redirects `hybridhelix.net` → `https://hybridhelix.consulting`.

## Why this exists

The primary HybridHELIX website lives at `hybridhelix.consulting`. The `.net` domain needs to redirect there with proper HTTPS (no browser security warnings). This repo provides that via GitHub Pages' free SSL provisioning.

## When to remove

This repo becomes unnecessary at the **Website 4.0 root-domain cutover** (rail 50), when the full site begins serving directly from `hybridhelix.net`. At that point, update DNS to point at the production site repo and archive or delete this one.

## Files

| File | Purpose |
|------|--------|
| `index.html` | Instant redirect via meta-refresh + JS |
| `404.html` | Catches all subpaths and redirects them too |
| `CNAME` | Tells GitHub Pages this site serves `hybridhelix.net` |