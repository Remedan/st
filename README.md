st - simple terminal
--------------------
st is a simple terminal emulator for X which sucks less.

**This is a fork of [suckless st](https://st.suckless.org/).**

Patches
-------
* [scrollback](https://st.suckless.org/patches/scrollback/)
    * st-scrollback-20170329-149c0d3.diff
    * st-scrollback-mouse-20170427-5a10aca.diff
    * st-scrollback-mouse-altscreen-20170427-5a10aca.diff
* [gruvbox](https://github.com/morhetz/gruvbox-contrib)
    * gruvbox-dark.h
* [vertcenter](https://st.suckless.org/patches/vertcenter/)
    * st-vertcenter-20171207-0ac685f.diff

Requirements
------------
In order to build st you need the Xlib header files.


Installation
------------
Edit config.mk to match your local setup (st is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install st (if
necessary as root):

    make clean install


Running st
----------
If you did not install st with make clean install, you must compile
the st terminfo entry with the following command:

    tic -sx st.info

See the man page for additional details.

Credits
-------
Based on Aurélien APTEL <aurelien dot aptel at gmail dot com> bt source code.

