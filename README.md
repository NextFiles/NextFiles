# Next Files

Next Files is a fork of the elementary OS Files app

![Files Screenshot](data/screenshot-grid.png?raw=true)

## Branches

The project uses the following branches:

 - The `main` branch. This is our default branch and is the base branch for PRs and code commits.
 - The `vendor` branch is kept up-to-date with the elementary OS Files app `master` branch.

We will create other branches as we go for PRs and feature requests.

Contributions are very welcome!

## Building, Testing, and Installation

You will need the following dependencies:
* meson
* valac
* libcanberra-dev
* libcloudproviders-dev >= 0.3.0
* libdbus-glib-1-dev
* libgail-3-dev
* libgee-0.8-dev
* libgit2-glib-1.0-dev
* libglib2.0-dev
* libgranite-dev >= 6.1.0
* libgtk-3-dev
* libhandy-1-dev >= 0.83.0
* libnotify-dev
* libpango1.0-dev
* libplank-dev
* libsqlite3-dev
* libunity-dev
* libzeitgeist-2.0-dev

Run `meson build` to configure the build environment. Change to the build directory and run `ninja` to build

```bash
meson build --prefix=/usr
cd build
ninja
```

To install, use `ninja install`, then execute with `io.elementary.files`

```bash
sudo ninja install
io.elementary.files
```
