# Pythagoras-Tree

An interactive fractal visualiser based on the Pythagoras tree. Use the controls to explore recursion depth, angle, animation speed, and randomisation. Reset restores the visualiser.

## Open locally

Open `index.html` in a browser, or start a local server from the project root:

```sh
python -m http.server 8000
```

Then visit <http://localhost:8000>.

## Files and editing

The visualiser is in the root-level `index.html`; `music.mp3` is also in the project root. Keep the audio file beside the page while its current relative reference is in use. If you move or rename either file, update the relevant reference in `index.html`.

Review the existing markup, styles, and scripts in `index.html` before editing. The supplied files do not list a separate stylesheet or theme configuration.

## Contributor handoff

Keep each change focused on the visualiser or the specific issue being addressed. Preserve existing filenames and relative references unless a change requires updating them, and update every affected reference when moving or renaming a file. In your handoff, describe what changed and which files were affected.

Before publishing, manually review the changed page in a browser. The checklist below is for review; it is not a report of completed checks or verified results.

## Manual review checklist

- Try the recursion-depth, angle, animation-speed, and randomisation controls. Use reset and check whether the visualiser returns to its reset state.
- Compare narrow and wide viewports for clipping or overlap.
- Use the keyboard to operate controls; check visible focus, accessible names, contrast, and motion behavior.
- If the page plays `music.mp3`, check that audio controls are keyboard accessible and clearly named.
- Check the browser Console and Network panel for errors or failed requests, and confirm that local file paths still match after edits.

No browser compatibility or performance results are reported here.