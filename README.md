# Vectr

Vectr is a next-gen OSM firmware targeting the OSMv2's accelerometer to seamlessly blend motion reactivity into your shows.
  It is not configurable on chip.

# Branch Information

Vectr-ClickResistant changes the first second of every click, adding an initial 500ms buffer that will absorb all those random clicks that can distract from your style.

Play operation:
Clicking the button on the OSM chip for under 500ms will initialize the mode or put the chip to sleep if set to conjure.
Holding between 0.5 and 1 seconds - Change the mode or put the chip to sleep if set to conjure. Flashes white at 1 seconds.
Holding between 1 and 2 seconds - Turns off light on release. Flashes blue at 2 seconds.
Hold between 2 and 4 seconds - Toggles conjure mode on release. Flashes red at 4 seconds.
Hold 4 seconds or more - Locks and turns off light on release. 

# Installation

Same requirements as vectr, this will create a google chrome app called VectrUI-clickResistant with version number 0.3.5. If you start it for the first time, it will ask for a folder for your modes and firmware folders. This uses a different version of the source.js file which will result in a different .ino firmware( primarily the 'handle_button' function ) than vectr 0.3.4 which this is based on.
