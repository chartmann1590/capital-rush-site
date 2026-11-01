# CAPITAL RUSH website

The marketing site for CAPITAL RUSH, an open-world crime game on the real streets of the New York Capital Region, free in the browser.

**Live:** https://chartmann1590.github.io/capital-rush-site/ · **Play:** https://chartmann1590.github.io/capital-rush-site/play/

- `index.html` and `img/`: the page and its stills, all captured from the game.
- `media/hero-loop.mp4` plays behind the title. The trailer streams as HLS from `media/trailer/` (a 1080p and a 720p ladder in two-second pieces, so no file in the repo is large); Safari plays it natively and other browsers load `media/hls.light.min.js` (hls.js, Apache-2.0) when the trailer comes into view.
- `play/` is the game itself: the `vite build` output of the game repo, with relative asset paths so it runs from this subpath. `data/world.json` is left out: the game streams the tiled region bake in `play/data/region/` instead.

Published with GitHub Pages from the `main` branch.
