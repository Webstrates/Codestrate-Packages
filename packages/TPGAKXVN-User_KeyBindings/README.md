<h2>Description</h2><div class="info"><b>Note</b>: This package requires users to be logged into the Webstrates server using for example GitHub.</p><p>This package allows to define user specific keybindings. It is possible to bind new keybindings and unbind existing bindings. The bindings are stored within the Webstrates Anywhere Cookies (<a href="https://webstrates.github.io/userguide/api/cookies.html" target="_blank">more information</a>). There it is <b>required </b>to be logged in using for example GitHub.</p><h3>Editing User Keybindings</h3><p>In order to modify user keybindings, one has to create a data paragraph and content in the structure as seen in the example. When finished the keybindings can be saved into the Webstrates cookie using the "Save from Paragraph" menu entry. The "Load into Paragraph" in return loads existing user keybindings from the Webstrates cookie into a data paragraph.</p><p>After saving keybindings the codestrate needs to be reloaded in order to apply them.</p><h3>Examples</h3><p>The following code shows an example of user keybindings in a data paragraph:</p><pre><code>{
  "bind": [
    {
      "id": "codestrates.toggleMenu",
      "key": "mod+m",
      "preventDefault": true
    }
  ],
  "unbind": [
    {
      "id": "codestrates.fullscreen",
      "key": "ctrl+shift+f"
    }
  ]
}</code></pre>
<p>The above code performs the following changes:</p>
<ul>
	<li>It binds <kbd>mod</kbd>+<kbd>m</kbd> to toggle the menu.</li>
	<li>It unbinds <kbd>ctrl</kbd>+<kbd>shift</kbd>+<kbd>f</kbd> to no longer toggle fullscreen.</li>
</ul>

# Properties

| Property | Value |
| :--- | :--- |
| Name | User KeyBindings |
| ID | TPGAKXVN |
| Version | 1.0.2 |
| Description | Utility to overwrite keybindings with user defined bindings. |
| Tags | `devtools` |
| Assets | - |
| Dependencies | - |
| Changelog | `{"1.0":"Initial version.","1.0.1":"Added check if codestrate has already loaded to trigger initialize user key bindings, which is important if the package is installed after the window.addEventListener(\"codestrateloaded\", () =&gt; {}) event was triggered.","1.0.2":"Using the new codestrate event loaded to initialize user key binding functionality."}` |