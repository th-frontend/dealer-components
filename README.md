# 360° House Viewer

This project demonstrates a simple 360° image viewer implemented with vanilla Web Components. A sequence of images is displayed in the `<product-viewer-360>` element, allowing the user to click and drag to rotate around a house. Interactive hotspots can be placed on the model to reveal additional information.

## Features

- Drag or use auto‑rotate to spin the house model
- Loading progress indicator while frames are fetched
- Play/Pause and Reset controls
- Hotspots that can follow specific frames and show modal descriptions
- Images loaded via a URL pattern, so the viewer can work with any numbered sequence

## Running

No build step is required. Simply open [`house/index.html`](house/index.html) in a modern browser or serve the folder with a static server:

```bash
npx serve house
```

The viewer pulls the image sequence from a Treehouse CDN, so an internet connection is required.

## Customizing

`<product-viewer-360>` accepts several attributes:

- `width`/`height` – viewer dimensions
- `images` – number of frames in the sequence
- `auto-rotate` – `true` or `false` to spin automatically
- `rotation-speed` – frames per second when auto‑rotating
- `image-url-pattern` – pattern for the image URLs. Use `{frame}` as a placeholder for the padded frame number
- `frame-padding` – number of digits used in filenames
- `start-frame` – starting index used when generating the image URLs

Hotspots are created with the `<product-hotspot>` element. Position them using `x` and `y` (percentages). A `positions` attribute can provide frame‑based coordinates so a hotspot moves with the object while rotating.

See [`house/index.html`](house/index.html) for an example configuration with two hotspots.

