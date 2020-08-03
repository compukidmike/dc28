# Car Hacking Village Badge 2020

This year we teamed up with the Car Hacking Village to bring you an awesome badge!

![Badge Front](/images/front.png)

The badge features two automotive ethernet media converters, which allow you to connect automotive ethernet devices to a standard ethernet network. Since there isn't a universal connector for automotive ethernet, the badge has a tool-less wire connector so you can connect any twisted wire pair to it.


## What is Automotive Ethernet?

Automotive ethernet is very similar to regular ethernet, but it runs over a single twisted pair instead of 2-4 pairs. For those of you who know the ins and outs of ethernet, it's just a different PHY. The badge is composed of back-to-back PHYs that transparently convert between the two physical formats. There are some small differences, like fixed speed (no auto-negotiation) and there is a Primary and Secondary side. The badge has two of these converters that run at 100Mbps. 

## Using the Badge

![Badge Back](/images/back.png)

There is a mode button on the back of the badge. Pressing it cycles through the various modes. There are 4 blinky modes and 4 ethernet modes. The ethernet modes use the bottom "thruster" LEDs to indicate the status of the automotive ethernet ports (see picture). The different modes allow you to change the Primary/Secondary setting for each automotive ethernet port.

The badge can be powered from batteries or USB. The batteries won't last long with the ethernet functions enabled, so USB power is suggested unless you just want the blinky lights.

NOTE: When using the ethernet functions, the badge will get warm. This is normal.

## Firmware Updates

If new firmware is released, it can be flashed via USB without any special tools. If you hold the mode button when turning on the badge while it's connected via USB, it will enter firmware update mode. It will show up as a flash drive on your computer. You can simply delete the "firmware.bin" file and copy the new firmware to it. Then power cycle it and the firmware is updated!

## Source (Code and Board Files)

Unfortunately I'm under NDA from NXP for the automotive ethernet chip. I'm working with them to see what I can release (the public datasheet doesn't even have the pinout, so releasing the code and schematic/board files might not happen). 
