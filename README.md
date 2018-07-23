MikeSuru Icons & Cursors
====================

This project is an extension of the [	Suru icon set](https://github.com/snwh/suru-icon-theme) to add/overwrite some icons and it will inherit all the other ones. At the moment the cursors are the same as the ones in the Suru icon set

## Copying or Reusing

This project has mixed licencing. You are free to copy, redistribute and/or modify aspects of this work under the terms of each licence accordingly (unless otherwise specified).

The Suru icon assets (any and all source `.svg` files or rendered `.png` files) are licenced under the terms of the [Creative Commons Attribution-ShareAlike 4.0 License](https://creativecommons.org/licenses/by-sa/4.0/).

Included scripts are free software licenced under the terms of the [GNU General Public License, version 3](https://www.gnu.org/licenses/gpl-3.0.txt).

## Installing & Using

You can build and install Suru from source using Meson.

```bash
# build
meson "build" --prefix=$HOME/.local
# install
sudo ninja -C "build" install
```

By default it installs to `/usr/` but you can specify a different directory with a prefix like: `/usr/local` or `$HOME/.local`.

After which you should be able to pick MikeSuru as your icon or cursor theme in GNOME Tweak tool, or you can set either from a terminal with:

```bash
# set the icon theme
gsettings set org.gnome.desktop.interface icon-theme "MikeSuru"
# or the cursor theme
gsettings set org.gnome.desktop.interface cursor-theme "MikeSuru"
```

### Uninstalling Suru

To uninstall MikeSuru, simply run the following. (If you installed it without superuser priveleges just omit the  `sudo`.)

```bash
sudo ninja -C "build" uninstall
```

Once uninstalled you can reset your icon and cursor theme to the default setting by running the following.

```bash
# reset icon theme to default
gsettings reset org.gnome.desktop.interface icon-theme
# reset cursor theme to default
gsettings reset org.gnome.desktop.interface cursor-theme
```

## Contributing

If you would like to support the [Suru](https://github.com/snwh/suru-icon-theme) development by making a donation you can do so [here](https://snwh.org/donate).
