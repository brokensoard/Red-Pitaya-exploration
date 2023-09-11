# Red-Pitaya-exploration
Experiments with the red Pitaya FPGA

This repository will contain ongoing experiments with the Red Pitaya 122.88-16 SDR FPA development board. I'll document the board and the development process using Vivado. As a beginner in FPGA Development, I hope that some of this work will be useful as others learn to develop on the platform.

The red_pitaya_barebones.tcl script was taken by building the LED Blink project and deleting all the IPs except the system 7 IP. Then, using the write_bd_tcl command, this script was created. It can be run to begin a new project by placing the script in the project directory. the new project will have a block design with the system 7 IP and all correct parameters to build on the STEM 122.88-16 SDR red pitaya board.

# red-pitaya-edt
The edt-red-pitaya.tcl script will recreate the edt project from teh xilinx tutorial. This example only sues the Zynq7 processing system and is then coupled with a hello world example that prints to the consle (via the USB console port). the main configurtion options that need to be set for the red-pitaya board are the DDR memory part, MT41J256M16 RE-125, and the DDR BUS Width, 16 bit.