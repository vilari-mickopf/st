# st - simple terminal

st is a simple terminal emulator for X which sucks less.

![Demo](./demo.gif)


## Patches

- onedark theme
- [anysize](https://st.suckless.org/patches/anysize/)
- [appsync](https://st.suckless.org/patches/sync/)
- [boxdraw](https://st.suckless.org/patches/boxdraw/)
- [newterm](https://st.suckless.org/patches/newterm/)
- [scrollback](https://st.suckless.org/patches/scrollback/)
- [scrollback-mouse](https://st.suckless.org/patches/scrollback/)
- [scrollback-mouse-altscreen](https://st.suckless.org/patches/scrollback/)
- [spoiler](https://st.suckless.org/patches/spoiler/)
- [vertcenter](https://st.suckless.org/patches/vertcenter/)


## Requirements

In order to build st you need the Xlib header files.

```
pacman -S libxft
```


## Installation

Enter the following command to build and install st (if
necessary as root):

```
make clean install
```

## Running st

If you did not install st with make clean install, you must compile
the st terminfo entry with the following command:

```
tic -sx st.info
```

See the man page for additional details.


## Credits

- [suckless](https://st.suckless.org/)
- Based on Aurélien APTEL <aurelien dot aptel at gmail dot com> bt source code.
