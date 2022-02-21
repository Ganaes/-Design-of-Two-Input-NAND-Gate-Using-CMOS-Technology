# Design of Two Input NAND Gate Using CMOS Technology
This repository presents the design of Two Input NAND Gate implemented using Synopsis Custom Compiler. The purpose of this Hackathon is to implement the proposed design in 28 nm PDK (Process Design Kit). As a result of literature survey and Implemantation, this is a final Report Submission for successful completion of  Two Input NAND Gate design and simulation, for Cloud Based Analog IC Design Hackathon.

# Table of Contents
  1. Introduction
  2. NAND Gate
  3. Tools Used
  4. Reference Circuit
  5. Working
  6. Schematic Netlist
  7. Simulation result
  8. References
  9. Acknowledgements
  11.  Author
 
 # Introduction
The trend in design and manufacturing in semiconductor production unit and implementing million and billion number of transistors in a single chip in very large-scale integration increasing day by day.The Logic gates are used to carry out logical operations using single or multiple binary inputs and a single binary output. The input and output of a logic gate are based on certain logic, which is explained using Boolean algebra. Boolean algebra uses only two variables zero or one. The most basic type of logic gates are OR gate, AND gate and NOT gate. In addition to the basic logic gate, there are combination gates like NAND gate, NOR gate, XOR gate, etc made by combining basic logic gates in different ways. The demand for Complementary MOSFET ICs will be continually strong due to its silent features such as low power consumption, reliable performance, low noise, lesser area. There have been many developments in integrated circuits (ICs) with its use in high performance computing, telecommunication, and consumer electronics requirement.  

# NAND Gate
The NAND gate or “NotAND” gate is the combination of two basic logic gates i.e. AND gate and the NOT gate connected in series. It is also called as the universal gates since the combination of these gates can be used to accomplish any of the basic operations. Hence, NAND gate can produce an inverter, an OR gate or an AND gate.
The output of a NAND gate is high when either of the inputs is high or if both the inputs are low. In other words, the output is always high and goes low only when both the inputs are high.

The symbol & Truth table of logic NAND function is,

![1](https://user-images.githubusercontent.com/100135066/154964797-15f3a295-a474-498d-8e35-3f49fc4fe3c0.JPG)
![2](https://user-images.githubusercontent.com/100135066/154965179-f0fe76f9-f8b2-4d4c-975b-8216178e36e1.JPG)

# Tools Used
• Synopsys Custom Compiler:
 The Synopsys Custom Compiler™ design environment is a modern solution for full-custom analog, custom digital, and mixed-signal IC design. As the heart of the Synopsys Custom Design Platform, Custom Compiler provides design entry, simulation management and analysis, and custom layout editing features. This tool was used to design the circuit on a transistor level.

• Synopsys Primewave:
 PrimeWave™ Design Environment is a comprehensive and flexible environment for simulation setup and analysis of analog, RF, mixed-signal design, custom-digital and memory designs within the Synopsys Custom Design Platform. This tool helped in various types of simulations of the above designed circuit.

• Synopsys 28nm PDK:
 The Synopsys 28nm Process Design Kit(PDK) was used in creation and simulation of the above designed circuit.
 
 # Reference Circuit
 ![sch](https://user-images.githubusercontent.com/100135066/154967434-e0fe4c42-948f-4795-be63-3624135700df.JPG)
![schematic](https://user-images.githubusercontent.com/100135066/154967444-73cb0c3a-7db2-4175-9fa2-e421fd4c01f5.JPG)

# Working
The schematic diagram of the two input NAND gate using CMOS demonstrates the employment of two pMOS i.e. M1 and M2 and two nMOS transistor i.e. M3 and M4 fabricated using 28nm technology. Inputs are given at VA and VB and output is obtained at Vout. Input from VA is given to M1 and M4 and input from VB is given to M2 and M3. Source of both M1 and M2 transistors are connected to the VDD and its corresponding drain terminal are connected together to the Vout, i.e. M1 and M2 are parallel. Similarly, the source terminal of M3 is connected to the ground and its corresponding drain terminal is connected to the source of M4 i.e M3 and M4 are in series. pMOS is ON if the input is LOW and OFF if the input is HIGH, nMOS is ON if the input is HIGH and OFF when input is LOW. When both the input VA and VB will HIGH, both nMOS will be on condition and both pMOS will be off condition. Hence the output is connected to ground & we get logic LOW at the output. Similarly, if any one of the inputs (either VA or VB) is low then the circuit will provide logic HIGH at output.

# Schematic Netlist

