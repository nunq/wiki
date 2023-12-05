# neovim

probably applies to vim as well but idk.

improve the usability of a default no config (n)vim instantly with this oneliner: 
```vim
:set number | :colorscheme desert | :set mouse=a
```

* enables line numbering
* sets an ok (default!) colorscheme
* enables the mouse, scrolling and other things

## windows
* `ctrl s` spawn window with same file
* `ctrl q` close window
* `ctrl v` split vertical (same as s, but vertical)

## copy stuff
* copy word under cursor: `yaw`

## other cmds
* r replace
* O new line above
* o new line below
* I insert at beginning
* A append
* d delete
* x del char
* diX delete inner X
* V select line
* n next match
* N previous match
* J join lines
* 0 cursor to start
* $ cursor to end
* dw delete word
* d$ del till end of line
* U undo all for current line
* P paste in line above

## etc

#### nautilus or thunar: open file in neovim with double click
symlink `xterm` to your terminal emulator, i.e. for kitty `sudo ln -sf /usr/bin/kitty /usr/local/bin/xterm`, because somehow somewhere xterm is the hardcoded default.


#### open urls
because neovim uses netrw it can open urls: `nvim "http://example.com/"` (wgets the html to /tmp and opens it)
