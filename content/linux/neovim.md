# neovim

probably applies to vim as well but idk.

## windows
* `ctrl s` spawn window with same file
* `ctrl q` close window
* `ctrl v` split vertical (same as s, but vertical)

## copy stuff
* copy word under cursor: `yaw`


## etc
nautilus: open file in neovim with double click.

change `Terminal=true` to `Terminal=false` and change the `Exec` directive to append your `$terminal_emulator-executable` before `nvim %F`.
this is because nautilus sees `Terminal=true` and tries to spawn nvim in xterm. i dont know why this seems to be hardcoded?
alternatively you can symlink xterm to your terminal emulator, i.e. for kitty `sudo ln -sf /usr/bin/kitty /usr/local/bin/xterm`

