# Pythagoras-Tree

Pythagoras-Tree is an interactive fractal visualizer based on the Pythagoras tree. Its controls let you explore recursion depth, angle, animation speed, and randomization; Reset restores the visualizer.

## Open locally

Open `index.html` in a browser, or start a local server from the project root:

```sh
python -m http.server 8000
```

Then visit <http://localhost:8000>.

## Files and editing

- `index.html` — visualizer entry point, including its markup, styles, and scripts.
- `music.mp3` — audio asset in the project root. Keep it beside the page while its current relative reference is in use, or update the reference if the file moves.

Review the existing markup, styles, scripts, and asset references in `index.html` before editing. The supplied files do not list a separate stylesheet or theme configuration.

## Review notes

After changes, try the recursion-depth, angle, animation-speed, and randomization controls, then use Reset and check the result. Compare narrow and wide viewports for clipping or overlap, and use keyboard navigation to review control operation and visible focus. If the page uses `music.mp3`, check that its audio controls are accessible and clearly named.

No publishing method, deployment configuration, browser compatibility results, or performance results are documented. If publishing, serve the directory containing `index.html` and include `music.mp3` if the page still references it. Confirm the page and asset load in the published context.