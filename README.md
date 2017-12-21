# Codestrate-Packages

Codestrate-Packages is an extension to [Codestrates](https://github.com/Webstrates/Codestrates). It provides additonal features to Codestrates, which can be easily added to or removed from a codestrate.

## Installation

To use Codestrate-Packages you need to setup a [codestrate](http://codestrates.org) first. Refer to the [Codestrates GitHub repository](https://github.com/Webstrates/Codestrates) for instructions on how to set one up. To import the packages into an existing codestrate you need to download the [zip-file](https://github.com/Webstrates/Codestrate-Packages/archive/master.zip) of this repository and import it into the codestrate using the _Package Management &rightarrow; Import Packages_ entry in the menu in Codestrates.

## Usage

The idea behind Codestrate-Packages is to have a `Codestrate` prototype, which offers the basic functionality of Codestrates, and additionally a separate codestrate named `Codestrate-Packages`, which acts as a repository of packages on the Webstrates server and from where packages are usually installed from.

### Installing and Updating Packages

Selecting the _Install and Update Packages_ entry in the menu will open a dialog, where one can select packages to install or update. At the top of the dialog one can select a codestrate and a codestrate version or tag, from which he wants to install packages from.

### Pushing Packages

When developing new packages or modifying existing packages, the packages can be pushed to another codestrate (e.g. the _Codestrate-Packages_ codestrate). This is done by using the _Push Packages_ entry in the menu.

### Removing Packages

Removing packages is done by selecting the _Remove Packages_ entry in the menu. It will open a dialog, where one can select the packages, that should be removed from a codestrate.

**Hint**: Packages section should not just be deleted but removed using the dialog.

## Development

For more detailed information on how packages exactly work and how they are structured, refer to the documentation of the _Package Management_ system section in a codestrate.

## Disclaimer

Codestrates is a research prototype in active development. Many features are still experimental and yet to be properly documented.

---

<p align="center">&copy;&nbsp;2017&nbsp;Aarhus&nbsp;University</p>
