## ECE 128 Lab 10 README File


## Project Description
This project involved designing an entire system on the FPGA board. The main functionality of the system is to serve as a multiplier with two 4-bit inputs to produce an 8-bit product that is represented visually using LEDs. This lab incorporated previous lab modules such as the combinational multiplier module from Lab 9, as well as RAM and ROM modules from Lab 8. The system design involves reading ROM values and processing them through a register file to prepare for the multiplication using the combinational multiplier. The new main implementation of this lab was a control unit used to connect every component. The output result is written to an address in the RAM, which is then read to output the product of the multiplication onto the FPGA board. 

## How to simulate the program and implement it on the FPGA 
To simulate the program, ensure that each model file is located in the design sources, the constraints files are in the constraints directory, and the testbench file is in the simulation sources directory. Make sure the modules you want to simulate are set to the top in Vivado. To run the simulation, go to the navigator on the left side of Vivado and click run simulation, then run behavioral simulation to output the waveforms of the testbench. 

To program the FPGA with the top_module, make sure the proper module, testbench, and constraint file are selected. Then run the synthesis, implementation, and generate the bitstream. Once the bitstream is generated, open the hardware manager and program the board using the .bit file. 
