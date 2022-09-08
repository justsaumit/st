# st
Attempt to make suckless tool [st (simple terminal)]((https://st.suckless.org/)) more featureful and allowing scripting.

## Added Features
+ Compatibility with `Xresources` and `pywal` for dynamic colors.
+ Ability to add a Primary font and then extra fonts in font2 for ligature/icons/color emoji support
+ Scroll with custom keybindings
+ Ligature support
+ Scripting using externalpipe

## dmenu scripiting using externalpipe
+ **Follow urls** by pressing &emsp;&emsp;&emsp;&emsp;&emsp;&ensp; `alt-o`
&emsp;&nbsp;//o for openurl
+ **Copy urls** in the same way with &emsp;&emsp;&nbsp;`alt-l`
&emsp;&nbsp;//linkcopy
+ **Copy the output of commands** with `alt-k`
&emsp;//kopyoutput

## Bindings for

+ **Scrollback** with `alt-↑/↓` or `alt-pageup/down` or `alt` while scrolling the
  mouse.
+ **Zoom/Change font size**: Achieved by long pressing 'Ctrl+Shift' and then pressing 'PageUp/PageDown' or 'vim-keys)(k/j)' to increase/decrease font size.  
Ctrl+Shift in succession with 'Home' key or 'u' sets font to default size
+ **copy text** with `alt-c`, **paste** is `alt-v` or `shift-insert`

## Added Patches (in order)
+ [xresources](https://st.suckless.org/patches/xresources/)
+ [anysize](https://st.suckless.org/patches/anysize/)
+ [bold-is-not-bright](https://st.suckless.org/patches/bold-is-not-bright/)
+ [font2](https://st.suckless.org/patches/font2/)
+ [scrollback](https://st.suckless.org/patches/scrollback/)
+ [scrollback-mouse](https://st.suckless.org/patches/scrollback/)
+ [boxdraw](https://st.suckless.org/patches/boxdraw/)
+ [vertcenter](https://st.suckless.org/patches/vertcenter/)
+ [st-dynamic-cursor-color](https://st.suckless.org/patches/dynamic-cursor-color/)
+ [patch to fix wide wide glyphs truncation](https://0x0.st/oeSQ.diff)
+ [st-ligatures-boxdraw-0.8.4](https://st.suckless.org/patches/ligatures/0.8.4/st-ligatures-boxdraw-20210824-0.8.4.diff)
+ [st-externalpipe](https://st.suckless.org/patches/externalpipe/)

## Dependencies

    Xlib, harfbuzz, xrdb

## Install

    make clean install
