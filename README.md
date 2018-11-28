# Atari Joystick Tester

Lately I've been going through my rather limited amount, but still designated a "sizable pile", of vintage joysticks. Maybe this was to be the year I got around to fixing them - given that we're constantly fast coming up on december, the time to get moving is definitively now. Did not want to subject one of my computers to all that plugging and unplugging while fiddling with wires and resoldering contacts, so the next step of procrastination was designing a simple joystick tester.

Joystick testers are certainly nothing new so based my design on an already existing one, specifically [http://www.mks.purespace.de/technical/c64tester.htm](http://www.mks.purespace.de/technical/c64tester.htm). So, if like me you feel that prototyping boards and the like are too unreliable and finicky to use in practice you can order a set of my PCB to make a more permanent version of it - if you like and prefer prototyping, then there's the page to start with.

![PCB](https://github.com/tebl/Atari-Joystick-Tester/raw/master/gallery/2018-11-18%2000.44.05.jpg)
![PCB](https://github.com/tebl/Atari-Joystick-Tester/raw/master/gallery/2018-11-18%2001.25.23.jpg)


# Schematic
The supplied KiCad files should be sufficient as both a schematic and as a  starting point for ordering PCBs (basically you could just zip the contents of the export folder and upload that on a fabrication site), the schematic is also available in [PDF-format]https://github.com/tebl/Atari-Joystick-Tester/raw/master/export/Atari%20Joystick%20Tester.pdf) and this is what you'll need to print and work your way through this things don't work as expected after assembly.

# BOM
Most parts should be easy to easily get from your favourite local electronic component shop, personally I live around a couple of hours away from the closest one (by plane) so mostly I just use whatever is available via ebay, AliExpress or similar site. Most components coming out of China are good enough for hobby projects such as this, and in quantities usually large enough to build ten of them for less than a somewhat fancy cup of coffee (contents, not counting the actual mug).

Resistor values are highly dependent on the type of LEDs used on the card, usually you'd need to check their datasheets for information on their forward voltage drops and then using that to calculate the proper resistor values to use. Or, just wing it by using 220 for the old style RED/GREEN/YELLOW types, 330 to be safe and 470 for those super-bright modern blue LEDs (you want an indication if it's working, not burn it into your retinas).

| Reference               | Item                                   | Count |
| ----------------------- | -------------------------------------- | ----- |
| PCB                     | Fabricate using Gerber files ([order here](https://www.pcbway.com/project/shareproject/Atari_Joystick_Tester.html))  |     1 |
| J1                      | DB9 male connector (2 rows), PCB mount |     1 |
| J4                      | 3 pin DC barrel connector              |     1 |
| SW1,SW2                 | 3pin SPDT slide-switch                 |     2 |
| R1-R7                   | 220-470 ohm resistor (dependent on LED)|     7 | 
| D1-R7                   | 5mm LED, assorted colors as desired    |     7 | 
