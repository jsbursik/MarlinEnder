# Marlin 2.0.x for Ender 3

This is my Marlin firmware for my Ender 3 with a BLtouch added using [this mount.](https://www.thingiverse.com/thing:3584158)

The board I'm using is the BIGTREETECH SKR Mini E3 V1.2 using the BLtouch as the Z endstop.

Some of these settings WILL NOT work for you. Specifically the Z offset and the VREF's set in Configuration_adv.h for the TMC2209's.

# Bed Size

## Y-Axis
I zeroed the Y axis and noticed the hotend sticks over the edge, so to zero the Y axis I moved it forward until it cleared the binder clips (Y = 15) then moved it until it got to the second set of binder clips, with subtraction you get 210 from clip to clip (give or take)

## X-axis
I then zeroed the X-axis and moved it to the middle of the bed - using the posts underneath the bed to get it as close as possible and measured 115mm from zero which means 230 across.

# Linear Advance
I used the calibration pattern to figure out what my linear advance value should be, without refining it, I decided to just use 1.2 This could use more tweaking. **This will be different for every machine, so set it to zero and use the test patterns on the marlin website to figure this out**
