# Introduction to FPGA and RTL for trigger in HEP

Codes for getting started with MAX10 FPGA board from a physics perspective.

## Introduction

The MAX_10_Dev_Board presents a compact and low priced FPGA development platform suitable for new
comers to the FPGA world. The on-board Altera/Intel® MAX® 10 FPGA revolutionizes non-volatile
integration by delivering advanced processing capabilities in a low-cost, single chip small form factor
programmable logic device. The board is designed to be used in the simplest possible implementation
targeting the Intel/Altera MAX 10 device up to 2000 LEs.
The MAX_10_Board has a collection of interfaces including two external GPIO headers to extend designs
beyond the MAX_10_Board, on-board USB-to-serial interface device for interfacing to a PC, as well as
general user peripheral with LEDs, 7-segment displays and push-.

See a set of slides for the school here :
- [ICFA : Field Programmable Gate Array (FPGA) Session](https://cernbox.cern.ch/s/iaIdKIaKCcFOSqc)

See the following links for instalation of the toolchain [ quartus + modelsim ] and setting up the connectivity to the Max10 board for programming.
 - [Installation of Quartus Lite](https://www.tifr.res.in/~icfa2023/assets/doc/InstallationSteps.pdf)
 - Inatalation of ModelSim
   - [Linux](https://profile.iiita.ac.in/bibhas.ghoshal/COA_2020/Lab/ModelSim%20Linux%20installation.html) , it is recomended to install the 20.1 version
 - [Installation of drivers for the Max10 Board and an a demo of the toolchain ](https://www.tifr.res.in/~icfa2023/assets/doc/JTAG_Driver.pdf)

## Datasheets and Manuals
 - [Max10 Development Board User manual](https://www.tifr.res.in/~icfa2023/assets/doc/Max10UserManual.pdf)
 - [Max10 Development Board Datasheet](https://www.tifr.res.in/~icfa2023/assets/doc/Max10DataSheet.pdf)

The following excercises have been designed to get you started with the toolchain interface and basics of VHDL programming.

### Exercise 1 : 
 - `1_NOT_BUTTON/`
    - A simple NOT gate is implemented in VHDL.
### Exercise 2 : 
 - `2_LED_blink/`
    - Clock divider connected to LEDs.
### Exercise 3 : 
 - `3_HEX_COUNTER/` 
    - A Counter with outputs encoded and displayed in a 7-Segment Display
### Exercise 4 :
 - `8bit_Counter_modelsim_simulation/`
   - An 8 bit counter is implemented
   - A testbench is developed for checking the logic

### Exercise 5 : Pseudo Random Bits using Linear-feedback Shift Register [ LFSR ]
Available in the [`leanDev`](https://github.com/abunickabhi/FPGA_ICFA_2023/tree/leanDev) branch
 - `5_PseudoRandomNumberGen/`
   - See more information about LSFR [here](https://en.wikipedia.org/wiki/Linear-feedback_shift_register)
   - `5_PseudoRandomNumgerGen/lsfr.vhd`  : Implementation of lsfr
   - `5_PseudoRandomNumgerGen/randomBit.vhd` : Driving an LED with a random bit
   - `5_PseudoRandomNumgerGen/randomNumber.vhd` : Display a random number on the 7-segment display

<<<<<<< HEAD
### More Logic Exercises :
Combinational Logic
Fibonacci Sequence
Pythagorean Theorem Pipeline
Incrementer
Ripple-Carry Adder
Pipelined FPGA Multiplier
Long Division
Finite State Machine

### Your idea that helps in your physics work :
It can be anything that helps you with your thesis and instrumentation work.

=======
### Fix for `libpng`  error
```
sudo add-apt-repository ppa:linuxuprising/libpng12
sudo apt install libpng12-0
```
>>>>>>> ff22077f936b5fa5344dad30cf38bf38c98cb867
- TIFR, Mumbai
- February, 2023
