# Deimonn's Void Templates

> [!WARNING]  
> This repository has been unmaintained for a while now and, as of 14th of April 2026, I'm formally deprecating it to soon turn it into a public archive.
>
> I'll be trying to push [keymapper](https://github.com/houmain/keymapper) into the official repo. The [wallpaper-engine-kde-plugin](https://github.com/catsout/wallpaper-engine-kde-plugin) template is being abandoned; build the plugin from source instead.

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

#### [keymapper](https://github.com/houmain/keymapper) 4.11.0

Provides `keymapper`, `keymapperd` and `keymapperctl`.

See [this page](https://deimonn.dev/view?r=void-guides&f=3.%20Extra%20Software/Key%20remapping%20with%20keymapper.md) for information on how to use keymapper on Void Linux.

#### [wallpaper-engine-kde-plugin](https://github.com/catsout/wallpaper-engine-kde-plugin) 0.5.4+20231104

Provides the "Wallpaper Engine for Kde" KDE wallpaper plugin.

See [this page](https://deimonn.dev/view?r=void-guides&t=master&f=3.%2520Extra%2520Software/Getting%2520animated%2520wallpapers.md) for instructions on how to use this package.
