# Changelog
|#|ACTION|CONTENT|
|---|---|---|
|1.|**remove**|user_opts.seekbarhandesize, since it causes side effects.|
|2.|**add**|user_opts.processvolume. the processed volume is to keep the loudness transition fluent, since the internal control gives the loudness dropping to fast when volume is high|
|3.|**add**|state.sys_volume.|
|4.|**add**|state.proc_volume.|
|5.|**add**|function set_volume(val)|
|6.|**change**|inhibit slider.seekRange when nil|
|7.|**change**|time slider show chapter name in tooltip|
|8.|**change**|volume slider show volume in tooltip|
|9.|**add**|when mouse over volume slider, wheel up/down change volume|
|10.|**add**|mp.observer_property('volume', 'number')|
