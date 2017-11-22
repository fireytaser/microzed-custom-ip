microzed-custom-ip
==================

Custom IP project for the MicroZed

## Requirements

This project is designed for Vivado 2017.3. If you are using an older version of Vivado, then you *MUST* use an older version
of this repository. Refer to the [list of commits](https://github.com/fpgadeveloper/microzed-custom-ip/commits/master "list of commits")
to find links to the older versions of this repository.

* Vivado 2017.3
* [MicroZed 7Z010](http://microzed.org "MicroZed 7Z010")

## Description

This project instantiates a custom IP peripheral that interfaces to the
Zynq PS as an AXI-lite slave. The custom IP contains a multiplier module
that connects to read/write registers which can be accessed by the PS.
The project is designed for and tested on the MicroZed board.

## Installation of MicroZed board definition files

To use this project, you must first install the board definition files
for the MicroZed into your Vivado installation.

The following folders contain the board definition files and can be found in this project repository at this location:

https://github.com/fpgadeveloper/microzed-custom-ip/tree/master/Vivado/boards/board_files

* `microzed_7010`
* `microzed_7020`

Copy those folders and their contents into the `C:\Xilinx\Vivado\2017.3\data\boards\board_files` folder (this may
be different on your machine, depending on your Vivado installation directory).

## Troubleshooting

Check the following if the project fails to build or generate a bitstream:

### 1. Are you using the correct version of Vivado for this version of the repository?
Check the version specified in the Requirements section of this readme file. Note that this project is regularly maintained to the latest
version of Vivado and you may have to refer to an earlier commit of this repo if you are using an older version of Vivado.

### 2. Did you follow the Build instructions in this readme file?
All the projects in the repo are built, synthesised and implemented to a bitstream before being committed, so if you follow the
instructions, there should not be any build issues.

### 3. Did you copy/clone the repo into a short directory structure?
Vivado doesn't cope well with long directory structures, so copy/clone the repo into a short directory structure such as
`C:\projects\`. When working in long directory structures, you can get errors relating to missing files, particularly files 
that are normally generated by Vivado (FIFOs, etc).

## License

Feel free to modify the code for your specific application.

## Fork and share

If you port this project to another hardware platform, please send me the
code or push it onto GitHub and send me the link so I can post it on my
website. The more people that benefit, the better.

## About us

This project was developed by [Opsero Inc.](http://opsero.com "Opsero Inc."),
a tight-knit team of FPGA experts delivering FPGA products and design services to start-ups and tech companies. 
Follow our blog, [FPGA Developer](http://www.fpgadeveloper.com "FPGA Developer"), for news, tutorials and
updates on the awesome projects we work on.