# Openlane_Workshop_VSD
This repository will reflect the work done in the Advanced Physical Design Flow workshop, offered by the folks at VSD. It's a 5 day workshop that aims to educate us on the intricacies of Open Source EDA tools and PDKs as used by industry leaders. Furthermore, it uses Openlane flow to help understand the flow of work when it comes to VLSI designs, starting from the RTL level to the GSDII stage, performing the synthesis, placement, floorplanning, routing and sta required to do so.


# Day 1 - An Introduction to OpenLANE

Day 1 kickstarted off with educating us about "chips". Most of us have played around with an Arduino, as electronics enthusiasts and hobbyists, but we've only toyed around with the functionalities of the Arudino, not the brain of the processor itself. The very first lecture of this workshop opened our eyes to what exactly lies in front of us if we choose to this "VLSI" career road, a road that in recent times has been travelled by many. 

Macros, IPs, RISC-V and the software-to-hardware piepline were some of the topics hit upon.

$PDK_ROOT is the parent root directory under which we will find the Skywater PDK files that have been used. Access to 3 main sub-directories, namely, sky130A, skywater-pdk and open_pdks have been provided.

![](Images/day1.8.PNG)

1. Skywater-pdk – Contains all the foundry provided PDK related files
2. Open_pdks – Contains scripts that are used to bridge the gap between closed-source and open-source PDK to EDA tool compatibility
3. Sky130A – The open-source compatible PDK files

### Calling upon OpenLANE ###

The command used to run the OpenLANE flow is ./flow.tcl 

This command is explicitly run in the docker, which should be installed along with the OpenLANE tools, pdks and other files. 

To run OpenLANE interactively, ./flow.tcl -interactive does the trick.

Furthermore, OpenLANE requires different software dependencies to run it, which is provided to it by running the command - package require openalane 0.9

![](Images/day1.1.PNG)

The Designs being run through OpenLANE flow are enlisted below, under the directory openlane/designs

![](Images/day1.5.PNG)

For the duration of this workshop, and for this repository, we will be focussing on the "picorv32a" design.
The design heirarchy for picorv32a is listed below

![](Images/day1.6.PNG)
