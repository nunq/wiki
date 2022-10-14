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

change `Terminal=true` to `Terminal=false` in `/usr/share/applications/nvim.desktop` and prepend your `$terminal_emulator-executable` before `nvim %F` in the `Exec` directive.
this is because nautilus sees `Terminal=true` and tries to spawn nvim in xterm. i dont know why this seems to be hardcoded?
alternatively you should be able to symlink xterm to your terminal emulator, i.e. for kitty `sudo ln -sf /usr/bin/kitty /usr/local/bin/xterm` although this doesnt seem to work for me

