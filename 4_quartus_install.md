# Installing Quartus

Now that we have a design that we know works in simulation, we are going to flash the desgin to our FPGA.

Before that however, we must first must install [Quartus] (https://www.intel.com/content/www/us/en/software-kit/661017/intel-quartus-prime-lite-edition-design-software-version-20-1-for-linux.html).

Make the installer executable:

```chmod +x qinst-lite-linux-23.1std.1-993.run```

Run the installer and install Quartus:

```./qinst-lite-linux-23.1std.1-993.run ```

Install Quartus into the `/opt` directory.

To use these tools from your command line, add the following line to either `.bashrc` or `.zshrc`.

``` export PATH=$PATH:/opt/quartus/bin ```

Next, we need to setup the USBBlaster driver for Linux.

We first need to set up the `udev` rules for USBBlaster.

```
cd /etc/udev/rules.d
sudo vim 92-usbblaster.rules
```

Add the following line to the rules file:

```SUBSYSTEM=="usb",ENV{DEVTYPE}=="usb_device",ATTR{idVendor}=="09fb",ATTR{idProduct}=="6001",MODE="0666"```

Next, we are going to fix the libraries for the JTAG interface.

Enter the following commands to do so:

```
cd /lib/x86_64-linux-gnu/
sudo ln -sf libudev.so.1 libudev.so.0
```

## Table of Contents
- [Intro](./0_intro.md)
- [ModelSim Install](./1_modelsim_install.md)
- [First Design](./2_first_design.md)
- [Simulation](./3_simulation.md)
- [Quartus Install](./4_quartus_install.md)
- [Synthesis](./5_synthesis.md)