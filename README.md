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

### .NET

Void Linux does not ship `dotnet` yet, and although Microsoft's install script works, it misses all of the advantages of installing it via package manager.

Thus here I provide templates to install `dotnet` via XBPS, as well as templates for some packages depending on it.

All of these download and install through binary blobs.

#### dotnet 8.0.301

Ships the latest .NET SDK and runtime.

#### dotnet7 7.0.410

Ships the .NET 7.0 SDK and runtime.

#### dotnet6 6.0.423

Ships the .NET 6.0 SDK and runtime.

#### dotnet5 5.0.408

Ships the .NET 5.0 SDK and runtime.

#### [OpenTabletDriver](https://github.com/OpenTabletDriver/OpenTabletDriver) 0.6.4.0

See [this page](https://github.com/deimonn/void-guides/blob/master/3.%20Extra%20Software/Installing%20OpenTabletDriver.md) for information on how to use this.
