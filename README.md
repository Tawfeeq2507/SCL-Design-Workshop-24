# SCL-Design-Workshop-24

![image](https://github.com/Tawfeeq2507/SCL-Design-Workshop-24/assets/142083027/b76430f9-a1a2-4d99-bb7d-5af8c24bd7db) 

Hello and welcome to my Github repository of Standard cell designing Workshop.

## Table of Contents

**Introduction to VLSI Design Flow**
+ Schematic Design
  - Design
  - Simulation
  - Analysis

+ Functional Simulation
+ Synthesis

**Standard Cell Design Rules**
+ Standard Cell Design
  - Layout Design
  - Physical Verification - DRC, LVS & RCX
  - Post Layout Simulation
  - Analysis
+ Characterization - Liberty File Creation
+ Abstraction - LEF File Creation
+ Synthesis
+ Gate Level Simulation
 

## Introduction to VLSI Design Flow:

In VLSI Design flow we have two types of Design flows:

1) ASIC - **Application Specific Integrated Circuits** 
2) GPIC - **General Purpose Integrated Circuits**

**Difference Between ASIC and GPIC**

![image](https://github.com/Tawfeeq2507/SCL-Design-Workshop-24/assets/142083027/83f03318-062d-4af0-94dc-02ff1d90112e)

**Design Styles**
In Design flow we have Different Styles of Designing:

![image](https://github.com/Tawfeeq2507/SCL-Design-Workshop-24/assets/142083027/94284881-f70a-4744-8367-b72f15a2052a)

1) **Full Custom Design:** we start designing from the Transistor Level with advantages as very high time and high performance as each and every parameter can be modified.
2) **Semi Custom Design:** under semi custom design we have:
- Standard Cell Based Design.
- Gate Array Based Design.
- FPGA Based Design. 

In this workshop we focus only on the Standard Cell Based Designing:

### SCHEMATIC DESIGN

In SSchematic Design we Design the schematic of the Gates using Transistors and we Design these using the CMOS logic where we have pull up network and a pulldown Network and Name them according to the Industrial Standard Naming of Cells:

![image](https://github.com/Tawfeeq2507/SCL-Design-Workshop-24/assets/142083027/c15de560-6f99-449f-88b0-17e1143bbc58)

**DESIGNS**

1) INV1X1:

![image](https://github.com/Tawfeeq2507/SCL-Design-Workshop-24/assets/142083027/73489db2-e708-4177-8c47-1cf8f1dc89f5)

Similarly we can design schematic for higher Driving Strength:

**Driving Strength:**
Driving Strength means "driving capacity" of the logic gate, ie if we have 4 NANDS connected to our logic gate to drive them we need wud need enuff driving strength which will lead to the formation of channel in them.The driving strength of a standard cell is determined by various factors including the size and layout of transistors within the cell, the power supply voltage, and the load capacitance it needs to drive. Cells with higher driving strength can handle larger loads and are typically used in critical paths of the design where timing and signal integrity are crucial.
   
2) INV1X2:
we increase the aspect ratio twice to get double the driving rate

![image](https://github.com/Tawfeeq2507/SCL-Design-Workshop-24/assets/142083027/3edc6c5d-dbcd-43cc-bc15-4148dfc3b022)

3) INV1X3:

![image](https://github.com/Tawfeeq2507/SCL-Design-Workshop-24/assets/142083027/1c732e48-20b9-46b4-91c2-d8fa0ea080c5)

4) INV1X4:

![image](https://github.com/Tawfeeq2507/SCL-Design-Workshop-24/assets/142083027/819190c1-a541-4083-8655-f4168150efc3)

5) NAND2X1:

![image](https://github.com/Tawfeeq2507/SCL-Design-Workshop-24/assets/142083027/1c592579-aea3-4579-b527-87ead55dc2fb)

6) NAND2X2:

![image](https://github.com/Tawfeeq2507/SCL-Design-Workshop-24/assets/142083027/82206417-7edc-40c9-baa4-242ec03b98a8)

7) NOR2X1:

![image](https://github.com/Tawfeeq2507/SCL-Design-Workshop-24/assets/142083027/0a1f6879-ed29-416a-9ae4-6212c836543f)

8) NOR2X2:

![image](https://github.com/Tawfeeq2507/SCL-Design-Workshop-24/assets/142083027/1e14ac8e-689d-485b-8bcd-72ee286abbe2)

9) AND2X1:

![image](https://github.com/Tawfeeq2507/SCL-Design-Workshop-24/assets/142083027/4877bbd2-38f1-4dd3-b17e-4d66954dee5e)

10) AND2X2:

![image](https://github.com/Tawfeeq2507/SCL-Design-Workshop-24/assets/142083027/c8938b0c-9ef9-47bb-b172-569136ec65e8)

11) OR2X1:

![image](https://github.com/Tawfeeq2507/SCL-Design-Workshop-24/assets/142083027/2b4df79d-76be-4385-80f9-c15cb07a11c9)

12) OR2X2:

![image](https://github.com/Tawfeeq2507/SCL-Design-Workshop-24/assets/142083027/fe501b98-8431-4f1b-ba54-e69fd2d0eda4)




 


















