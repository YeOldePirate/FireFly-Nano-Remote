# Nano version of FireFly-Remote

Control your electric skateboard with an Arduino controlled remote. This repository contains the needed software for the remote and the receiver. You can find the 3D-models for the remote (STL files) on Thingiverse: https://www.thingiverse.com/thing:3303495 and read more about the project on: https://www.electric-skateboard.builders/t/simple-3d-printed-nrf-remote-arduino-controlled/28543

I have made a Wiki here on Github, with a few tips and guides on how to build the remote. The Wiki can be found here: https://github.com/DroidSector/FireFly-Nano-Remote/wiki

**Important**: This remote is still in development, and is far from perfect. Stay safe, and remember to wear protective gear!

This branch contains fixes for the heltec v2.1 board that silently ships as v2.0

Notes: 

-dont forget to set the frequency in radio.h (868 for yurop, 915 for US), wifi credentials in wifi_credentials.h and the rest of the stuff in global.h

-the hall sensor min max and center points have to be defined before compiling, since the built in calibration is broken

-the flash needs to be wiped before flashing for the settings to take effect

-if the screen is blank after flashing the remote but the white led is on it means that the battery probe is either reporting a wrong value or DISPLAY_BATTERY_MIN in globals.h is set too high

-button on top is power/back, trigger acts as select and throttle is for going up/down in the menus


good luck with your build.
