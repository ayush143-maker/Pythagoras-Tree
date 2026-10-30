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
- Check that `music.mp3` and any other changed image or media references resolve from the paths used in `index.html`. Review the audio behavior if you changed its file or reference.
- Inspect the visualiser and its controls at narrow mobile-sized and wide desktop-sized viewports. Check that the drawing remains visible and that controls can be reached without clipping or overlap.

## Accessibility review checklist

These are future checks to perform after a change; they are not claims that the page has been tested or found accessible:

- Use the keyboard to reach and operate recursion-depth, angle, animation-speed, randomisation, and reset controls. Check that focus order follows the visual and reading order and that every action is possible without a pointer.
- Check that each control has a meaningful accessible name, and that value changes can be understood without relying on the drawing alone. Check that keyboard focus remains visible while the tree changes.
- Review text, control, and focus-indicator contrast. If the tree's colors distinguish branches or states, check that the distinction is also available without color alone.
- Check whether the fractal drawing has a text alternative or explanation that conveys its relevant content. If images are added, provide appropriate alternatives for informative images and avoid redundant alternatives for decorative ones.
- Review the animation-speed control and any other motion for a way to pause or reduce movement. Check behavior with reduced motion requested and whether the visualiser remains usable without animation.
- If `music.mp3` is played by the page, check that audio controls are keyboard reachable and meaningfully named, and that sound is not the only way to understand a state or action.