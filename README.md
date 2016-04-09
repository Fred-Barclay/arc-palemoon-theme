# Arc Pale Moon Theme.

Unoffical [Arc](https://github.com/horst3180/Arc-theme) Pale Moon theme.
WORK IN PROGRESS. NOT WORKING WELL AT THE MOMENT!!!! USE AT YOUR OWN RISK.

**Note**: This theme is meant to be used in conjunction with the [Arc GTK theme](https://github.com/horst3180/Arc-theme), don't use it with other GTK themes or it will look broken.

#### Manual building and installation

These instructions are for testers and package maintainers. They also allow to install the theme globally for all users.

You will need `autoconf` and `automake` for the following.

Clone the repository

    git clone https://github.com/horst3180/arc-firefox-theme && cd arc-firefox-theme

Generate the .xpi files (drag and drop these into your Firefox window)

    ./autogen.sh --prefix=/usr
    make mkxpi

Alternatively the theme can be installed globally without using the .xpi files

    ./autogen.sh --prefix=/usr
    sudo make install

Other build options to append to `autogen.sh` are

    --disable-light         disable Arc Light Firefox support
    --disable-darker        disable Arc Darker Firefox support
    --disable-dark          disable Arc Dark Firefox support

Uninstall the theme with

    sudo make uninstall
