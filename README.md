# mpv-osc-morden x
Yet another mpv osc script, based on [mpv-osc-morden](https://github.com/maoiscat/mpv-osc-morden/), which is in turn mpv built-in osc.
Mostly minor changes including repurposing the skip_back/forward buttons to go to the previous/next chapter and fixing the play/pause button.

![img](https://github.com/cyl0/mpv-osc-morden-x/blob/main/preview.png)

# How to install

put the .lua file into "\~\~/scripts/" folder, and remove other osc scripts.

mpv.conf

```
osc = no
border = no # Optional, but recommended
```

It needs [Material-Design-Iconic-Font](https://zavoloklom.github.io/material-design-iconic-font/) to work. just put the ttf in "\~\~/fonts" folder.

# How to config

edit osc.conf in "\~\~/script-opts/" folder, however many options are changed, so refer to the user_opts variable in the script file for details.

# Buttons

like the built-in script, some buttons may accept multiple mouse actions, here is a list:

## seekbar
* mbtn_left: seek to chosen position.
* mbtn_right: seek to the head of chosen chapter
## skip_back/forward
* mbtn_left: go to previous/next chapter.
## playlist_back/forwad
* mbtn_left: play previous/netx file.
* mbtn_right: show playlist.
## cycle_audio/subtitle
* mbtn_left/right: cycle to next/previous track.
* mbtn_mid: show track list.
