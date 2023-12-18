# Debian Package Exercise

This repository contains the modifications made for the Canonical assignment.

## Changes

1. `testing.sh`: A script to echo a string on the standard error (STDERR).

2. `debian/postinst`: A script to echo a string during the Debian package installation time.

3. `debian/rules`: The `rules` file in the `debian` directory was updated to install the `testing.sh` script.

## Usage

### Build and Install from Source

To use these scripts and changes, follow the steps below:

Build the .deb file from the modified source code:
```bash
debuild
```

Then, install and test .deb package:
```bash
dpkg -i <package>.deb
```

### Install from PPA

As another option, the PPA for this package is available at [Launchpad 
link](https://launchpad.net/~wennyilin/+archive/ubuntu/deb-pack-exercise).

The package can be installed from the PPA as follows:
```bash
sudo add-apt-repository ppa:wennyilin/deb-pack-exercise
sudo apt-get update
sudo apt-get install hello
```

