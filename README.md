# Deimonn's Void Templates

This repository holds all of my Void Linux package templates. Some of these have yet to be merged into the official repositories, others are still work-in-progress, and others are simply not fit to be official for some reason or another.

I still make all of them available here for my (and perhaps your) convenience.

## Usage

### Setting up the repository

1.  Install prerequisites:

    ```Shell
    sudo xbps-install git xtools
    ```

2.  Clone the repository:

    ```Shell
    git clone https://github.com/deimonn/void-templates
    ```

3.  Move into the `void-templates` directory and bootstrap the `masterdir`:

    ```Shell
    cd void-templates
    ./xbps-src binary-bootstrap
    ```

### Installing packages

1.  Within the repository root, build the desired package with:

    ```Shell
    ./xbps-src pkg <package-name>
    ```

2.  If the build succeeded, you can then install the package with:

    ```Shell
    xi <package-name>
    ```

    If it didn't, please do [open an issue](https://github.com/deimonn/void-templates/issues).

## Packages

### For merge

These packages are meant to be included into the official void repositories if accepted.

#### [clapper](https://github.com/Rafostar/clapper) 0.6.0

*Status*: PR open, not merged yet.

Includes *clapper-devel* as a subpackage.

#### [keymapper](https://github.com/houmain/keymapper) 4.4.0

*Status*: PR open for 3.5.2, not merged yet.

The version in this repository is 4.4.0, which comprises various changes, the addition of a tray icon, and the `keymapperctl` program.
