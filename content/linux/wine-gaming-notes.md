# wine gaming notes

notes on running certain windows games using wine.

## fallout new vegas 22380
works with v7.0-1 and launch opts `DO=(%command%); "${DO[@]/%FalloutNVLauncher.exe/FalloutNV.exe}"` [src](https://www.youtube.com/watch?v=3WtAex5uljw)

mouse sensitivity suggested fix: add
```
fForegroundMouseAccelBase=0
fForegroundMouseAccelTop=0
fForegroundMouseBase=0
fForegroundMouseMult=0
```
to `.local/share/Steam/steamapps/common/Fallout\ New\ Vegas/Fallout_default.ini` under section `[Controls]` [src](https://www.protondb.com/app/22380#O0SBH92X9). but it doesnt actually seem to work?

## anno 1404 (venice) history edition 1887720
works with v6.3-8 and launch opts `PROTON_USE_D9VK=1 %command%`

set wineprefix to pfx root and run ubisoft connect installer downloaded form ubisoft dot com. [src](https://www.protondb.com/app/1281630#5-3V2InGYh)
