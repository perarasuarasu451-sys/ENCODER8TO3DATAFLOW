### ENCODER 8TO3 DATAFLOW Modelling

**AIM:**

To implement  Encoder 8 To 3 in Dataflow Modelling using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:** Quartus prime

**THEORY**

**Encoder 8 To 3**

The 8 to 3 line Encoder is also known as Octal to Binary Encoder. In 8 to 3 line encoder, there is a total of eight inputs, i.e., D0, D1, D2, D3, D4, D5, D6, and D7 and three outputs, i.e., A0, A1, and A2. In 8-input lines, one input-line is set to true at a time to get the respective binary code in the output side. Below are the block diagram and the truth table of the 8 to 3 line encoder.

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/0bc242c1-eb9e-4c47-afe5-30428470efc3)

Figure 01  Block Diagram of Encoder 8 * 3

**Truth Table**

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/35496b14-ae6e-4cd1-9abd-d6736b576575)

The logical expression of the term A0, A1, and A2 are as follows:

A0 = D1 + D3 + D5 + D7

A1 = D2 + D3 + D6 + D7

A2 = D4 + D5 + D6 + D7

Logical circuit of the above expressions is given below:

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/95acaee6-c873-4c75-89eb-ef09fb158053)

Figure 02  Encoder 8 * 3

**Procedure**

1.Type the program in Quartus software.

2.Compile and run the program.

3.Generate the RTL schematic and save the logic diagram.

4.Create nodes for inputs and outputs to generate the timing diagram.

5.For different input combinations generate the timing diagram.


**PROGRAM**

```
/* Program for Encoder 8 To 3 in Dataflow Modelling and verify its truth table in quartus using Verilog programming. 

Developed by: Puli Naga Neeraj
RegisterNumber: 212223240130
*/
module encoder83 (a0,a1,a2,d0,d1,d2,d3,d4,d5,d6,d7);
input d0,d1,d2,d3,d4,d5,d6,d7;
output a0,a1,a2;
assign a0 = d1|d3|d5|d7;
assign a1 = d2|d3|d6|d7;
assign a2 = d4|d5|d6|d7;
endmodule
```

Developed by: PERARASU K RegisterNumber: 25004665


**RTL LOGIC FOR Encoder 8 To 3 in Dataflow Modelling**
<img width="863" height="753" alt="encoders circuit" src="https://github.com/user-attachments/assets/93a1fdfc-3af1-41e3-9f3d-325604eb8ea9" />

**TIMING DIGRAMS FOR Encoder 8 To 3 in Dataflow Modelling**
<img width="1310" height="489" alt="encoders wave" src="https://github.com/user-attachments/assets/91a54ba9-86e9-4637-b894-0273d33879e2" />

**RESULTS**
Implementing Encoder 8 To 3 in Dataflow Modelling using verilog and validating their functionality using their functional tables executed successfully



