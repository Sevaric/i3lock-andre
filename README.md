i3lock-andre
============

This is an i3lock bash script that takes a screenshot of the desktop, posterizes it and adds the "We'll be right back" text.

Dependencies
------------
* [i3lock-color-git](https://github.com/chrjguill/i3lock-color) - this is a fork of i3lock-color that is kept up to date with i3lock
* imagemagick
* bash
* util-linux

Optional Dependencies
---------------------
* wmctrl
* a screenshot utility such as scrot or maim.

Installation
------------
git clone the repository and copy lock and overlay.png to "/usr/local/bin"

Usage
-----

    lock [options]

    Options:
        -h, --help       This help menu.

        -d, --desktop    Attempt to minimize all windows before locking. Requires wmctrl.

        -n, --nofork     Do not fork i3lock after starting.

        --               Must be last option. Set command to use for taking a
                         screenshot. Default is 'import -window root'. Using 'scrot'
                         or 'maim' will increase script speed and allow setting
                         custom flags like haing a delay.

example: ```lock -d -- scrot -z```

