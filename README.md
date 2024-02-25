# OBSPro
This is a different version of the OpenBikeSensor main PCB (checkout https://github.com/openbikesensor/OpenBikeSensor_PCB_Board) with a few design goals:
* Optimized for pick-and-place manufacturing. This means no modules for each functionality, everything is on a single board and SMD parts are widely used.
* Parts only from trustworthy and reliable sources. This also includes that it should be possible to order these parts with a proper bill.
* Software compatibility as far as possible with the original hardware/software.

# PCBA
The PCB is aimed for a production with parts from LCSC and JLCPCB, which are a good mixture of trustworthiness/reliability and price. JLC also offers a PCB assemby service, which is used for manufacturing the board. If you only want up to 10 boards, it is probably not woth it, but for larger orders it is a great option.

# GPS
There are multiple option for the GPS module. You can use any MAX-8* or MAX-10* from u-blox, which cost around 20€ for single quantities. The pinout is also compatible with the ATGM336H-5N* modules from Zhongkewei. It costs only around 5€, but the performance still needs to be evaluated. I recommend using the MAX-M10M module, as this is what I have been using for the tests.

# Firmware
Due to the fact, that the ultrasonic sensing is now based on the PGA460 chip from Texas Instruments and the U-Blox MAX-M10* module has a slightly different command set, the software changes are a bit larger than initially intendet. Nevertheless, the changes/extensions are integrated into the orginal OBS firmware. Currently the source code is hosted over at https://codeberg.org/FabianSchwartau/OpenBikeSensorFirmware in the OBSPro branch. But I hope to get it migrated into the official OBS firmware repo soon.

# Battery
The battery was quite a challenge to get from a decent supplier. The goal was to get a battery with included safety electroinics, so that even a damage to the cable will not be a problem. This means that 18650 cells are not an option. They are also too thick. A flat pack is the proper solution.

There are now two solutions:
* A custom battery made for me, which I will re-sell.
* One of many offerings like the LP-785060 over at [Berrybase](https://www.berrybase.de/lp-785060-lithium-polymer/lipo-akku-3-7v-2500mah-mit-2-pin-jst-stecker). You can find plenty of similar chells on Alibaba/Aliexpress/Ebay/Amazon/...

# The PCB
Here is an image of the board.

![](OBSPro_3D.png)

# Housing
You can find the custom housing in the [mechanics](mechanics) folder. It is fully compatible with the [OBSClassic mouting parts](https://github.com/openbikesensor/OpenBikeSensor3dPrintableCase).

# Cost
Many people are interested in the cost for a sensor, especially when building more than one. Currently there is no detailed list of the cost, but the first 25 demonstrators costed around 1900€, or 76€ per device. This does include VAT, shipping, and everything else. There is still a bit of potential, a few things were more expensive due to the time frame and relatively low quantity.

# Buying
You are of course welcome to use the open source plans to build your own. However, I am planing to sell kits and maybe later fully assembled units. Naturally those will not be sold for the material cost, a factor of 1.5 (kit) and 2.5 (assembled) are common here.

The kit will come with all SMD components fully populted. You just have to solder the through-hole parts, crimp the connectors, add the metal threaded inserts, and screws everything together.

