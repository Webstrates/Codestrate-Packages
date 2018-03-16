<h2>Description</h2><p>Add drawing capabililties to body paragraphs and slides. Latter requires the presentation package.</p><p>The Canvas Mutation Observer code paragraph is run-on-load and observes the codestrate for body paragraphs that have the class canvas. A body paragraph will be upgraded in a canvas when the canvas class is set; and downgraded when the canvas class is removed.<br></p><p>The Pen Tips code paragraph implements a felt pen algorithm that generates felt-pen-like stroke paths.<br></p><p>The Canvas code paragraph modifies a body paragraph of class canvas to allow whiteboard-like drawing. Therefore, it adds a SVG element to the body paragraph, if it does not exist. It further adds event listeners to the body paragraph to listen for pen and eraser events. Currently these events are hard-coded, but may be dynamically assignable by the user. On pen down event, it generates a path and on pen move it generates a stroke based on the pen points. On eraser move events, it checks for intersections of the eraser movement and path elements in the SVG element. If the eraser movement and a path element intersect, the path element will be removed.<br></p>

# Properties

| Property | Value |
| :--- | :--- |
| Name | Canvas |
| ID | Kw6McUkB |
| Version | 1.3.9 |
| Description | Add drawing capabililties to body paragraphs and slides. Latter requires the presentation package. |
| Tags | `tools, body paragraphs` |
| Assets | - |
| Dependencies | `[{"id":"rEpvSgsq","name":"Transformer"}]` |
| Changelog | `{"1.0":"Initital Release","1.1":"Snackbar and Toolbar integration.","1.2":"Update offset on transient-fullscreen.","1.2.1":"Canvas works with presentation package. Add `canvas` class to `slide-content` element.","1.2.2":"Added workaround to make Drawing package work with Presentation package.","1.2.3":"Cleanup remaining tool-palettes before creating new ones.","1.2.4":"Deactivated snackbar button and added 'hide-palette' style.","1.2.5":"Used Commands API.","1.3":"Renamed package to Canvas","1.3.1":"Added context menu to canvas","1.3.2":"Added option to set user specific colors. These colors are stored in anywhere cookies.","1.3.3":"Fixed canvas re-calculating offset when scrolling.","1.3.4":"Dispose event listeners of canvas","1.3.5":"More adjustment of styles when no .canvas class is present","1.3.6":"Dispose context menu","1.3.7":"Adapted to changes in context menu","1.3.8":"Adapted to changes in context menu","1.3.9":"Fixed style for .canvas class not present, but svg.drawing-canvas still render correctly."}` |