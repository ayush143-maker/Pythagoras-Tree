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

## Deployment-readiness checklist

The supplied project files identify a root-level `index.html` and `music.mp3`; they do not document a publishing method or deployment configuration. The items below are recommendations to check for the publishing method you choose, not verified deployment results.

- [ ] Confirm the publishing setup serves the directory containing `index.html` as the site root, or configure its output/root directory so the published page is available at the intended address. Do not assume a build step or generated output directory that is not present in this project.
- [ ] Ensure `music.mp3` is included alongside `index.html` if the page still refers to it with its current relative path. Check the reference in `index.html` if either file is moved or renamed.
- [ ] Review the page and its references for local-only paths, machine-specific values, or configuration that should not be published. The supplied project files do not document deployment-specific settings.
- [ ] After publishing, open the actual published page in a browser. Check that the page loads, the visualiser and its controls work, and the audio file loads if the page uses it. Check the browser Console and Network panel for errors or failed requests.
- [ ] Repeat the preview at narrow and wide viewports and with keyboard navigation; check for clipping, overlap, visible focus, and accessible control names.

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

## Final release review

- Open `index.html` from the published location and confirm the page loads as expected.
- Review the published result once on a narrow screen and once on a wider screen; treat this as a release check, not an automated test report.
