# Pythagoras-Tree

An interactive fractal visualiser based on the Pythagoras tree. Use the controls to explore recursion depth, angle, animation speed, and randomisation. The reset control restores the visualiser.

## Open locally

Open `index.html` in a browser, or start a local server from the project root:

```sh
python -m http.server 8000
```

Then visit <http://localhost:8000>.

## Editing the experience

The visualiser is in the root-level `index.html`. The repository also includes the root-level audio file `music.mp3`; retain its relative path if replacing the file. No deployment provider or configuration is documented.

For content or appearance changes, inspect the existing markup, styles, and scripts in `index.html` first; no separate theme or stylesheet file is listed. If adjusting the visualiser's appearance, make the change in the existing implementation rather than assuming a separate theme configuration. Keep `music.mp3` beside `index.html` while its current relative reference is in use, or update that reference if the file is moved or renamed.

## Manual review checklist

These are actions to perform after a change, not verified results:

- Open `index.html` or the local server URL and inspect the visualiser.
- Try the recursion-depth, angle, animation-speed, and randomisation controls. Then use reset and check that the visualiser returns to its reset state.
- Inspect the visualiser and its controls at narrow mobile-sized and wide desktop-sized viewports. Check that the drawing remains visible and that controls can be reached without clipping or overlap.

## Asset and loading review checklist

These are review steps, not measured performance results or claims that assets have been checked:

- Check the `music.mp3` reference in `index.html` against the file beside it. If the file moves or is renamed, update the reference and review the audio behavior.
- Search `index.html` for local image, audio, font, and other media references. Verify each path against the intended local file; the supplied root-file list identifies `music.mp3` but does not enumerate references within the page.
- Review the audio file size and any referenced image dimensions and file sizes. Consider whether large media can be reduced without losing needed quality; no sizes have been measured here.
- Before removing a local file, check whether the page still references it. Keep the active asset set limited to resources the visualiser uses, while retaining any source files that are intentionally part of the project.
- No external font or script links are listed in the supplied link information. Inspect `index.html` before concluding there are none, and verify that any external dependency found or added is intentional and has suitable fallback behavior.
- After asset changes, review the visualiser and its controls, including behavior if an audio or other referenced resource cannot load.

## Accessibility review checklist

These are future checks to perform after a change; they are not claims that the page has been tested or found accessible:

- Use the keyboard to reach and operate recursion-depth, angle, animation-speed, randomisation, and reset controls. Check that focus order follows the visual and reading order and that every action is possible without a pointer.
- Check that each control has a meaningful accessible name, and that value changes can be understood without relying on the drawing alone. Check that keyboard focus remains visible while the tree changes.
- Review text, control, and focus-indicator contrast. If the tree's colors distinguish branches or states, check that the distinction is also available without color alone.
- Check whether the fractal drawing has a text alternative or explanation that conveys its relevant content. If images are added, provide appropriate alternatives for informative images and avoid redundant alternatives for decorative ones.
- Review the animation-speed control and any other motion for a way to pause or reduce movement. Check behavior with reduced motion requested and whether the visualiser remains usable without animation.
- If `music.mp3` is played by the page, check that audio controls are keyboard reachable and meaningfully named, and that sound is not the only way to understand a state or action.