# [GitHub Desktop](https://desktop.github.com) - The Linux Fork

[![Build Status](https://brendanforster.visualstudio.com/desktop-linux/_apis/build/status/Azure%20Pipelines%20Build?branchName=linux)](https://brendanforster.visualstudio.com/desktop-linux/_build/latest?definitionId=10&branchName=linux)
[![license](https://img.shields.io/github/license/desktop/desktop.svg?style=flat-square)](https://github.com/desktop/desktop/blob/development/LICENSE)
![90+% TypeScript](https://img.shields.io/github/languages/top/desktop/desktop.svg?style=flat-square&colorB=green)

GitHub Desktop is an open source [Electron](https://electron.atom.io)-based
GitHub app. It is written in [TypeScript](http://www.typescriptlang.org) and
uses [React](https://facebook.github.io/react/).

![GitHub Desktop screenshot - Windows](https://cloud.githubusercontent.com/assets/359239/26094502/a1f56d02-3a5d-11e7-8799-23c7ba5e5106.png)

## What is this repository for?

This repository contains specific patches on top of the upstream
`desktop/desktop` repository to support Linux usage.

It also hosts preview packages for various Linux distributions:

 - AppImage (`.AppImage`)
 - Debian (`.deb`)
 - RPM (`.rpm`)
 - Snap (`.snap`) - also available from [snapcraft.io](https://snapcraft.io/github-desktop)

Check out the [latest releases](https://github.com/shiftkey/desktop/releases) to
help out with testing on your distribution.

### Snapcraft Store

We are currently testing out a new version of the Snap that requires using the
`classic` enclosure, as GitHub Desktop has integrations to launch your chosen
shell or editor which are not supported in the `strict` enclosure.

**If you are currently running the Snap installed from `edge`**

You will be prompted to manually upgrade to the `beta` channel as an installed
application cannot upgrade it's enclosure via an update.

To upgrade manually, run these commands:

```
$ snap remove github-desktop
$ snap install github-desktop --beta --classic
```

## Other Distributions

Arch Linux users can install GitHub Desktop from the
[AUR](https://aur.archlinux.org/packages/github-desktop-bin/).

`gnome-keyring` is required and the daemon must be launched either at login or when the X server is started. Normally this is handled by a display manager, but in other cases following the instructions found on the [Arch Wiki](https://wiki.archlinux.org/index.php/GNOME/Keyring#Using_the_keyring_outside_GNOME) will fix the issue of not being able to save login credentials.

## More information

Please check out the [README](https://github.com/desktop/desktop#github-desktop)
on the upstream [GitHub Desktop project](https://github.com/desktop/desktop) and
[desktop.github.com](https://desktop.github.com) for more product-oriented
information about GitHub Desktop.

## License

**[MIT](LICENSE)**

The MIT license grant is not for GitHub's trademarks, which include the logo
designs. GitHub reserves all trademark and copyright rights in and to all
GitHub trademarks. GitHub's logos include, for instance, the stylized
Invertocat designs that include "logo" in the file title in the following
folder: [logos](app/static/logos).

GitHub® and its stylized versions and the Invertocat mark are GitHub's
Trademarks or registered Trademarks. When using GitHub's logos, be sure to
follow the GitHub [logo guidelines](https://github.com/logos).
