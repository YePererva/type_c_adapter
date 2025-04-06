# [WIP] USB Type C Receptacle to USB 2.0 breakout board

A few breakout boards for USB Type C Receptacle to breadboard and flex ribbon cables.

## Purpose

Fix / upgrade some equipment that is still using previous generation of USB connectors

## Why?

1. Because most of found adapter boards are missing (or have only 1) pull-down 5K1 resistors
2. I also want to have alternative option with EDS protection IC
3. Want to have extra option for us 5-pin flat ribbon cable instead of loose wires

## Details

This repository contails 2 kinds of breakout board:

- simple
- with ESD protection: utilizing USBLC6-2SC6 IC (same as used on STM32-Nucleo boards)

Both versions contain:
- 16-pin USB Type Reptacle
- 4-pin regular breadboard-friendly pin-header
- 2 x 5-pin soldering footprints for flat-ribbon cable with the same pitch as USB Micro connector
	- straight pin-out
	- mirrored pin-out

Solder to the footprint depending on the side, you'll install this adapter in your device. Silkscreen provides details regrading the pin-out.


