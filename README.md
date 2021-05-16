# mpv-osc-morden x
An MPV OSC script, based on [mpv-osc-morden](https://github.com/maoiscat/mpv-osc-morden/), with some minor changes including making the skip_back/forward buttons go to the previous/next chapter like in MPV's default OSC and fixing the play/pause button.

![img](https://github.com/cyl0/mpv-osc-morden-x/blob/main/preview.png)

# How to install

Locate your MPV folder. It is typically located at `%APPDATA%\mpv\scripts\mpv_thumbnail_script_server.lua` on Windows and `~/.config/mpv/scripts/mpv_thumbnail_script_server.lua` on Linux/MacOS. See the [Files section](https://mpv.io/manual/master/#files) in mpv's manual for more info.

Put mordenx.lua into your mpv "\~\~/scripts/" folder, and remove other osc scripts,
then put the `Material-Design-Iconic-Font.ttf` from [Material-Design-Iconic-Font](https://zavoloklom.github.io/material-design-iconic-font/) in the "\~\~/fonts" folder.

in mpv.conf:

```
osc = no
border = no # Optional, but recommended
```


# How to config

edit osc.conf in "\~\~/script-opts/" folder, however many options are changed, so refer to the user_opts variable in the script file for details.

# Buttons

like the built-in script, some buttons may accept multiple mouse actions, here is a list:

## seekbar
* mbtn_left: seek to chosen position.
* mbtn_right: seek to the head of chosen chapter
## skip_back/forward
* mbtn_left: go to previous/next chapter.
* mbtn_right: show chapter list.
## playlist_back/forwad
* mbtn_left: play previous/next file.
* mbtn_right: show playlist.
## cycle_audio/subtitle
* mbtn_left/right: cycle to next/previous track.
* mbtn_mid: show track list.
