# Pythagoras-Tree

Pythagoras-Tree is an interactive fractal visualizer. It draws a Pythagoras tree on a 2D canvas with a dark background and gradient coloring, using the browser’s Canvas 2D API and `requestAnimationFrame`.

## Open locally

Open `index.html` in a browser, or start a local server from the project root:

```sh
python -m http.server 8000
```

Then visit <http://localhost:8000>.

## Controls and behavior

The depth slider ranges from 1 to 19, the angle slider from 25° to 65°, and the animation-speed slider from 0.1× to 1×. Changing depth or angle animates the drawing. Randomize changes the angle. Reset returns the sliders to their defaults and restarts the drawing. The canvas layout is recalculated when the window is resized.

The page includes a looping `music.mp3` audio element and a sound-toggle control. Keep `music.mp3` beside `index.html` while its current relative reference is in use, or update that reference if the file moves.

## Files and review

`index.html` contains the visualizer’s markup, styles, and scripts. The supplied files do not list a separate stylesheet or theme configuration. Review the existing code and asset references there before editing.

After changes, try the depth, angle, animation-speed, and randomization controls, then use Reset to check that the drawing restarts. Resize the window to review the canvas layout. No publishing method, deployment configuration, browser compatibility results, or performance results are documented; if publishing, include the audio file if the page still references it and confirm the page and asset load in that context.