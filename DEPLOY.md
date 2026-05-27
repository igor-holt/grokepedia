# Deploying Grokepedia Globally

## Current Status
- GitHub repo: https://github.com/igor-holt/grokepedia
- Main node: `nodes/touching-gods-er-epr.html` (includes full SEO, OG, Twitter, JSON-LD)

## Recommended: Cloudflare Pages (one-command)

Since this project is part of Genesis Conductor infrastructure:

```bash
# From the grokepedia directory
npx wrangler pages deploy . --project-name=grokepedia --branch=main
```

After first deploy, connect the custom domain `grokepedia.x` (or your preferred domain) in the Cloudflare dashboard.

## Alternative: GitHub Pages

1. Enable GitHub Pages on the repo (Settings → Pages)
2. Select "Deploy from a branch" → `main` / root
3. The site will be available at `https://igor-holt.github.io/grokepedia/`

Then update the canonical URLs in the HTML files.

## Quick Local Preview

```bash
npx serve .
```

## Updating Cross-Links

After deployment, update:
- This `DEPLOY.md`
- The HTML canonical URL
- The diamondnode `GROKEPEDIA-CROSS-INDEX.md`
- Any other Genesis Conductor docs

Current live references:
- GitHub: https://github.com/igor-holt/grokepedia
- Diamondnode cross-index: See GROKEPEDIA-CROSS-INDEX.md in the diamondnode repo

## Provenance
prov: x/invariantx/2058116141470425560 ⇄ er-epr
