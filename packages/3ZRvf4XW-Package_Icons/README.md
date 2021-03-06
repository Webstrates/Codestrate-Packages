<h2>Description</h2>
<p>Sidebar for managing of packages and package repositories.</p><h2>Two Views</h2><p>The sidebar has two views: Packages and Repositories. In the packages view, which is the default view, one can see all packages of the selected repository as well as just locally installed packages. The user can switch between the views by pressing the indigo menu button on the top of the sidebar.</p><h2>Packages</h2><p>Packages are displayed as a list of package icons. The color of the package icons indicate the current state (see list below). When hovering over an package a tooltip shows the name of the package. Three buttons allow for basic package routines: installing/updating, removing, pushing. The icon of each package can be set in the section-properties of each package.</p><p>The "Refresh Packages List" makes it possible to update the package icons without having to reload the page (e.g. when there were updates on a repository). Local changes as adding packages or removing them is directly updated inside the package view.</p><h3>Package Colors</h3><p>The color of the icon indicate the state of the package:</p><p><ul><li><b style="color: rgb(238, 238, 238);">Lightgrey</b>: Package is available on the prototype for download.</li><li><b style="color: rgb(76, 175, 80);">Green</b>: The package is installed and up to date.</li><li><b style="color: rgb(255, 152, 0);">Orange</b>: The package is installed but has a changed version.</li><li><b style="color: rgb(0, 150, 136);">Teal</b>: The package is installed but versions couldn't be compared with repository.</li><li><b style="color: rgb(3, 169, 244);">Cyan</b>: The package is installed but not available in the repository.</li><li><b style="color: rgb(66, 66, 66);">Darkgrey</b>: Only persistent parts of the package are installed.</li></ul><h2>Repositories</h2></p><p>In the repositories view users can add, remove and select package repositories. The list of repositories is stored in a webstrate anywhere cookie. So currently one has to be logged in to add new repositories to your own list.</p><p>Like package icons the repository icons allow to select them and thus update the package view or remove repositories from the list. The default package at the moment is "mb-packages".</p>

# Properties

| Property | Value |
| :--- | :--- |
| Name | Package Icons |
| ID | 3ZRvf4XW |
| Version | 1.2.1 |
| Description | Sidebar for packages. |
| Tags | `devtools, packages` |
| Assets | - |
| Dependencies | - |
| Changelog | `{"1.2.1":"Fixed z-index to let the icons stay under the snackbar.","1.2":"Renaming from stores to repositories.","1.1":"Style fixes and global package store manager.","1.0":"Initial Release"}` |