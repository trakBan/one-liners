# one-liners
Bash one-liners i came up with (may or may not be useful)
Most of these commands need to be modified in order for them to be added as aliases.

## MPV autoload
Autoloads files in mpv (like [autoload.lua](https://github.com/mpv-player/mpv/blob/master/TOOLS/lua/autoload.lua))
```
echo `ls` >> list.mpvlist && sed -i 's/ /\n/g' list.mpvlist && mpv --playlist=list.mpvlist & rm list.mpvlist
```
