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

Convert from *Hor+* FOV to *Vert-* FOV.

*Hor+* is where the vertical FOV has the same value as it would have on a 4:3
aspect ratio monitor and the horizontal FOV is changed to fit the monitors
aspect ratio. 

*Vert-* is where the vertical FOV is lowered to compensate for higher horizontal
FOV. This is what OpenArena currently uses (but that might be changed to Hor+ in
OA3).

See [this page](https://en.wikipedia.org/wiki/Field_of_view_in_video_games) for
more information.
