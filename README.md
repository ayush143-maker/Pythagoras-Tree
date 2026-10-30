# Pythagoras-Tree

Pythagoras-Tree is an interactive fractal visualiser based on the Pythagoras tree. It lets visitors explore how the branching pattern changes through controls for recursion depth, angle, animation speed, randomisation, and reset.

## Open locally

The project is delivered as a standalone HTML page. Open index.html in a modern browser, or serve it locally:

    python -m http.server 8000

Visit http://localhost:8000 to explore the visualiser.

## Experiment with the controls

Try changing one parameter at a time to see how it affects the shape of the tree. When updating the drawing logic, keep the controls responsive and provide a reliable reset path so the visitor can return to a known starting state. The repository also includes music.mp3 as a local asset; preserve its relative path if you replace it.
