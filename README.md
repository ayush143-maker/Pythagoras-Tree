# Pythagoras-Tree

An interactive fractal visualiser based on the Pythagoras tree. Use the controls to explore recursion depth, angle, animation speed, and randomisation. Reset restores the visualiser.

## Open locally

Open `index.html` in a browser, or start a local server from the project root:

```sh
python -m http.server 8000
```

Then visit <http://localhost:8000>.

## Configuration and data

This repository is a static page: the supplied files include `index.html` and `music.mp3`, and no environment template or backend configuration is listed. The page runs in the browser, so values placed in its HTML, scripts, styles, or other delivered files are public—not secrets. Do not put credentials or private data in tracked files. If configuration is added later, keep its template free of real secret values and keep any actual secrets out of version control. The page's visible behavior does not imply that it securely stores or transmits data.

## Editing the experience

The visualiser is in the root-level `index.html`. Keep `music.mp3` beside it while the current relative reference is in use, or update that reference if the file is moved or renamed. Review the existing markup, styles, and scripts before editing; no separate stylesheet or theme configuration is listed.

## Manual review checklist

These are actions to perform after a change, not verified results:

- Open `index.html` or the local server URL and inspect the visualiser.
- Try the recursion-depth, angle, animation-speed, and randomisation controls. Use reset and check whether the visualiser returns to its reset state.
- Check that `music.mp3` and any other referenced local resources resolve. Inspect the page for remote requests and review their behavior if a resource is unavailable.
- Compare narrow mobile-sized and wide desktop-sized viewports for clipping or overlap. Review relevant browsers and the developer console; no compatibility or performance results are reported here.
- Use the keyboard to operate controls, check visible focus and meaningful accessible names, and review contrast and motion behavior, including whether movement can be reduced or paused.
- If the page plays `music.mp3`, check that audio controls are keyboard accessible and clearly named.

## Assets

Before moving or removing a file, check references in `index.html`. Review media sizes and image dimensions if assets are added; no asset sizes or performance measurements are reported here. Keep the audio file's relative path aligned with its reference.