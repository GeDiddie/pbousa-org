# Photo Booth Options — pbousa.org

Neon-styled official site for **Photo Booth Options**, the largest custom photo booth manufacturer on the West Coast.

Built from the 2025 marketing deck. Dark background, cyan/magenta/lime neon accents, clean single-page experience.

## Live Domain
**pbousa.org** (registered on Cloudflare)

## Quick Deploy (Recommended: Cloudflare Pages)

Since the domain is already on Cloudflare, this is the cleanest path:

1. Go to [Cloudflare Dashboard](https://dash.cloudflare.com) → **Workers & Pages** → **Create** → **Pages** → **Connect to Git**
2. Select the `GeDiddie/pbousa-org` repository
3. Build settings:
   - Framework preset: **None**
   - Build command: leave empty
   - Build output directory: `/` (or leave default)
4. Deploy
5. Once live, go to the Pages project → **Custom domains** → Add `pbousa.org` and `www.pbousa.org`
6. Cloudflare will automatically handle DNS and free SSL

Done. The site will be live on your domain with global CDN and HTTPS.

### Alternative: GitHub Pages
- Repo Settings → Pages → Source: Deploy from a branch → `main` / root
- Then in Cloudflare DNS add a CNAME for `pbousa.org` → `gediddie.github.io` (or the Pages URL) and follow GitHub’s custom domain docs.

## Form
The contact form currently uses a `mailto:` fallback pointing at `hello@pbousa.org`.  
Once on Cloudflare Pages you can:
- Switch to Cloudflare Forms / Turnstile, or
- Point it to Formspree, Basin, or a simple Worker.

Update the email address in `index.html` before going live.

## Tech
- Pure HTML + CSS + tiny vanilla JS
- Google Fonts: Orbitron (display) + Rajdhani (body)
- Fully responsive
- No build step, no dependencies

## Content Source
Marketing deck: “PBO Marketing Deck - Lease 9_20_25”
- About / manufacturing capacity
- Session flow
- Data collection vs buying lists (stats included)
- 2-seater & 4-seater dimensions
- Lease inclusions

---

Made for G by SuperGrok · Neon mode engaged.
