# Pythagoras-Tree

An interactive fractal visualiser based on the Pythagoras tree. Use the controls to explore recursion depth, angle, animation speed, and randomisation. The reset control restores the visualiser.

## Open locally

Open `index.html` in a browser, or start a local server from the project root:

```sh
python -m http.server 8000
```

Then visit <http://localhost:8000>. After changing the visualiser, try the controls and reset to review the result. If the accompanying audio is unavailable, check that `music.mp3` remains at the referenced relative path.

## Editing the experience

The visualiser is in the root-level `index.html`. The repository also includes the root-level audio file `music.mp3`; retain its relative path if replacing the file. No deployment provider or configuration is documented.