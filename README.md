### Register number : 24901022
### Name : KATHIRESH M
### Experiment 2: IMPLEMENTATION OF BOOLEAN FUNCTION 

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory:**

Implementing Boolean functions in Quartus using Verilog programming involves a systematic approach to design, synthesize, and verify digital logic functions. Here, we’ll cover the theoretical background and implementation of Boolean functions using Verilog, focusing on the functions:

𝐹1=𝐴′𝐵′𝐶′𝐷′+𝐴𝐶′𝐷′+𝐵′𝐶𝐷′+𝐴′𝐵𝐶𝐷+𝐵𝐶′𝐷 𝐹2=𝑥𝑦′𝑧+𝑥′𝑦′𝑧+𝑤′𝑥𝑦+𝑤𝑥′𝑦+𝑤𝑥𝑦

Theory of Boolean Logic in Digital Circuits In digital electronics, Boolean functions describe the relationships between inputs and outputs using binary logic (0s and 1s). These functions are often represented in Sum of Products (SOP) form, where each term (or "product") represents a specific combination of inputs that will produce a high (1) output. The SOP form uses the following logic operations:

AND Operation: Produces a high output only if all inputs are high. OR Operation: Produces a high output if any of the inputs are high. NOT Operation: Produces the opposite of the input (inverts it).

In SOP form, the function is an OR of multiple AND terms, with each AND term representing a unique combination of the inputs that yield a true (1) output.

Analyzing the Boolean Functions F1 and F2 Function F1 Analysis The function F1 is given as: 𝐹1=𝐴′𝐵′𝐶′𝐷′+𝐴𝐶′𝐷′+𝐵′𝐶𝐷′+𝐴′𝐵𝐶𝐷+𝐵𝐶′𝐷 Terms:

𝐴′𝐵′𝐶′𝐷′:True when A,B,C,𝐷 are all zero. AC′D′:True when A is 1, C and D are 0. 𝐵′𝐶𝐷′:True when B is 0, C is 1, D is 0. 𝐴′𝐵𝐶𝐷:True when A is 0, B,C, and D are 1. 𝐵𝐶′𝐷:True when B is 1, C is 0, D is 1. Each terms represents a specific input combination that yields an output of 1 for F1. Function F2 Analysis the function F2 given as: 𝐹2=𝑥𝑦′𝑧+𝑥′𝑦′𝑧+𝑤′𝑥𝑦+𝑤𝑥′𝑦+𝑤𝑥𝑦 Terms: xy'z:True when xix 1,y is 0,z is 1. x'y'z:True when x andd y are 0, z is 1. w'x'y:True when w is 0,x and y are 1. wx'y:True when w,y are 1, and x is 0. wxy:True when w,x,y are 1. Each of these combination results in an output of 1 for F2. Implementing Boolean Functions in Verilog To implement these functions in Verilog, we use logical operators to replicate the behavior of AND, OR, and NOT operations.

AND is represented as &. OR is represented as |. NOT is represented as ~.

And start the verilog code for F1 and F2

Quartus Simulation and Verification Once the Verilog code is written, we can verify the logic using Quartus, an FPGA design and simulation tool.

Steps in Quartus

Create a New Project: Open Quartus, create a new project, and add the Verilog file.

Compilation: Compile the Verilog code to synthesize it into logic gates. Quartus will map the Boolean functions to FPGA resources, ensuring that the code is correctly interpreted.

Testing with a Testbench: To verify the function, create a testbench file that applies various combinations of inputs and observes the outputs F1 and F2.

Simulation: Open the simulation tool in Quartus and select the testbench.Run the simulation and observe the waveforms. Each input combination should produce the expected result for F1 and F2 as per the truth table.

Verify Results: Compare the output waveforms against the expected values to confirm correct operation.

**Logic Diagram**

![WhatsApp Image 2024-12-12 at 18 43 23_192c5539](https://github.com/user-attachments/assets/e853c371-f288-4284-a017-175e56f20d5e)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

![Screenshot 2024-11-21 115027](https://github.com/user-attachments/assets/36056715-5149-42c4-9c5e-ad235c1cb27b)

**Truthtable:**

![image](https://github.com/user-attachments/assets/20453e89-c853-4268-96af-641f6bcd698a)

![WhatsApp Image 2024-11-21 at 11 37 11_cf5478f1](https://github.com/user-attachments/assets/dea62550-6a6e-4266-af5c-1224e8b310d5)



**RTL realization Output:**
![WhatsApp Image 2024-11-21 at 11 37 28_50b25449](https://github.com/user-attachments/assets/e875f7e8-65de-49db-b3c4-21aa39e65297)

**RTL**

**Timing Diagram**
![WhatsApp Image 2024-11-21 at 11 39 41_aa44bcd9](https://github.com/user-attachments/assets/80b7a8bb-1d77-4ad2-bfb1-a20952def3de)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

