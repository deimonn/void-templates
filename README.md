# Deimonn's Void Templates

This repository holds all of my Void Linux package templates, primarily for my own convenience - but perhaps for yours as well.

These are unofficial and not currently found in the [void-packages](https://github.com/void-linux/void-packages) repo.

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

#### [clapper](https://github.com/Rafostar/clapper) 0.6.1

Provides the Clapper desktop application as well as `clappersink`. Includes *clapper-devel* as a subpackage.

If you get errors about missing decoders, see [this page](https://deimonn.dev/view?r=void-guides&f=4.%20Notes%20%26%20Troubleshooting/Missing%20video%20decoders.md).

#### [keymapper](https://github.com/houmain/keymapper) 4.8.2

Provides `keymapper`, `keymapperd` and `keymapperctl`.

See [this page](https://deimonn.dev/view?r=void-guides&f=3.%20Extra%20Software/Key%20remapping%20with%20keymapper.md) for information on how to use keymapper on Void Linux.
