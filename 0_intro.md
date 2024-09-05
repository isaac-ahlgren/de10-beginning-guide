# Beginning

Hello! This is a small guide for creating a small digital design for the DE10-Lite.

The motivation for writing this is that the Intel development toolchain can be very intimidated for new people, particularly those who develop with Linux.
There are an overwhelming amount of tools, little gimmicks, and a oversights in the toolchain that are obvious to seasoned developers but completely unintuitive to those who just want to quickly get their feet wet with a design.
This guide will also go over Windows secific installation issues also when they arise and are substantial. 
I've spent the last week or so encountering and fixing these small issues so this guide is a quick and easy way to get around them so noone has to waste time like I did.

This guide will primarily be about installing and using the development toolchain in Linux.
My guide has been tested on Ubuntu 22.04 and Arch Linux.
We will first design a small little verilog design and simulate it's functionality using ModelSim.
We will then synthesize the design and flash it onto the DE10-Lite FPGA to see our design in action.
Because this is supposed to be beginner friendly, I will be explaining as much of the verilog syntax as possible during my examples.
However, this is not a verilog tutorial. Verilog is a more nuanced language then what I will be covering in my tutorial.
If you want to learn more about it, the best way is to create more projects using your FPGA.

## I think there is an issue!
If you think there is an issue or that something is missing, let me know! I'd appreciate it if you either raise an issue or submit a pull request about the change.

## Table of Contents
- [Intro](./0_intro.md)
- [ModelSim Install](./1_modelsim_install.md)
- [First Design](./2_first_design.md)
- [Simulation](./3_simulation.md)
- [Quartus Install](./4_quartus_install.md)
- [Synthesis](./5_synthesis.md)