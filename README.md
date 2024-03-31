**AIM: **

To simulate and synthesis of DEMULTIPLEXER1TO4 using vivado 2023.2

**APPARATUS REQUIRED:**

vivado 2023

**PROCEDURE:**

STEP:1 Start the vivado software, Select and Name the New project.

STEP:2 Select the device family, device, package and speed.

STEP:3 Select new source in the New Project and select Verilog Module as the Source type.

STEP:4 Type the File Name and module name and Click Next and then finish button.

Type the code and save it.

STEP:5 Select the run simulation and then run Behavioral Simulation in the Source Window and click the check syntax.

STEP:6 Click the simulation to simulate the program and give the inputs and verify the outputs as per the truth table.

STEP:7 compare the output with truth table.



# DEMULTIPLEXER1TO4
![image](https://github.com/RESMIRNAIR/DEMULTIPLEXER1TO4/assets/154305926/b6d81e6c-81ec-4f91-ae42-832a68f8facc)
# Truth Table
![image](https://github.com/RESMIRNAIR/DEMULTIPLEXER1TO4/assets/154305926/bb0a83c7-b4f3-463b-b422-f2ff65b1a0ee)
# Circuit Diagram
![image](https://github.com/RESMIRNAIR/DEMULTIPLEXER1TO4/assets/154305926/dcd56444-97dd-454b-bddf-c7472c4af1de)
![image](https://github.com/RESMIRNAIR/DEMULTIPLEXER1TO4/assets/154305926/03fbbbdf-8ae3-4653-8047-7d4cbf555ccb)
![image](https://github.com/RESMIRNAIR/DEMULTIPLEXER1TO4/assets/154305926/f48cc07d-c76f-4d1c-8907-11e99711b751)
![image](https://github.com/RESMIRNAIR/DEMULTIPLEXER1TO4/assets/154305926/a3075cf9-55ba-4478-b20c-c7128badef04)
![image](https://github.com/RESMIRNAIR/DEMULTIPLEXER1TO4/assets/154305926/e07386db-69b3-4a5f-945f-b38929b801ea)

**verilog code**

module demux(s,I,y );

input I;

input [1:0]s;

output [3:0]y;

assign y[0] = ~s[1]&~s[0]&I;

assign y[1] = ~s[1]&s[0]&I;

assign y[2] = s[1]&~s[0]&I;

assign y[3] = s[1]&s[0]&I;

endmodule

**output**

![demux hdl](https://github.com/nithin2134/DEMULTIPLEXER1TO4/assets/160302970/b9fb1aed-4f7d-4e7b-bb60-b0d659fde1a2)

**result**

Thus the simulation and synthesis of Demltiplexer1to4 using vivado 2023.2 is successfully executed and verified.
