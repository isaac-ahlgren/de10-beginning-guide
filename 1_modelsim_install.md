# Part 1: ModelSim Install

First things first, we need to download a Verilog simulator. For this tutorial, we will be using [ModelSim] (https://www.intel.com/content/www/us/en/software-kit/750666/modelsim-intel-fpgas-standard-edition-software-version-20-1-1.html) (link is for both Windows and Linux).

Make the installer executable:

```chmod +x ModelSimSetup-20.1.1.720-linux.run```

Run the installer and install ModelSim:

```./ModelSimSetup-20.1.1.720-linux.run ```

Install ModelSim into the `/opt` directory.

To use these tools from your command line, add the following line to either `.bashrc` or `.zshrc`.

``` export PATH=$PATH:/opt/modelsim_ase/bin ```

## Table of Contents
- [Intro](./0_intro.md)
- [ModelSim Install](./1_modelsim_install.md)
- [First Design](./2_first_design.md)
- [Simulation](./3_simulation.md)
- [Quartus Install](./4_quartus_install.md)
- [Synthesis](./5_synthesis.md)
