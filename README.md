[![npm (scoped)](https://img.shields.io/npm/v/@gnu-mcu-eclipse/openocd.svg)](https://www.npmjs.com/package/@gnu-mcu-eclipse/openocd) 
[![license](https://img.shields.io/github/license/gnu-mcu-eclipse/openocd-xpack.svg)](https://github.com/gnu-mcu-eclipse/openocd-xpack/blob/xpack/LICENSE) [![npm](https://img.shields.io/npm/dt/@gnu-mcu-eclipse/openocd.svg)](https://www.npmjs.com/package/@gnu-mcu-eclipse/openocd/)


## GNU MCU Eclipse OpenOCD binaries

This xPack installs the platform specific binaries for OpenOCD.

This project is open source and it is publicly available from [GitHub](https://github.com/gnu-mcu-eclipse/openocd-xpack).

## How to use

This section is intended for developers who plan to use the OpenOCD binaries.

### Prerequisites

A recent [`xpm`](https://www.npmjs.com/package/xpm), which is a 
portable [Node.js](https://nodejs.org/) command line application.

### Easy install

The package is available as [`@gnu-mcu-eclipse/openocd`](https://www.npmjs.com/package/gnu-mcu-eclipse/openocd) from the `npmjs.com` registry; with `xpm` available, installing the latest version of the package is quite easy:

```console
$ xpm install @gnu-mcu-eclipse/openocd --global
```

Global `xpm` packages are installed in the user home folder, and do not require `sudo`.

To remove the installed xPack, the command is similar:

```console
$ xpm uninstall @gnu-mcu-eclipse/openocd --global
```

(Note: not yet implemented)

## Developer info

### xPack git repo

The few xPack source files are available from GitHub:

```console
$ git clone https://github.com/gnu-mcu-eclipse/openocd-xpack.git openocd-xpack.git
```

### OpenOCD binaries

The binaries are downloaded from the [gnu-mcu-eclipse/openocd.git](https://github.com/gnu-mcu-eclipse/openocd) project, the [releases](https://github.com/gnu-mcu-eclipse/openocd/releases) page.

## Maintainer info

### How to publish

* open [releases](https://github.com/gnu-mcu-eclipse/openocd/releases) and select the latest release
* update the `baseUrl:` with the file URLs (including the tag/version)
* from the blog post, copy the SHA & file names
* commit all changes, use a message like `0.10.0-5.1` (without `v`)
* `npm version 0.10.0-5.1`
* push all changes to GitHub
* `npm publish`

## License

The original content is released under the [MIT License](https://opensource.org/licenses/MIT), with all rights reserved to [Liviu Ionescu](https://github.com/ilg-ul).

The binary distributions include several open-source components; the
corresponding licenses are available in the `gnu-mcu-eclipse/licenses`
folder.
