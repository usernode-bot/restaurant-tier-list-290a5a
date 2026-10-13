# Restaurant Tier List brand files

**Glyph:** a fork standing beside three stepped tier-ranking bars. The bars
run from longest at the top to shortest at the bottom, like a ranking; the
top bar, the best tier, is yellow. Flat, no text.

**Colours:** brand Black `#000000`, Cream `#FFFEEA`, Yellow `#FFEE6F` only,
in the Homeroom brand pairings Cream + Black and Yellow + Black.

**Files**

- `icon.svg` → `icon.png` (1024 × 1024, opaque RGB) — the app icon, declared
  as `icon.image` in `dapp.json`. The 📊 emoji stays declared as the fallback.
- `featured-light.svg` → `featured-light.png` (1600 × 900) — featured
  illustration, light look: black mark on cream. No yellow, since yellow on
  cream is not a brand pairing.
- `featured-dark.svg` → `featured-dark.png` (1600 × 900) — featured
  illustration, dark look: cream mark with the yellow top bar on black, same
  as the app icon.

The featured illustration has no `dapp.json` field that publishes it; the
files are kept here for whoever manages the app's Homeroom directory listing.

**How the PNGs are made:** rasterized from the SVG sources in this directory
with a throwaway renderer (rounded rectangles, 4× supersampling, standard
Python `zlib`/`struct`). Redraw the SVG first, then re-render.
