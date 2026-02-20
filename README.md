# hollow knight
## please credit me with a pop up if you use this please.
fixed a lot of stuff and hopefully the full game works.

### Low-end Chromebook Support
To improve compatibility on lower-tier Chromebooks we have:

- Added detection for devices with 2 GB RAM or fewer CPU cores.
- Automatically shrink the WebGL canvas and lower the device pixel ratio.
- Sequentialize asset downloads to reduce simultaneous network/memory pressure.
- Hide the FPS display and other non‑essential UI for better performance.
- Changed the asset base URL to point at the GitHub repository via jsDelivr CDN (`https://cdn.jsdelivr.net/gh/kararh0916/hollow-knight@latest/`)

These changes live in `index.html` and are applied at runtime. No Unity project files are included,
so further optimization requires rebuilding the WebGL export with lower quality settings or
removing unused assets from the scene.

