<h2>Vega Lite Plotting</h2><p>Adds a <code>vplot</code> and <code>vplotlive</code> function to the global scope that can be used to plot using <a href="https://vega.github.io/vega-lite/" target="_blank">Vega Lite</a>.</p><p><code>vplot</code> renders a static plot, while <code>vplotlive</code> takes a reference to a data paragraph, and updates when the spec in the data paragraph is changed.</p>

# Properties

| Property | Value |
| :--- | :--- |
| Name | Vega Lite Plotting |
| ID | KX9BMP3y |
| Version | 0.4.3 |
| Description | Vega and Vega Lite plotting package. Adds global vplot function. |
| Tags | `function, code paragraphs` |
| Assets | `vega.js, vega-lite.js, vega-embed.js, seattle-weather.csv` |
| Dependencies | `[{"id":"qRcedryV","name":"Output"}]` |
| Changelog | `{"0.4.3":"Fixed styling of documentation.","0.4.2":"Fixed bug that prevented the vega lite package from initialize correctly.","0.4.1":"'this' in vplot and vplotlive now correctly refers to the calling paragraph.","0.4":"Added vplotlive and support for outputting to an element with a given id","0.3":"Added support for output target with CSS selector","0.2":"Multi-user support","0.1":"Initial version."}` |