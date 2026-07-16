# Bright ADeaS — Website

Scroll-driven single-page website for **Bright ADeaS**, a signage, printing and
fabrication workshop in Silang, Cavite, Philippines.

**Live concept:** the storefront neon sign disassembles as you scroll — letters
fly apart in 3D to reveal a fabrication blueprint, followed by an exploded view
of a built-up letter's four layers (acrylic face, LED array, aluminum returns,
backplate). *"We build signs from the inside out."*

## Structure

| Path | Purpose |
|------|---------|
| `index.html` | The entire site — HTML, CSS and JS in one self-contained file. No frameworks, no build step. |
| `Products/` | Portfolio photos of real client installations, referenced by the gallery section. |

The only external dependency is Google Fonts (Montserrat, Space Grotesk, Pacifico).

## Deploying on Cloudflare Pages

1. Cloudflare dashboard → **Workers & Pages → Create → Pages → Connect to Git**
2. Select this repository (`A2conceptdesigns/BrightAds`), branch `main`
3. Settings:
   - **Framework preset:** None
   - **Build command:** *(leave empty)*
   - **Build output directory:** `/`
4. Deploy. Every push to `main` auto-redeploys.

## Updating the site

- **Content/design:** edit `index.html`, commit, push.
- **Portfolio:** drop new photos into `Products/` and add a card in the
  "Signs we've already switched on" section of `index.html`.
- **Preview locally:** just open `index.html` in a browser (all paths are relative).

### Handy URL parameters

- `?sp=0.5` — deep-link to a scroll position (0–1 through the whole page)
- `?hp=0.5` / `?ap=0.5` — force the hero disassembly / letter-explosion progress (design QA)

## Contact

- Email: bright.ads.ph@gmail.com
- Facebook: [fb.com/bright.adeas.9](https://www.facebook.com/bright.adeas.9)
