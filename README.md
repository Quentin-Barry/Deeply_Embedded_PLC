Deeply_Embedded_PLC
===================

I wish to start an open source project using the Atmel SAM3S4C with either an FPGA or a CPLD and ELUA. 
The concept being that open source tools are used to generate the VHDL code which can be used to program the Xilinx FPGA,
which will probably be easier that building an onboard JTAG programmer for the CPLD. The FPGA need not be an expensive BGA
type, but a low cost TQFP device. Something along the Spartan 3 series like the Spartan®-3/-3E/-3A TQ144 devices.

I will design the hardware using the selected components and make provision for isolated analogue inputs using the TI 
ADS1234IPW 24 bit A/D converter IC, their XTR111 4-20mA current loop transmitters. Isolation will be accomplished using a 
high speed SPI bus isolated by the Si-Labs Si8442 AB-D which can run up to 150 MHz.

All digital inputs will be optically isolated, including the serial ports. The digital outputs will drive relays. One serial 
port will be dedicated to drive a LCD which will have a serial interface. This leaves the option open to add a graphics
touch screen at a later date.

A wireless transceiver will be fitted using either the TI CC1125 or the Si-Labs Si1000. This should perhaps be a starting
point. Open source tools to create VHDL files and ELUA to run the different processes.