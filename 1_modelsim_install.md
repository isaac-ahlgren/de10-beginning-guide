# Part 1: ModelSim Install

First things first, we need to download a Verilog simulator. For this tutorial, we will be using [ModelSim](https://www.intel.com/content/www/us/en/software-kit/750666/modelsim-intel-fpgas-standard-edition-software-version-20-1-1.html) (link is for both Windows and Linux).

Install dependencies needed to run it with:

```
sudo dpkg --add-architecture i386
sudo apt-get update
sudo apt-get install libc6:i386 libncurses6:i386 libstdc++6:i386 lib32ncurses6 libxft2 libxft2:i386 libxext6 libxext6:i386  
```

Make the installer executable:

```sudo chmod +x ModelSimSetup-20.1.1.720-linux.run```

Run the installer and install ModelSim:

```./ModelSimSetup-20.1.1.720-linux.run ```

Install ModelSim into your home directory.

To use these tools from your command line, add the following line to either `.bashrc` or `.zshrc`.

``` export PATH=$PATH:~/intelFPGA/20.1/modelsim_ase/bin ```

Then close and open your terminal again to load the new configuration.

## Table of Contents
- [Intro](./0_intro.md)
- [ModelSim Install](./1_modelsim_install.md)
- [First Design](./2_first_design.md)
- [Simulation](./3_simulation.md)
- [Quartus Install](./4_quartus_install.md)
- [Synthesis](./5_synthesis.md)
