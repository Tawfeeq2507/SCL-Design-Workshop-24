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
 
## INTRODUCTION TO VLSI DESIGN FLOW
<details>
<summary> INTRODUCTION </summary>
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

In this workshop we focus only on the Standard Cell Based Designing.

</details>

<details>
<summary>SCHEMATIC DESIGN</summary>

In Schematic Design we Design the schematic of the Gates using Transistors and we Design these using the CMOS logic where we have pull up network and a pulldown Network and Name them according to the Industrial Standard Naming of Cells:

![image](https://github.com/Tawfeeq2507/SCL-Design-Workshop-24/assets/142083027/c15de560-6f99-449f-88b0-17e1143bbc58)

**DESIGNS**

1) INV1X1:

![image](https://github.com/Tawfeeq2507/SCL-Design-Workshop-24/assets/142083027/73489db2-e708-4177-8c47-1cf8f1dc89f5)

![image](https://github.com/Tawfeeq2507/SCL-Design-Workshop-24/assets/142083027/db816eef-2f94-4684-8c97-c3b5be31ef77)

Similarly we can design schematic for higher Driving Strength:

**Driving Strength:**
Driving Strength means "driving capacity" of the logic gate, ie if we have 4 NANDS connected to our logic gate to drive them we need wud need enuff driving strength which will lead to the formation of channel in them.The driving strength of a standard cell is determined by various factors including the size and layout of transistors within the cell, the power supply voltage, and the load capacitance it needs to drive. Cells with higher driving strength can handle larger loads and are typically used in critical paths of the design where timing and signal integrity are crucial.
   
2) INV1X2:
we increase the aspect ratio twice to get double the driving rate

![image](https://github.com/Tawfeeq2507/SCL-Design-Workshop-24/assets/142083027/3edc6c5d-dbcd-43cc-bc15-4148dfc3b022)

![image](https://github.com/Tawfeeq2507/SCL-Design-Workshop-24/assets/142083027/a64ff788-03e4-4a9f-a53b-78db42910489)

3) INV1X3:

![image](https://github.com/Tawfeeq2507/SCL-Design-Workshop-24/assets/142083027/1c732e48-20b9-46b4-91c2-d8fa0ea080c5)

![image](https://github.com/Tawfeeq2507/SCL-Design-Workshop-24/assets/142083027/165490fd-ed9f-46bc-b27a-64a5c7cd18cd)

4) INV1X4:

![image](https://github.com/Tawfeeq2507/SCL-Design-Workshop-24/assets/142083027/819190c1-a541-4083-8655-f4168150efc3)

![image](https://github.com/Tawfeeq2507/SCL-Design-Workshop-24/assets/142083027/b9b923e4-2248-4a85-b1da-72cc6e1d3fab)

5) NAND2X1:

![image](https://github.com/Tawfeeq2507/SCL-Design-Workshop-24/assets/142083027/1c592579-aea3-4579-b527-87ead55dc2fb)

6) NAND2X2:

![image](https://github.com/Tawfeeq2507/SCL-Design-Workshop-24/assets/142083027/82206417-7edc-40c9-baa4-242ec03b98a8)

7) NOR2X1:

![image](https://github.com/Tawfeeq2507/SCL-Design-Workshop-24/assets/142083027/0a1f6879-ed29-416a-9ae4-6212c836543f)

![image](https://github.com/Tawfeeq2507/SCL-Design-Workshop-24/assets/142083027/d515f451-f54d-4839-8f77-0fe991324f73)


8) NOR2X2:

![image](https://github.com/Tawfeeq2507/SCL-Design-Workshop-24/assets/142083027/1e14ac8e-689d-485b-8bcd-72ee286abbe2)

![image](https://github.com/Tawfeeq2507/SCL-Design-Workshop-24/assets/142083027/1b8fe776-f849-4ab1-87b4-7f5af4fe606f)

9) AND2X1:

![image](https://github.com/Tawfeeq2507/SCL-Design-Workshop-24/assets/142083027/4877bbd2-38f1-4dd3-b17e-4d66954dee5e)

![image](https://github.com/Tawfeeq2507/SCL-Design-Workshop-24/assets/142083027/a8c37e36-4d1d-45b2-853d-ea0b85918220)

10) AND2X2:

![image](https://github.com/Tawfeeq2507/SCL-Design-Workshop-24/assets/142083027/c8938b0c-9ef9-47bb-b172-569136ec65e8)

![image](https://github.com/Tawfeeq2507/SCL-Design-Workshop-24/assets/142083027/f603563d-e8ca-417d-b0e2-712887564320)

11) OR2X1:

![image](https://github.com/Tawfeeq2507/SCL-Design-Workshop-24/assets/142083027/2b4df79d-76be-4385-80f9-c15cb07a11c9)

![image](https://github.com/Tawfeeq2507/SCL-Design-Workshop-24/assets/142083027/f67ccc4a-ccb9-4386-9502-2426d6d9f791)

12) OR2X2:

![image](https://github.com/Tawfeeq2507/SCL-Design-Workshop-24/assets/142083027/fe501b98-8431-4f1b-ba54-e69fd2d0eda4)

![image](https://github.com/Tawfeeq2507/SCL-Design-Workshop-24/assets/142083027/c6cd8a76-8cf7-49b6-85f3-edad898b3ab6)

</details>

<details>
<summary> SIMULATION </summary>

For Simulating the Designed Schematic designs we will Follow the steps given Below:

STEP 1:

Create a Cellview Symbol of the Designed Schematic with required Input and Output pins Generated.

STEP 2: 

Create a new TEST file to test simulate and test the Schematics we designed, create instance and select the required Symbol from the Your library created.

STEP 3:

we now Add the VDC, GND, CAPACITOR OF 10f Farad  and required Input Voltages and connect them to the respective Inputs and Outputs and create a Pin Vout from which we will generate our Output of the Schematic Design.

STEP 4:

We now perform Transient Analysis and select the outputs from the plot as the inputs and ouputs to be plotted.

</details>

## LAYOUT DESIGNING:

<details>
<summary> STANDARD CELL DESIGN RULES </summary>

Before Designing the Layout there are certain Standard Cell Design Rules that needs to followed by the Designer, The Rules are :

There are 3 Considerations In the Standard Cell Designing which are the **Height, track, Pitch**.

+ Keep Fixed Spacing Between the **HORIZONTAL** and **VERTICAL** gridlines.
+ **Height** of the Track Should be **Fixed**.
+ Metal to Metal connection Via **Contact** are always centered  to crossing.
+ Different Schemes Used in defininf the Pitch Size which are:
  - LINE TO LINE:

    ![image](https://github.com/Tawfeeq2507/SCL-Design-Workshop-24/assets/142083027/cc29a5f6-4543-4a4d-9309-472ac8f6652a)

    Using LINE TO LINE we Have Advantage of using less area but Disadvantage is that we have the Cells Densily Packed with very few spaces left which will lead to it Having very HIGH Routing Grid Density.
    
  - LINE TO VIA:

    ![image](https://github.com/Tawfeeq2507/SCL-Design-Workshop-24/assets/142083027/8c3fd147-e6e2-4aed-b80c-81ca1eaee29e)

    We Have A DRC Error when it comes to using LINE TO VIA.
    
  - VIA TO VIA:
 
    ![image](https://github.com/Tawfeeq2507/SCL-Design-Workshop-24/assets/142083027/792a26aa-007f-4cb1-9eb1-4e84169d8045)

    Using VIA TO VIA During Global routing we have enough spacing to Route without DRC Error.
    
+ Via Pin Positioning : Always place Via Pins on the crossing points of the grid.
+ VDD RAIL - Generally (3-5) Times The minimum width of the Metal1. VDD and GND rail lines are used to provide adequate Current to all the Cells in the ROW.

![image](https://github.com/Tawfeeq2507/SCL-Design-Workshop-24/assets/142083027/ed4c3b92-0caa-4780-8781-e056faaf3508)

+ N-well extension outside the PR Boundary: N-well is extended to That the N-Well of the Neighboring PMOS cells **Merges** giving a Common N-well.
+ PR Boundary: This Gives the Size of the Cell. Its Height is Taken from Centre of VDD and GND rail line and width By excluding the Extentions. 
+ Outside PR Boundary the VDD and GND rails are Extended which helps to **abut** the neighboring Cells Automatically.

![image](https://github.com/Tawfeeq2507/SCL-Design-Workshop-24/assets/142083027/85461aaf-e0d5-4705-bad7-33f90c31a02b)

+ Spacing between and n/p type active region is to provide spacing/isolation Between Neighboring standard cell MOS devices.

Other than these we also take Care of the **LAMBDA RULES** which play an important Role in Providing No **DRC ERRORS**.

</details>









 


















