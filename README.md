# OpenArena utility programs/scripts

Small scripts that can be useful to do stuff related to OpenArena.

## FOV Sensitivity Calculator - `fovsenscalc`

A script to calculate how much sensitivity and mouse acceleration should change
when `cg_fov` is changed for the mouse to keep the exact same feeling. It should
take the same movement to change look direction to a specific point on the
screen independent on FOV.

The correct formula for this is `tan(newfov / 2) / tan(oldfov / 2)` and it is
what the script uses.

## Hor+ FOV calculator - `hor+fovcalc`

Newer versions of OpenArena engine will use *Hor+* FOV for `cg_fov` so this
script should only be used if playing with older engine. The latest engine-code
for OpenArena can be downloaded here: https://github.com/OpenArena/engine/ (note
that you have to compile it yourself).

Convert from *Hor+* FOV to *Vert-* FOV.

*Hor+* is where the vertical FOV has the same value as it would have on a 4:3
aspect ratio monitor and the horizontal FOV is changed to fit the monitors
aspect ratio.

*Vert-* is where the vertical FOV is lowered to compensate for higher horizontal
FOV. This is what older versions of the OpenArena engine code uses.

See [this page](https://en.wikipedia.org/wiki/Field_of_view_in_video_games) for
more information.
