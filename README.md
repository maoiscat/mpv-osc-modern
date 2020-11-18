# mpv-osc-morden
Yet another mpv osc script, based on mpv built-in osc

![img](https://github.com/maoiscat/mpv-osc-morden/blob/main/preview.png)

# How to install

put the .lua file into "\~\~/scripts/" folder, and remove other osc scripts.

mpv.conf

```
osc=no
```

It needs [Material-Design-Iconic-Font](https://zavoloklom.github.io/material-design-iconic-font/) to work. just put the ttf in "\~\~/fonts" folder.

besides i suggest a white backgound when idling

```
[idle]
profile-cond=p["idle-active"]
profile-restore=copy-equal
background=1
```
# How to config

edit osc.conf in "\~\~/script-opts/" folder, however many options are changed, so refer to the user_opts variable in the script file for details.

# Buttons

like the built-in script, some buttons may accept multiple mouse actions, here is a list:

## seekbar
* mbtn_left: seek to chosen position.
* mbtn_right: seek to the head of chosen chapter
## skip_back/forward
* mbtn_left: skip 5 seconds.
* mbtn_right: skip 60 seconds.
## playlist_back/forwad
* mbtn_left: play previous/netx file.
* mbtn_right: show playlist.
## cycle_audio/subtitle
* mbtn_left/right: cycle to next/previous track.
* mbtn_mid: show track list.
