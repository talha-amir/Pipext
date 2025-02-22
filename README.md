# pipext

`pipext` is a utility to enhance Python's package installer `pip`. With `pipext`, when you install or uninstall a package, it automatically manages your `requirements.txt` file by appending, commenting out, or uncommenting package entries as needed.

## Features

- **Automatic Requirements Management**: On package installation, `pipext` appends the installed package (with version) to `requirements.txt` or uncomments it if it's already there.
  
- **Commenting on Uninstall**: On package uninstallation, instead of removing the package from `requirements.txt`, `pipext` comments it out, making it easy to keep track of previously used packages.

## Installation

To install pipext, run:

```bash
pip install pipext
```
This will download and install the pipext utility from PyPI, allowing you to use it directly from your terminal or command prompt.

## Usage

### Install a Package

```bash
pipext install package_name
```

This will:
1. Install the package using `pip`.
2. Add the package with its specific version to `requirements.txt` or uncomment it if it's already present (but commented out).

### Uninstall a Package

```bash
pipext uninstall package_name
```

This will:
1. Uninstall the package using `pip`.
2. Comment out the package in `requirements.txt`.

## Why pipext?

Managing a `requirements.txt` can be tedious. You install and uninstall packages during development, and sometimes it's easy to forget to update `requirements.txt` accordingly. `pipext` eases this process by automatically managing your requirements file as you modify your environment.

## Contributing

Any kind of contribution is appreciatable! Please open an issue or submit a pull request on my [GitHub repository](https://github.com/usmanmukhtar/Pipext).
