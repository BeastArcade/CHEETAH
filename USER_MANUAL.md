# USER MANUAL
This is a quickstart guide detailing CHEETAH's essential functions. Full documentation of the GP2040-CE firmware available [here](https://gp2040-ce.info/introduction/).

## BUTTON LAYOUT
![iCHBUT](https://github.com/BeastArcade/CHEETAH-PCB/assets/154543056/5cc47d19-68b1-449c-9ab9-a505c6b346e7)

## SWITCHING INPUT MODE
![iCHMODE](https://github.com/BeastArcade/CHEETAH-PCB/assets/154543056/f7a1ef5e-56fe-4a2b-9531-0dac8add8936)

CHEETAH is fully compatible with PC, PS3, PS4, Nintendo Switch, Steam Deck, MiSTer, and Android. In PS4 mode there is an 8-minute timeout. Using an adapter such as the [Brook Wingman FGC](https://www.brookaccessory.com/products/wingmanfgc/index.html) defeats the timeout and enables PS5 compatibility (for fighting games only).

By default, CHEETAH is set to PC/XInput mode. To change CHEETAH's input mode:

- Unplug CHEETAH (if connected)
- Hold the specified button for the desired mode
- Connect CHEETAH to your PC/Console
- Release the button

## CHANGING D-PAD MODE
The input mode of the directional buttons can be changed while CHEETAH is plugged in.

- D-Pad: `Start` + `Select` + `Down`
- Left Stick: `Start` + `Select` + `Left`
- Right Stick: `Start` + `Select` + `Right`

## CHANGING SOCD MODE
The SOCD Cleaning Method can be changed while CHEETAH is plugged in.

- Up Priority: `Start` + `Home` + `Up`
- Neutral: `Start` + `Home` + `Down`
- Last Wins: `Start` + `Home` + `Left`

## WEB CONFIGURATOR
Several configuration settings are only available via the Web Configurator. To access it:

- Unplug CHEETAH (if connected)
- Hold the `Start` button
- Connect CHEETAH to your PC
- Release the `Start` button
- Open [http://192.168.7.1](http://192.168.7.1) in a web browser

## UPDATING DEVICE FIRMWARE
The steps below include wiping the current firmware, reverting any configuration changes. If you would like to keep those changes, backup your configuration using the Web Configurator before installing new firmware.

To update CHEETAH's firmware:

- Download "[flash_nuke.uf2](https://github.com/dwelch67/raspberrypi-pico/blob/main/flash_nuke.uf2)"
- Download the Flatbox rev5 version of the firmware from the [GP2040-CE Download Page](https://gp2040-ce.info/downloads/download-page/)
- Unplug CHEETAH (if connected)
- Hold `Start` + `Select` + `Up`
- Connect CHEETAH to your PC
- Release the buttons (a RPI-RP2 folder should appear)
- Copy "flash_nuke.uf2" into the aforementioned RPI-RP2 folder
- CHEETAH will reboot and the RPI-RP2 folder will re-appear
- Copy the .uf2 file for the new firmware into the RPI-RP2 folder
- CHEETAH will reboot into the new firmware
- Access the Web Configurator to confirm--the splash page denotes the firmware version.

## SUPPORT
[OpenStick GP2040-CE Discord](https://discord.gg/k2pxhke7q8) <br>
- Join the OpenStickCommunity Discord!
- The "GP2040-CE Support" Channel is available for issues related to devices running the GP2040-CE firmware

[GP2040-CE Info Page](https://gp2040-ce.info/)<br>
- Contains the most up-to-date information
- Includes full documentation for the GP2040-CE firmware

---

CHEETAH by BeastArcade is [Licensed Under CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)

