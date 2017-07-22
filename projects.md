---
layout: page
title: Projects
permalink: /projects/
---

I am working on multiple research projects and some open-source projects for everybody to enjoy. Check them out below!

## Open-source softwares and projects

### Current
#### [Data Preprocessing Helper](https://howardcheung.github.io/data-preprocessing-helper/)
I made this Windows 64-bit application to help building engineers to preprocess their building management system (BMS) data for easier analysis in spreadsheet format. Issues it solves includes filling in gaps of data and aligning the recording time of the data. It also works for other types of time-series data as well. Check the website and the repository for more information over [here](https://howardcheung.github.io/data-preprocessing-helper/). The project is mainly built in Python.

### Previous
#### [Openstudio fault models](https://github.com/nrel/openstudio-fault-models)                        {#OpenStudioFaultModel}
I worked on this project previously to create models of faults (e.g. deviation from design) of building equipment for building simulation in [OpenStudio](https://www.openstudio.net/). You can download the OpenStudio and EnergyPlus measure scripts in the repository to model the impact of different types of building equipment faults on building thermal performance and energy consumption. You can also read the details of the models I made in the technical report [Development of Fault Models for Hybrid Fault Detection and Diagnostics Algorithm](http://www.nrel.gov/docs/fy16osti/65030.pdf) or conference paper [Hybrid Model-Based and Data-Driven Fault Detection and Diagnostics for Commercial Buildings](http://www.nrel.gov/docs/fy16osti/65924.pdf). The measure scripts are built by Ruby with post-processing being conducted by R.

## Research projects

### Current
#### Building energy assessment
I am working on examining the energy-saving potentials and faults in various building systems to reduce their energy consumption. Issues like chiller and pump sequencing, overcooling, low-$\Delta$T syndromes are being examined, and their control systems are being configured to reduce the unnecessary energy consumption caused by these issues.

#### Data center energy management solution
I am working on energy management solutions such as fault detection and diagnostics and control designs for data centers to reduce their cooling system energy consumption. The project has just started and if you're interested in collaboration, feel free to contact me at <howard.at@gmail.com>!

#### Uncertainty calculation for thermal system applications
I have spent quite some time to work on calculation of uncertainties due to various factors such as regression data measurement uncertainties, choice of regression data, model structure, etc. for thermal system models. There are some publications about the research for compressor models, and the project is still on-going for other thermal applications. If you want to know more, you can look it up at my publication list or contact me directly at <howard.at@gmail.com>!

### Previous
I am still organizing this section and haven't listed everything yet. In the meantime, check out [my publication list](../publications) for more information!

#### Evaluating performance of a building audit tool
I worked on an evaluation project of the performance of an automatic building audit tool for small commercial buildings. The tool estimates the type of energy uses in a building and diagnoses operation issues that burdens the building energy bills unnecessarily, and building owners can fix the issues to save some money. To know if the tool performance meets its claims, I evaluated its accuracy and reliabililty to estimate the end uses and to conduct the diagnoses using more than 2,000 building simulation scenarios on the cloud. More details can be found at the technical report [Methodology to Assess No Touch Audit Software Using Simulated Building Utility Data](http://www.nrel.gov/docs/fy17osti/66001.pdf).

#### Modeling of HVAC equipment faults in energy models of commercial buildings
Please refer to the development of the open-source software [Openstudio fault models](#OpenStudioFaultModel). In case you don't know, HVAC means heating, ventilating and air conditioning ([Wikipedia](https://en.wikipedia.org/wiki/HVAC)).

#### Inverse modeling to simulate fault impacts for air conditioning equipment
This is my PhD thesis project related to the study of the impact of air conditioner faults on the performance of air-conditioners. How do faults affect the operation mechanisms and hence increase the operation cost of the air conditioners? The faults modeled include

* Under- and over-charging (i.e. too little or too much refrigerant)
* Heat exchanger fouling
* Refrigerant pipeline blockages (i.e. refrigerant pipeline blockages)
* Compressor valve leakages
* Electronic valve opereation failure

and they all show adverse effect to both the cooling capacity and efficiency of the air conditioners. In other words, they increase the operation cost of your ACs.

The modeling was mainly conducted in MATLAB with a little bit of C++.
