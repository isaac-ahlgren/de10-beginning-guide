# Beginning

Hello! This is a small guide for creating a small digital design for the DE10-Lite.

The motivation for writing this is that the Intel development toolchain can be very intimidated for new people, particularly those who develop with Linux.
There are an overwhelming amount of tools, little gimmicks, and a oversights in the toolchain that are obvious to seasoned developers but completely unintuitive to those who just want to quickly get their feet wet with a design.
I've spent the last week or so encountering and fixing these small issues so this guide is a quick and easy way to get around them so noone has to waste time like I did.

This guide will primarily be about installing and using the development toolchain in Linux.
My guide has been tested on Ubuntu 22.04 and Arch Linux.
The guide will be split into 2 seperate parts: Simulation and Synthesis.
We will first design a small little verilog design and simulate it's functionality using ModelSim.
We will then synthesize the design and flash it onto the DE10-Lite FPGA to see our design in action.

## Table of Contents
- [Simulation](./1_simulation.md)
- [Synthesis](./2_synthesis.md)