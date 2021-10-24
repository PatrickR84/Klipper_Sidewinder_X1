# Klipper_Sidewinder_X1
This is my current Klipper config for the Artillery Sidewinder X1 with a BL Touch.

PID autotune bed heater:
There are some issues with Klippers PID autotune with the bed heater. The values that are currently active allow a stable temperature with little delay. The autotune values for the heater make it heat approx. 8 degrees celcius above target and fluctuate more than 3 degrees leading to Z-banding on the print.


START_PRINT:
Currently set up to print a single purge line and MESH_LEVEL the bed before each print.
There are still issues with some filament oozing out during travel, after the purge line.
Don't forget to set up your custom start and end GCode in your slicer to send the START_PTINT and END_PRINT.
START_PRINT needs the parameters for EXTRUDER_TEMP and BED_TEMP

PAUSE_PRINT and RESUME_PRINT:
I have not yet tested these as I still need to hook up the filament sensor to the mainboard. I found these code snippets on some forums.


This config has not been tuned for linear advance or input shaping.

Use at your own risk and feel free to use, modify and share.
