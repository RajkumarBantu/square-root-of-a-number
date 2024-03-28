#
The Objective of this task is RT Level simulation and verification of algorithm of sqrt

Algorithm Analysis

There are three registers Rn, Rdelta, and Rdata in the data path to store the  data.we have Rn = Rn + Rdelata and then Rdelta = Rdelta+2 .
The Square Root can be easily obtained by taking the quotient of Rdelta/2 and right shifting the bits of Rdelta by 1 
Steps taken to solve the task

•	For this task we have used modelsim tool
•	First a Project Work is created and sqrt.v and its testbench are loaded into the project
•	Then once its compiled we can begin the simulation
•	Once its simulated we can observe the following waveform
•	The Testbench and Code files are submitted seperately
•	From the below images the squareroot of 25 can be obtained 
•	The initial conditions are set as start=1,clear=1,clk=0

Circuit synthesis and gate-level test bench simulation using Design Compiler and ModelSim

The objective of doing logic synthesis for SQRT

Synthesis is process of transferring higher level of abstraction (RTL) to implementable lower level of abstraction. It is the process of transforming RTL to gate-level netlist.
• Synthesis process can be optimized for Speed(timing)/Area/Testability (DFT)/Power(DFP/Run time.
• Inputs : RTL, Technology libraries, Constraints (Environment, clocks, 10 delays etc.).
• Outputs : Netlist, SDC, Reports etc.
• Design Compiler (DC) from Synopsys and RTL Compiler from Cadence are the tools widely used for synthesis.

Give a top-level overview on the way to solve the problem

•	The first step is to synthesize the verilog file of squareroot using DC Compiler.
•	In order to do that we have to use the compile design and reduce the circuit to gate level
•	Then we have to specify the limits for area,time etc
•	Once this is done a synthesis file is generated 
•	Then by loading this synthesis file in Modelsim we have to test for the same testbench which is written for verilog file 
•	Then the results are verified against the original results


