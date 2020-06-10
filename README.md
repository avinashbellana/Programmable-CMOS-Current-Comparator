# Getting a glance on the IP:
This main aim of this project is to develop a Programmable CMOS current coparator with Hysteresis, i.e., the reference current should be adjustable with a wide range of values without altering the (W/L) values of the MOS transistors. The key idea in developing the circuit is to find parameters in the circuit which are linked directly in the current equation such as a voltage other than the physical parameters. So, we develop a equation in which reference current is a function of a voltage rather than the physical parameters.

This repository has files needed to design and implement a Programmable CMOS current comparator.

1) Download the Understanding CMOS Comparator word doc provided in this repository.
2) Carefully study it to understand the use of this IP and check the references section for the research papers and weblinks for further information on the IP.
3) Download and read the Applications of Current Comparator to understand the practical uses of a current comparator.

# Setting up the simulator:
Steps to install NI multism on windows 10 and opening the schematic provided:
1) go to the following link https://www.malavida.com/en/soft/ni-multisim/#gref 
2) click the download button 
3) open the .exe file from the downloads
4) click ok on the dailouge box opened and unzip the file to your preffered destination on the PC
5) After the files are unzipped click on install NI circuit design suite 14.0 and continue the installation process
6) Download the Basic Circuit with extension .ms14 provided in this repository.
6) Now open NI multism and go to File and click open and browse the downloaded Basic Circuit file and click open.

# Overview of the schematic:
1) Once the steps mentioned above are done in the same order, a schematic circuit opens, which is first circuit required in the process of simulation.
2) You can see that all the components and the Voltage and Current sources are clearly annotated.
3) M1-M7 are the MOS Transistors and the values just adjacent to them are the channel length and width of the MOS respectively.
4) You can understand the working of the circuit by reading the CMOS Comparator Simulations doc file provided in this repository.

# Running the simulations:
1) Now go to Simulate -> Analyses and simulation and select interactive mode of simulation.
2) Click F5 to run the simulation.
3) You can notice the reference current genarated in current measuring probe 2 mentioned as PR2 in the circuit.
4) Make a note of it and you can verify it with the equation provided in the  CMOS Comparator Simulations doc file.
5) Now again go to Simulate -> Analyses and simulation and change it to DC Sweep and choose source as VRef and uncheck 'Use source 2' box.
6) Choose the start value as 0V, stop value as 5V, and Increment as 0.25V. 
7) Go to Output which is present just beside the Analyses parameters tab and check for I(PR4) in the right coloumn, this is the parameter which is to used in the plot.
8) Use Remove to delete any other parameters which are present on the right coloumn. Make sure that you select 'all variables' in the drop down box present in the first coloumn.
9) Now click Run.

You can see a graph plotted, which is plot of I(PR2) vs Vref plot with both the axes named as current. Its just a label and can be changed by double clicking on the label and changing the names to Vref and Iref for X and Y axes respectively.

