# mpv-osc-modern

updated 2022.7.8

I have to say sorry that I misspelled the word "modern" to "morden". Now it is corrected.

This osc is updated to provide a mute button and a simple volume slider, yet they can be disabled through the conf file.

This modern.lua file is coded with [Lua](https://www.lua.org/), anyone can learn to develop his demanding feature.

---

Yet another mpv osc script, based on mpv built-in osc

![img](https://github.com/maoiscat/mpv-osc-modern/blob/main/preview.png)

# Installation

modern.lua --> "\~\~/scripts/" (!!REMOVE OTHER OSC SCRIPTS!!)

material-design-iconic-font.ttf --> "\~\~/fonts" ([FONT LINK](https://zavoloklom.github.io/material-design-iconic-font/))

Then edit "\~\~/mpv.conf", add the following lines to the end

```
osc=no

[idle]
profile-cond=p["idle-active"]
profile-restore=copy-equal
background=1
```
# Configuration

Config file locates at "\~\~/script-opts/osc.conf". Supported options are listed below.

```
    showwindowed = true,        -- show OSC when windowed?
    showfullscreen = true,      -- show OSC when fullscreen?
    scalewindowed = 1,          -- scaling of the controller when windowed
    scalefullscreen = 1,        -- scaling of the controller when fullscreen
    scaleforcedwindow = 2,      -- scaling when rendered on a forced window
    vidscale = false,           -- scale the controller with the video?
    hidetimeout = 1000,         -- duration in ms until the OSC hides if no mouse movement. enforced non-negative for the user, but internally negative is 'always-on'.
    fadeduration = 500,         -- duration of fade out in ms, 0 = no fade
    minmousemove = 3,           -- minimum amount of pixels the mouse has to move between ticks to make the OSC show up
    iamaprogrammer = false,     -- use native mpv values and disable OSC internal track list management (and some functions that depend on it)
    font = 'mpv-osd-symbols',   -- default osc font
    seekbarhandlesize = 1.0,    -- size ratio of the slider handle, range 0 ~ 1
    seekrange = true,           -- show seekrange overlay
    seekrangealpha = 128,       -- transparency of seekranges
    seekbarkeyframes = true,    -- use keyframes when dragging the seekbar
    title = '${media-title}',   -- string compatible with property-expansion to be shown as OSC title
    showtitle = true,           -- show title and no hide timeout on pause
    timetotal = true,           -- display total time instead of remaining time?
    visibility = 'auto',        -- only used at init to set visibility_mode(...)
    windowcontrols = 'auto',    -- whether to show window controls
    volumecontrol = true,       -- whether to show mute button and volumne slider
    language = 'eng',           -- eng=English, chs=Chinese
```

# Button Actions

Some buttons may accept multiple mouse actions, here is a list:

(NOTE: mbtn = mouse button)

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
