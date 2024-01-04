# CHEETAH by BeastArcade
CHEETAH by BeastArcade is based on the [Flatbox rev4 by jfedor2](https://github.com/jfedor2/flatbox/tree/master/hardware-rev4) and utilizes the same firmware found on the [GP2040-CE Download Page](https://gp2040-ce.info/downloads/download-page/).

![CHEETAH 2](https://github.com/BeastArcade/CHEETAH/assets/154543056/4b83d867-b2c0-4ea9-a7eb-9baaf58b6d84)
![CHEETAH](https://github.com/BeastArcade/CHEETAH/assets/154543056/9f8f0089-1098-4353-bd26-2551c721a826)


## OVERVIEW OF CHANGES
The goal for this project is to increase the ergonomics and functionality of the original Flatbox rev4.  The 8 action buttons are changed from Vewlix-style to Sega 2P-style, then both hands are rotated inward 15-20 degrees.  The two index finger buttons are aligned symmetrically, resulting in an equal proximity to the "up" button from the neutral hand position.  This also aligns one's shoulders' position, as the hand positions are no longer offset.

Cable-wrap "ears" are added to secure the USB-C cable.  Meant to be used with a 90-degree connector, it helps to prevent disconnects caused by cable pull and diverts force away from the USB-C port.

Auxiliary buttons are changed from the built-in flaps to individual pegs, increasing the confidence with which one can press those buttons blindly.  And it allows for more varied aesthetic choices with respect to color.

A shadow line is added where the top and bottom panels join to keep out dust, provide self-alignment, and improve the case aesthetically.  The thickness of the case is increased 1-2mm so the buttons do not protrude too from the case and bottom out just above level--for ease of double-tapping.  The button wells are extended deeper into the case to help prevent dust.

All keycaps are 22mm in diameter.  Choc v1 switches do not perform as well at the northern and southern extremes with large circular keycaps.  That said, this same issue persists at the smaller 22mm size, though to a much lesser degree.  The keycaps are of an original design, and are optimized for the case.  The stems are 2mm long, have a shallow "[" shape, and (anecdotally) experience less breakage when made in PLA--*as long as they are pulled either straight up or from top/bottom (north/south)*.

Due to the position change of the "up" button, the case's depth is increased.  This change is made without an increase to the PCB size.  Consequently, a "shim" is added to the bottom panel below the PCB which helps to align the board while also filling the empty space one would normally see under the keycap without a shim.  The total case size (with the cable-wrap ears and without depressed buttons) is 218mm x 141 mm x 15mm.

Due the constraints of a 220x220x250 build volume, the button layout is not centered to the case.  A sacrifice had to be made in order to fit the button layout in the original Flatbox's form-factor.  Ideally, the case would be extended out from the left-most button an additional 40-50mm, to align the jump button to the center.  Those with the printing capability have the option of extending the case.

For the PCB, while changes to the silkscreen are obvious, a top ground fill is added to prevent warping of the board during manufacture.  Additionally, to accomodate the change in button layout, the center hole is moved to the left ~5mm.

## 3D PRINTING, PCB ORDERING, & ASSEMBLY

![CHEETAH 5](https://github.com/BeastArcade/CHEETAH/assets/154543056/8865b804-de90-4126-855c-607933f63515)

Although all parts were specifically designed for FDM 3d printing, warping in large flat objects is common in this medium.  Many design decisions are made to reduce warping, but there is no guarantee.  Highly recommend the use of an adhesive (hairspray or gluestick) to increase bed adhesion.  As long as the corners do not lift from the build plate during printing, the parts should fit together as intended.

PCB assembly will require basic soldering skills.  6 tactile switches (through-hole) and 12 hotswap sockets (SMT) will need to be soldered to the board.  Alternatively, the Kailh Choc v1 switches can be soldered directly to the board via the through-holes.<br>
**NOTE: The required hotswap sockets are NOT THE SAME as Cherry MX hotswap sockets.  They are Kailh low-profile hotswap sockets.**

**Recommended Slicer Settings:**<br>
Orientation: Flat side on the bed for Top, Bottom, and Keycaps.  Smaller side on the bed for Pegs.<br>
Layer Height: 0.2mm<br>
Initial Layer Height: 0.2mm<br>
Wall Count: 3<br>
Top Layers: 3<br>
Bottom Layers: 3<br>
Infill: 10% / Honeycomb<br>
Supports: N/A<br>
Material: PLA/PLA+ or PETG (no other materials tested, but should still work)<br>
Build Plate Adhesion: Skirt<br>
Other Settings: As determined by user/printer/filament preferences<br>

**[JLCPCB](https://jlcpcb.com/) Order Recommendations (all settings default unless otherwise specified):**<br>
PCB Type: "Standard PCB/PCBA"<br>
PCB Qty: "50" at the most (to keep it as a small batch)<br>
PCB Color: User Preference<br>
Remove Order Number: "Specify a location"<br>
PCB Assembly: Move Slider to Right<br>
Confirm Product File: "Yes"<br>
Confirm Parts Placement: "Yes"<br>

**Parts Required for Case Assembly:**<br>
x1 Top Panel<br>
x1 Bottom Panel<br>
x12 Keycaps<br>
x4 Silicone Rubber Feet (optional)<br>
x7 M2x6mm Self-Tapping Hex Screws<br>
x1 Hex Screw Driver<br>

**Parts Required for PCB Assembly:**<br>
x12 Kailh Choc v1 Switches<br>
x12 Kailh Low-Profile Hotswap Sockets (optional)<br>
x6 6x6x5mm 4-Pin Tactile Switch<br>
x1 Soldering Iron & Solder Wire<br>

## USER MANUAL

Below is the default button layout for CHEETAH, identical to the Flatbox rev4.

![CHEETAH_Universal_Button_Layout](https://github.com/BeastArcade/CHEETAH/assets/154543056/d1f083ae-1443-42c2-bce2-9f03f3792e74)

By default, CHEETAH is set to PC/XInput mode.  To change CHEETAH's input mode, while unplugged, hold the corresponding button indicated below, plug in the USB cable, then release the button.

![CHEETAH_Mode_Switching](https://github.com/BeastArcade/CHEETAH/assets/154543056/14ff590f-5dba-432a-a7b2-ae73b984a219)

More advanced configuration settings are available via the Web Configurator. To access it, while unplugged, hold the "Start" button, connect CHEETAH to a PC, release the button, then browse to [http://192.168.7.1](http://192.168.7.1).

CHEETAH is fully compatible with PC, PS3, Nintendo Switch, Steam Deck, MiSTer, and Android.  It is also partially compatible with PS4 (limited by an 8-minute timeout).  An adapter such as the [Brook Wingman FGC](https://www.brookaccessory.com/products/wingmanfgc/index.html) enables full PS4 compatibility and partial PS5 compatiblity (fighting games only).

To update CHEETAH's firmware, first download the Flatbox rev4 version of the desired firmware from the [GP2040-CE Download Page](https://gp2040-ce.info/downloads/download-page/).  Then, while unplugged, hold "Start" + "Select" + "Up", connect CHEETAH to a PC, release the buttons, and copy the .uf2 file obtained from the GP2040-CE Download Page into CHEETAH's directory (the RPI-RP2 folder).  After the files are copied over, it will reboot into the new firmware.  Access the Web Configurator to confirm that the firmware was installed successfully.<br>
**NOTE: Recommend [nuking](https://github.com/OpenStickCommunity/GP2040-CE/blob/main/site/docs/downloads/flash_nuke.uf2) the current firmware before installing the updated firmware.**

For the most up-to-date information, visit the [GP2040-CE Info Page](https://gp2040-ce.info/) or join the [OpenStick GP2040-CE Discord](https://discord.gg/k2pxhke7q8).

=-=-=-=-=-=-=-=-=-=-=

CHEETAH by BeastArcade is licensed under [CC-BY-4.0](https://creativecommons.org/licenses/by-sa/4.0/)<br>
Flatbox rev4 by jfedor2 is licensed under [CC-BY-4.0](https://creativecommons.org/licenses/by-sa/4.0/)
