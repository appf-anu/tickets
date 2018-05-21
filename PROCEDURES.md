### Chamber has frozen

**Causes:**

*[CRIT] Chamber <chamber> temperature spread 3.00.*

**Resolve by:**

1. Ctrl-C the relevant script on jetson.
2. Turn switch on chamber (side of blue column) to OFF position.
3. Turn switch on chamber to ON position.
4. Wait for screen on chamber.
5. Press SELECT on screen using stylus.
6. On the jetson, in the tab for the relevant script, press "Restart" at the top right.
7. Wait 24 hours (spread) for [OK] message on ticket before escalating or closing.

### Camera has failed

**Causes:**

*[OFF] Camera <camera name> deadman*

**Resolve by:**

1. Open chamber.
2. Remove micro-usb power plug from raspberry pi.
3. Switch camera switch to the OFF position, the screen on the camera should show "Cleaning sensor", or give some indication that it is turning off.
4. Wait 10-20s.
5. Switch camera back on, the screen on the camera should turn on and show information, if not escalate.
6. Insert [micro-usb](https://en.wikipedia.org/wiki/USB_(Physical)#Micro_connectors) power plug into raspberry pi, there should be lights on within the raspberry pi (red, green and orange). The particularly important ones are the green and orange lights on the ethernet port (port where the thickest, blue cable plugs in). If there are no lights, escalate.
7. Wait 2 hours for [OK] message on ticket before escalating or closing.

### Raspberry Pi has failed.

**Causes:**

*[OFF] RPi <chamber> deadman*

**Resolve by:**

1. Open chamber and locate Raspberry Pi.
2. Remove [micro-usb](https://en.wikipedia.org/wiki/USB_(Physical)#Micro_connectors) power plug from Raspberry Pi.
3. Insert [micro-usb](https://en.wikipedia.org/wiki/USB_(Physical)#Micro_connectors) power plug into Raspberry Pi, there should be lights on within the raspberry pi (red, green and orange). The particularly important ones are the green and orange lights on the ethernet port (port where the thickest, blue cable plugs in). If there are no lights, escalate.
4. Wait 30 minutes for [OK] message on ticket before escalating or closing.

### Jetson has failed

**Causes:**

*[OFF] RPi jetson deadman*

**Resolve by:**

1. Check power status of Jetson. If the screen is black, check that the screen is turned on. If the Jetson is off go to step 4.
2. Press the gear button at the top right of the screen -> Shutdown -> Restart. Go to Step 6.
3. Remove [IEC C13](https://en.wikipedia.org/wiki/IEC_60320#C13/C14_coupler) power plug from jetson.
4. Wait 1m.
5. Plug [IEC C13](https://en.wikipedia.org/wiki/IEC_60320#C13/C14_coupler) power plug into jetson.
5. If Jetson doesn't turn back on or show anything on screen, escalate.
6. Ensure that the Jetson starts up fully and is running the appropriate scripts.
4. Wait 30 minutes for [OK] message on ticket before escalating or closing.

### Lights have failed

**Causes:**

*[OFF] PAR <chamber> deadman*

*[CRIT] PAR spread*

**Resolve by:**

1. Visually check status of lights.
2. Switch lights off switch exists on light module.
3. Ensure all lights within a chamber are off at the same time before turning them back on.
4. Turn all lights back on.
5. Ctrl-C the relevant script on jetson.
6. On the jetson, in the tab for the relevant script, press "Restart" at the top right.
7. Wait 3 hours (deadman) or 24 hours (spread) for [OK] message on ticket before escalating or closing.


### Chamber has run out of solarcalc file

**Causes:**

*[CRIT] Chamber <chamber> temperature spread 3.00.*

*[CRIT] Chamber <chamber> temperature diff*

*[OFF] PAR <chamber> par deadman*

*[OFF] Chamber <chamber> deadman*

**Resolve by:**

1. Check on jetson for relevant error.
2. Escalate.

