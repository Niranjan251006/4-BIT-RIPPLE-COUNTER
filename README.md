# 4-BIT-RIPPLE-COUNTER

**AIM:**

To implement  4 Bit Ripple Counter using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**4 Bit Ripple Counter**

A binary ripple counter consists of a series connection of complementing flip-flops (T or JK type), with the output of each flip-flop connected to the Clock Pulse input of the next higher-order flip-flop. The flip-flop holding the least significant bit receives the incoming count pulses. The diagram of a 4-bit binary ripple counter is shown in Fig. below.

![image](https://github.com/naavaneetha/4-BIT-RIPPLE-COUNTER/assets/154305477/cb4b74d4-31ab-4359-95d0-d22e67daba13)

In timing diagram Q0 is changing as soon as the negative edge of clock pulse is encountered, Q1 is changing when negative edge of Q0 is encountered(because Q0 is like clock pulse for second flip flop) and so on.

![image](https://github.com/naavaneetha/4-BIT-RIPPLE-COUNTER/assets/154305477/a573a7d6-014e-4e54-93e6-e2ac9530960b)

![image](https://github.com/naavaneetha/4-BIT-RIPPLE-COUNTER/assets/154305477/85e1958a-2fc1-49bb-9a9f-d58ccbf3663c)

**Procedure**

/* write all the steps invloved */

**PROGRAM**

/* Program for 4 Bit Ripple Counter and verify its truth table in quartus using Verilog programming.

 Developed by:NIRANJAN S
 RegisterNumber: 24900209
~~~
module ripple_counter(

input wire clk,

input wire rst,

output reg[3:0] count

);

always @(posedge clk or posedge rst)

begin

if(rst)

count <= 4'b0000;

else

count <= count + 1;

end

endmodule
~~~

**RTL LOGIC FOR 4 Bit Ripple Counter**
![398441048-673db1ec-f59d-4dbb-8836-6bbf9a92c164](https://github.com/user-attachments/assets/c3a609f0-a866-4a33-81de-2976ab86d4af)

**TIMING DIGRAMS FOR 4 Bit Ripple Counter**
![398441004-033fb14f-7bfc-4c01-b1dc-29d00ee12927](https://github.com/user-attachments/assets/02854ad5-7938-4d68-b69b-fab8a35f48bb)

**RESULTS**
Thus implement 4 Bit Ripple Counter using verilog and validating their functionality using their functional tables is done successfully
