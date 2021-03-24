# st - simple terminal

st is a simple terminal emulator for X which sucks less.

![Demo](./demo.gif)


## Patches

- onedark theme
- [anysize](https://st.suckless.org/patches/anysize/) - resize to any pixel size, makes the inner border size dynamic
- [appsync](https://st.suckless.org/patches/sync/) - better draw timing to reduce flicker/tearing and improve animation smoothness
- [boxdraw](https://st.suckless.org/patches/boxdraw/) - proper rendering of lines/blocks/braille characters for gapless alignment
- [column](https://github.com/juliusHuelsmann/st-history-vim/tree/patch_column) - when shrinking the width of the window, invisible content is kept instead of removed, such that it becomes visible when the width is increased again
- [externalpipe](https://st.suckless.org/patches/externalpipe/) - reading and writing st's screen through a pipe - extracting all visible URLs and present dmenu to select and open one
- [externalpipe-eternal](https://st.suckless.org/patches/externalpipe/) - using history from scrollback for externalpipe
- [newterm](https://st.suckless.org/patches/newterm/) - new terminal in current directory
- [scrollback](https://st.suckless.org/patches/scrollback/) - scroll back through terminal output using Shift+{PageUp, PageDown}
- [scrollback-mouse](https://st.suckless.org/patches/scrollback/) - scrolling using MouseWheel
- [scrollback-mouse-altscreen](https://st.suckless.org/patches/scrollback/) -  allow scrollback only when not in MODE_ALTSCREEN
- [spoiler](https://st.suckless.org/patches/spoiler/) - use inverted defaultbg/fg for selection when bg/fg are the same
- [vertcenter](https://st.suckless.org/patches/vertcenter/) - vertically center lines in the space available if you have set a larger chscale in config.h


## Requirements

In order to build st you need the Xlib header files.

```bash
pacman -S libxft
```


## Installation

Enter the following command to build and install st (if
necessary as root):

```bash
make clean install
```

## Running st

If you did not install st with make clean install, you must compile
the st terminfo entry with the following command:

```bash
tic -sx st.info
```

See the man page for additional details.


## Credits

- [suckless](https://st.suckless.org/)
- Based on Aurélien APTEL <aurelien dot aptel at gmail dot com> bt source code.
