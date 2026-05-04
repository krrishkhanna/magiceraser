# MagicEraser

Implementation strategy: [DEMO_STRATEGY.md](/Users/kkk/magiceraser/DEMO_STRATEGY.md)

Working local website: [index.html](/Users/kkk/magiceraser/index.html)

Open `index.html` in a browser to use the object-removal studio. It runs fully in the browser and includes:

- image upload and built-in sample scenes,
- paint and erase mask tools,
- undo and redo for mask edits,
- adjustable brush, mask overlay, context radius, blending, and texture controls,
- naive fill and context-aware smart fill,
- original / naive / smart / split comparison views,
- live previews and PNG export.

What it proves:

- even without a full diffusion model, using surrounding scene context gives better erasure than a flat baseline.
