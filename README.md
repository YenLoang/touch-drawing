# Touch Drawing App 🎨

A mobile-friendly drawing app built with vanilla HTML, CSS, and JavaScript
using the Canvas API and Pointer Events.

**Live demo:** https://<your-username>.github.io/touch-drawing/
(best on a phone!)

## Features
- Draw with your finger, mouse, or stylus
- Cycle through pen colors
- Eraser mode
- Undo / redo (stack-based, up to 50 steps)
- Clear canvas (undoable)
- Responsive toolbar that fits any screen

## How it works
- **Pointer Events** handle touch, mouse, and stylus with one API
- **Canvas 2D** draws strokes with `lineTo` / `stroke`
- **Eraser** uses `globalCompositeOperation = 'destination-out'`
- **Undo/redo** saves canvas snapshots (`getImageData`) onto two stacks

## Run locally
python -m http.server 8000
Then open http://localhost:8000
