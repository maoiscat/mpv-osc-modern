# mpv-osc-metro
Yet another mpv osc script based on the original osc of mpv.

metro.lua     -- osc script

metro-chs.lua -- the same script with texts in chinese

# How to use

copy either one of the .lua file into "~~/scripts/" folder, and remove other osc scripts.

mpv.conf

```
osc=no
```

besides i suggest a white backgound when idling

```
[idle]
profile-cond=p["idle-active"]
profile-restore=copy-equal
background=1
```

osc.conf

```
font=Segoe UI
```

It needs [Material-Design-Iconic-Font](https://zavoloklom.github.io/material-design-iconic-font/) to work.

![img](https://github.com/maoiscat/mpv-osc-metro/blob/main/preview.png)
