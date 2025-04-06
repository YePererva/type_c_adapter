# [WIP] USB Type C Receptacle to USB 2.0 breakout board

A few breakout boards for USB Type C Receptacle to breadboard and flex ribbon cables.

## Purpose

Fix / upgrade some equipment that is still using previous generation of USB connectors

## Why?

1. Because most of found adapter boards are missing (or have only 1) pull-down 5K1 resistors, while 2 of those are required
2. I also want to have alternative option with EDS protection IC
3. I wanted to have extra opportunity to use 5-pin flat ribbon cable instead of loose wires

Additionally:

- use the size of SMD components that are still solderable manually (0805 Resistors)

## Details

This repository contains 2 kinds of breakout board:

- simple
- with ESD protection: utilizing USBLC6-2SC6 IC (same as used on STM32-Nucleo boards)

Both versions contain:
- 16-pin USB Type Receptacle
- 4-pin regular breadboard-friendly pin-header
- 2 x 5-pin soldering footprints for flat-ribbon cable with the same pitch as USB Micro connector
	- straight pin-out
	- mirrored pin-out

Solder to the footprint depending on the side, you'll install this adapter in your device. Silkscreen provides details regrading the pin-out.

## Visuals

| Variation | Top-view | Bottom view |
| :---         |     :---:      | :---: |
| Simple   | ![Simple top view](images/render/TypeC_simple_top.png)     | ![Simple bottom view](images/render/TypeC_simple_bottom.png)    |
| With ESD     | ![ESD top view](images/render/TypeC_with_ESD_top.png)      | ![ESD bottom view](images/render/TypeC_with_ESD_bottom.png)      |

## Remarks

There are a few tended vias used in these PCB, which is not ussually recomended. However, it seem to be the safest way of having some connections under the USB connector.  


