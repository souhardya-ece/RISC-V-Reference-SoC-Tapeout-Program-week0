# RISC-V Reference SoC Tapeout Program VSD -Week 0

## Introduction :-

First to built an application or to make an chip .We have to write the code in the high level language like C with the proper functinality for verification purpose we have to write the test bench after that we model that bolck of code and get some  output. This is called chip  modelling.

  ![image alt](https://github.com/souhardya-ece/RISC-V-Reference-SoC-Tapeout-Program-week0/blob/main/images/O1.png)

The next is that whatever code that we have written in c is converted into hardware descriptive language like verilog.(RTL architechture)
This RTL is sub devided into two parts one is processor and the another one is perepheral/IP's.
This precessor is gate level netlist. Which is synthesizable in nature.
And the IP's is devided into two parts one is macros Which is synthesizable in nature and another one is analog IC Which is non synthesizable in nature.

 ![image alt](https://github.com/souhardya-ece/RISC-V-Reference-SoC-Tapeout-Program-week0/blob/main/images/O2.png)
 
The high level block of code is fed into the SOC integration using GPIO's

![image alt](https://github.com/souhardya-ece/RISC-V-Reference-SoC-Tapeout-Program-week0/blob/main/images/O3.png)

Then we come up with the Physical design process step which include floorplan,placement,clock tree synthesis and routing.So with that end up with the RTL to GDS Flow
and at the end of the Physical design life cycle.

![image alt](https://github.com/souhardya-ece/RISC-V-Reference-SoC-Tapeout-Program-week0/blob/main/images/O4.png)

Then the further process is as follws:- GDSII -> DRC/LVS Checks -> fabrication    (tapeout to tapein)

![image alt](https://github.com/souhardya-ece/RISC-V-Reference-SoC-Tapeout-Program-week0/blob/main/images/O5.png)

Here one thing that need to be care of is that in each step functionality and specification is same means O1=O2=O3=O4=O5

Then after the fabrication we use that chip in microconreoller.

## Tools Installation:-

### Oracle virtual machine link:- https://www.virtualbox.org/wiki/Downloads

### System Check 

6GB RAM

50 GB HDD

Ubuntu 20.04+

4vCPU

### Tool check:-

### Yosys

```
$ sudo apt-get update
$ git clone https://github.com/YosysHQ/yosys.git
$ cd yosys
$ sudo apt install make (If make is not installed please install it)
$ sudo apt-get install build-essential clang bison flex \
 libreadline-dev gawk tcl-dev libffi-dev git \
 graphviz xdot pkg-config python3 libboost-system-dev \
 libboost-python-dev libboost-filesystem-dev zlib1g-dev
$ make config-gcc
$ make
$ sudo make install 
```

![image alt](https://github.com/souhardya-ece/RISC-V-Reference-SoC-Tapeout-Program-week0/blob/main/images/Yosys.png)

### Iverilog 

```
sudo apt-get update
sudo apt-get install iverilog
```

![image alt](https://github.com/souhardya-ece/RISC-V-Reference-SoC-Tapeout-Program-week0/blob/main/images/iverilog.png)

### gtkwave
```
 sudo apt-get update
sudo apt install gtkwave
```

![image alt](https://github.com/souhardya-ece/RISC-V-Reference-SoC-Tapeout-Program-week0/blob/main/images/gtkwave.png)

![image alt](https://github.com/souhardya-ece/RISC-V-Reference-SoC-Tapeout-Program-week0/blob/main/images/Window.png)



 



