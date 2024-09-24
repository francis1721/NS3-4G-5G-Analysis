## Description and Purpose

This project aims to compare the performance of 4G and 5G cellular technologies using case studies with different traffic types: TCP and UDP.

The purpose of this project is to determine to what extent 5G can achieve the claimed benefits over its predecessors.

## NS3 Modules Used 
- The LTE module will be utilised to simulate the 4G simulations.
- NYU Wirelss' mmwave module will be utilised to simulate the 5G simulation.
- The Mobility Model will be utilised to simulate the UE's movement.
- The Flow Monitor module will be usitilsed to measure the tx bytes, rx bytes, throughput (Mbps) and delay (ns). 

## How to Run

Prequisites: 

- Install NS-3 (version 3.29) with NYU Wireless' mmwave module.

You must copy the .cc files from this project to your 'Scratch' directory within the 'ns3-mmwave' folder.

1. Files are run from the 'mmwave' folder by default with the use of the'./waf --run' command, example below

      ./waf --run scratch/TCPRandomWalk //Note that the file extension is not included

2. Command line options can be set which will overwrite some of the default configurations in the file, example below

      ./waf --run 'scratch/TCPRandomWalk --simTime=500' //This will run the file for 500 seconds instead of the default time set in the file.
