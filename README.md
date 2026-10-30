# Pythagoras-Tree

An interactive fractal visualiser based on the Pythagoras tree. Use the controls to explore recursion depth, angle, animation speed, and randomisation. Reset restores the visualiser.

## Open locally

Open `index.html` in a browser, or start a local server from the project root:

```sh
python -m http.server 8000
```

Then visit <http://localhost:8000>.

## Editing the experience

The visualiser is in the root-level `index.html`. Keep `music.mp3` beside it while the current relative reference is in use, or update that reference if the file is moved or renamed. Review the existing markup, styles, and scripts before editing; no separate stylesheet or theme configuration is listed.

## Configuration and data

The supplied files include `index.html` and `music.mp3`, with no environment template or backend configuration listed. The page runs in the browser, so values placed in its HTML, scripts, styles, or other delivered files are public—not secrets. Do not put credentials or private data in tracked files. The page's visible behavior does not imply that it securely stores or transmits data.

## Troubleshooting

Use these as diagnostic steps; they are not reports of known failures:

1. Confirm `index.html` is the intended entry page.
2. If the visualiser or audio is missing, check the references in `index.html` and confirm the required local files are present. Keep `music.mp3` beside the page unless its relative reference is updated.
3. Preserve relative paths when moving or renaming files. Compare the requested path in the browser's Network panel with the file location in the repository.
4. Inspect the browser Console and Network panel for script errors, failed local requests, or unexpected requests while using the controls.
5. No external resource links are listed in the supplied files. If you find a remote reference in `index.html`, distinguish that network-dependent resource from local files when diagnosing a load issue.

## Manual review checklist

These are actions to perform after a change, not verified results:

- Try the recursion-depth, angle, animation-speed, and randomisation controls. Use reset and check whether the visualiser returns to its reset state.
- Compare narrow mobile-sized and wide desktop-sized viewports for clipping or overlap. Review relevant browsers; no compatibility or performance results are reported here.
- Use the keyboard to operate controls, check visible focus and meaningful accessible names, and review contrast and motion behavior, including whether movement can be reduced or paused.
- If the page plays `music.mp3`, check that audio controls are keyboard accessible and clearly named.
- Before moving or removing a file, check its references in `index.html`. Consider media sizes if assets are added; no asset sizes or performance measurements are reported here.