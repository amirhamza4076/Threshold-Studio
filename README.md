# Photoshop Threshold Studio

A browser-based image threshold editor with a Photoshop-inspired dark interface.

## Features

- Open images from your device or drag and drop them into the workspace
- Adjust threshold level from 0 to 255
- Choose Rec. 601, Rec. 709, average, or individual RGB channels
- Apply pre-blur for basic noise reduction
- Invert the threshold output
- Compare the original and processed image with split view
- View a luminance histogram and black/white pixel ratios
- Zoom toward cursor, pan, pinch-to-zoom, and export the result as PNG
- 3-dot menu for presets, view controls, reset, and about
- Slider focus mode: chrome fades while you drag threshold or blur so the image stays clear
- Automatic downscale for very large images (dimension / pixel-count guard)
- Keyboard shortcuts:
  - `+` or `=`: zoom in
  - `-`: zoom out
  - `0`: fit image to screen
  - `1`: 100% zoom
  - `Esc`: close menus

## Run locally

No build step is required.

1. Download or clone this repository.
2. Open `index.html` in a modern browser.
3. Choose an image and start editing.

For the sample presets and external icons/fonts to load, an internet connection is required. Local image editing does not upload images to a server; processing happens in the browser.

## GitHub Pages

This repository is a static website and can be hosted with GitHub Pages:

1. Open the repository on GitHub.
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Select the `main` branch and `/ (root)` folder.
5. Save and wait for the Pages deployment to finish.

Your site will be available at `https://YOUR-USERNAME.github.io/REPOSITORY-NAME/`.

## Mobile support

The interface adapts to phones and tablets with a stacked editing workspace, larger touch targets, portrait and landscape layouts, one-finger canvas panning, and two-finger pinch-to-zoom. The adjustment panel remains below the canvas on narrow screens.

## Technology

- HTML
- CSS
- Vanilla JavaScript
- HTML Canvas API
- Tailwind CSS CDN
- Font Awesome CDN

## Notes

- The application uses external CDN resources for Tailwind CSS, Font Awesome, and Google Fonts.
- Images above ~12 megapixels or 6000px on a side are automatically downscaled for stability.
- Very large images may still exceed browser canvas or memory limits on low-end devices.
- This project is a standalone browser tool; it does not require a backend.

## License

MIT License — see `LICENSE`.
