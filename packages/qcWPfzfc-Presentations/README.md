<h2>Description</h2><p>This package makes it possible to create slides and presentations in Codestrates.</p><h2>Slides</h2><h4>Adding Slides</h4><p>Slides can be added to the Codestrate by using the "Add Slide" button in the global toolbar.</p><h4>Converting to Slides</h4><p>Body paragraphs can be converted to a slide (and vice versa). This is done by selecting a body-paragraph and then using the "Toggle Slide" button in the snackbar.</p><h4>Aspect Ratio of Slides</h4><p>Slides by default have an aspect ratio of 16:9. The aspect ratio can be changed by adding a <code>aspect-x-y</code> class to a slide paragraph. The following aspect ratios are supported: <code>aspect-4-3</code>, <code>aspect-16-10</code> and <code>aspect-1-1</code>.</p><h2>Presentations</h2><h4>Start Presentation from Start</h4><p>A presentation can be started from the first slide on by using the "Start Presentation" button in the global toolbar. A presentation can also be started from the start by pressing <kbd>Ctrl</kbd>+<kbd>Enter</kbd> or <kbd>F5</kbd> while no slide is selected.</p><h4>Start Presentation from a Specific Slide</h4><p>A presentation can also be started from a specific slide. This is done by selecting the slide and pressing the "Start Presentation" button in the snackbar. A presentation can also be started from a specific slide by pressing <kbd>Ctrl</kbd>+<kbd>Enter</kbd> or <kbd>F5</kbd> while the slide is selected.</p><h4>Exit a Presentation</h4><p>To exit a presentation press <kbd>Esc</kbd> or <kbd>Ctrl</kbd>+<kbd>Enter</kbd> or <kbd>F5</kbd> during a presentation.</p><h3>Navigating Slides</h3><p>To go to the next or previous slides use the <kbd>&lt;-</kbd> and <kbd>-&gt;</kbd> arrow keys or <kbd>Page Up</kbd> and <kbd>Page Down</kbd>.</p><h3>Slide Notes</h3><p>To toggle slide notes during press <kbd>Ctrl</kbd>+<kbd>K</kbd> during a presentation.</p><h2>Heavy Content</h2><p>In the context of this package, heavy content means iframes or scripts or videos, which should be executed lazy, i.e. when the slide comes up or shortly before and be again removed afterwards. To facilitate these kind of loading this package provides slide scripts and <code>&lt;slide-content&gt;</code> elements to do so.</p><h3>Slide Scripts</h3><p>A slide script is a script, which has the same ID as a slide paragraph followed by <code>-script</code> and provides three functions for three slide states. A newly created script looks as follows:</p><pre><code>// Called on slide preload
exports.preload = (paragraph, slide) =&gt; {
  // Your code...
};

// Called on slide enter
exports.enter = (paragraph, slide) =&gt; {
  // Your code...
};


// Called on slide exit
exports.exit = (paragraph, slide) =&gt; {
  // Your code...
};</code></pre><p>As the comments suggest, the three functions will either be called when the slide comes up (<code>.enter</code>), is left (<code>.exit</code>) or when the slide before the one of the script is opened (<code>.preload</code>).</p><h3><code>&lt;slide-content&gt;</code> Element</h3><p>When one just wants to lazy load an HTML element into a slide, one can use the <code>&lt;slide-content&gt;</code> Element:</p><pre><code>&lt;slide-content&gt;
  &lt;template event="preload"&gt;&lt;/template&gt;
  &lt;template event="enter"&gt;&lt;/template&gt;
  &lt;template event="exit"&gt;&lt;/template&gt;
  &lt;render-to&gt;&lt;/render-to&gt;
&lt;/slide-content&gt;</code></pre><p>This element will render the contents of the <code>&lt;template&gt;</code> elements into the <code>&lt;render-to&gt;</code> element on the same slide states as described in slide scripts.</p><h2>Transient Presentation (experimental)</h2><p>When starting a presentation it is started persistent, i.e. on every client. When one wants to preview a presentation or leave a presentation just on the local client, one can add the <kbd>Alt</kbd> key to the shortcuts from above (e.g. <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>Enter</kbd>) in order to do that. An orange border indicates, that the presentation is started (or left) just on the local client.</p><p><b>Warning</b>: This is an experimental function, so some things like presentation scripts or <code>&lt;slide-content&gt;</code> are not loading.</p>

# Properties

| Property | Value |
| :--- | :--- |
| Name | Presentations |
| ID | qcWPfzfc |
| Version | 1.0.19 |
| Description | Makes it possible to create slides and presentations. |
| Tags | `tools, body paragraphs` |
| Assets | `presentation_pointer.png` |
| Dependencies | `[{"id":"jFx9fAE8","name":"Text Tools","optional":true,"usage":"Text tools provides valuable text formatting capabilities for slides."}]` |
| Changelog | `{"1.0.19":"Added text tools as optional dependency.","1.0.18":"Fixed issue with table header (thead) rendering multiple times within table body when printing presentation slides.","1.0.17":"New indicator for transient hidden presentation.","1.0.16":"Extended basic style.","1.0.15":"Pull classes from content into slide-content and convert slide back without notes.","1.0.14":"Fixed scaling in paragraphs, added 'basic' class for basic slide styles.","1.0.13":"Fixed printing CSS.","1.0.12":"Added documentation and new description.","1.0.11":"Fixed fullscreen scaling by using 'window.innerWidth'.","1.0.10":"Update slide numbers when creating slides.","1.0.9":"Fixed scaling bug when first slide is hidden.","1.0.8":"Always show slide number.","1.0.7":"Fixed slide flex direction.","1.0.6":"Added transient element as wrapper around heavy slide content. Fixed comment in slide script template.","1.0.5":"Added add heavy slide content button to snackbar content editor.","1.0.4":"Added persistent styles to package.","1.0.3":"Fixed slide notes text color in other themes.","1.0.2":"Added print slide style.","1.0.1":"Fixed slide scaling when first slide is added and debounced slide scaling on window resize.","1.0":"Initial version."}` |