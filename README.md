# MagicEraser

A small browser-based object removal demo inspired by the MagicEraser paper.

Live demo: https://krrishkhanna.github.io/magiceraser/

The app lets a user load an image, mark the object they want to remove, and compare a simple fill against a context-aware fill. Everything runs in the browser, so there is no backend or model server to set up.

## Features

- upload your own image or use one of the built-in sample scenes
- paint, erase, grow, shrink, invert, and undo/redo masks
- auto-mask for the sample scenes and a basic saliency fallback for uploads
- compare original, naive fill, smart fill, and split view
- tune context radius, blending, texture, and mask opacity
- download the final result as a PNG

## Running Locally

Open `index.html` directly in a browser, or serve the folder locally:

```bash
python3 -m http.server 8000
```

Then visit:

```text
http://127.0.0.1:8000/
```

## Notes

This is a lightweight demo, not a full reproduction of the research model. The current version uses canvas-based masking and context-based filling so the complete workflow can be shown without GPU dependencies. The built-in samples are designed to make the comparison easy to explain during a presentation.

More detailed implementation notes are in [DEMO_STRATEGY.md](DEMO_STRATEGY.md).
