# neovim

probably applies to vim as well but idk.

improve the usability of a default no config (n)vim instantly with this oneliner: `:set number | :colorscheme desert | :set mouse=a`
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
* 
* dw delete word
* d$ del till end of line
* 
* U undo all for current line
* P paste in line above

## etc
nautilus: open file in neovim with double click.

change `Terminal=true` to `Terminal=false` in `/usr/share/applications/nvim.desktop` and prepend your `$terminal_emulator-executable` before `nvim %F` in the `Exec` directive.
this is because nautilus sees `Terminal=true` and tries to spawn nvim in xterm. i dont know why this seems to be hardcoded?
alternatively you should be able to symlink xterm to your terminal emulator, i.e. for kitty `sudo ln -sf /usr/bin/kitty /usr/local/bin/xterm` although this doesnt seem to work for me

