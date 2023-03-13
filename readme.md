# SNAP

![SNAP](https://nullbits.co/static/img/snap10.jpg)

A unique, tweakable split 75% keyboard kit built by nullbits. [More info at nullbits.co](https://nullbits.co/nibble/)

* Keyboard Maintainer: [Jay Greco](https://github.com/jaygreco)
* Hardware Supported: SNAP Rev1, Pro Micro comaptible MCUs.
* Hardware Availability: [nullbits.co](https://nullbits.co/)

Note: If you are seeing issues with MacOS and keyboard hangs after sleep, make sure `NO_USB_STARTUP_CHECK = yes` is set in your rules.mk.

Adds experimental "Remote Keyboard" functionality, which forwards keystrokes from an external macropad, keyboard, or numpad over UART/TRRS, removing the need for an additional USB connection. 

Make example for this keyboard (after setting up your build environment):

    make nullbitsco/snap:default

See the [build environment setup](https://docs.qmk.fm/#/getting_started_build_tools) and the [make instructions](https://docs.qmk.fm/#/getting_started_make_guide) for more information. Brand new to QMK? Start with our [Complete Newbs Guide](https://docs.qmk.fm/#/newbs).

----
## Fork Modifcation
- [x] Reconfigured to Adfuit KB2040 pinout, which the pinout diagram can be found [here](https://github.com/adafruit/Adafruit-KB2040-PCB/blob/main/Adafruit%20KB2040%20Pinout.pdf)
- [ ] Adding Caplock toggle all led to certain color like the post [here](https://www.reddit.com/r/glorious/comments/t9s0yh/comment/i17kkt6/?utm_source=share&utm_medium=web2x&context=3) mentioned and links to the github [here](https://github.com/gourdo1/qmk_firmware/blob/490e1ad77b1fcaf3bc56e97d5cfde2eb70216e6a/keyboards/gmmk/pro/rev1/ansi/keymaps/gourdo1/keymap.c#L244)
- [ ] Need to figuare the onboard Neopixle driver