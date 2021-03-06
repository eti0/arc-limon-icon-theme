# Arc Limon Icon Theme

**Note:** This is still unfinished. It may not work as expected in some cases.

At the moment this theme mainly includes icons for folders and mimetypes.

### Requirements

This theme doesn't provide application icons, it needs another icon theme to inherit them.
By default this theme will look for the [Moka icon theme](https://snwh.org/moka) to get the missing icons. If Moka is not installed it will use the Gnome icon theme as fallback.
To change the application icons, edit `ArcLimon/index.theme` and replace `Moka` with the name of your preferred icon theme

For example, if you like the Faenza icon theme, change

    [Icon Theme]
    Name=Arc
    Inherits=Moka,Adwaita,gnome,hicolor
    Comment=Arc Limon Icon theme

to

    [Icon Theme]
    Name=Arc
    Inherits=Faenza,Adwaita,gnome,hicolor
    Comment=Arc Limon Icon theme

### Installation

Installation via autotools:

    git clone https://github.com/eti0/arc-limon-icon-theme --depth 1 && cd arc-limon-icon-theme
    ./autogen.sh --prefix=/usr
    sudo make install

Alternatively you may copy the `ArcLimon` folder to `~/.icons` or to `/usr/share/icons` for system-wide use.

### Uninstall

Run

    sudo make uninstall

from the same directory as this README resides in, or

    sudo rm -rf /usr/share/icons/ArcLimon


License: GPLv3
