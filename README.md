
First to built an application or to make an chip .We have to write the code in the high level language like C with the proper functinality for verification purpose we have to write the test bench after that we model that bolck of code and get some  output. This is called chip  modelling.

  ![image alt](https://github.com/souhardya-ece/RISC-V-Reference-SoC-Tapeout-Program-week0/blob/main/Screenshot%202025-09-20%20133746.png)

The next is that whatever code that we have written in c is converted into haedware descriptive language like verilog.(RTL architechture)
This RTL is sub devided into two parts one is processor and the another one is perepheral/IP's.
This precessor is gate level netlist. Which is synthesizable in nature.
And the IP's is devided into two parts one is macros Which is synthesizable in nature and another one is analog IC Which is non synthesizable in nature.

 ![image alt](https://github.com/souhardya-ece/RISC-V-Reference-SoC-Tapeout-Program-week0/blob/main/Screenshot%202025-09-20%20140315.png)
 
The high level block of code is fed into the SOC integration using GPIO's

![image alt](https://github.com/souhardya-ece/RISC-V-Reference-SoC-Tapeout-Program-week0/blob/main/Screenshot%202025-09-20%20140332.png)

Then we come up with the Physical design process step which include floorplan,placement,clock tree synthesis and routing.So with that end up with the RTL to GDS Flow
and at the end of the Physical design life cycle.
![image alt]()

Then the further process is as follws:- GDSII -> DRC/LVS Checks -> fabrication    (tapeout to tapein)
![image alt]()

