---
layout: page
title: Projects
permalink: /projects/
---

I am working on multiple research projects and some open-source projects for everybody to enjoy. Check them out below!

## Open-source softwares and projects

### Current
#### [Data Preprocessing Helper](https://howardcheung.github.io/data-preprocessing-helper/)
I made this Windows application to help building engineers to preprocess their building management system (BMS) data for easier analysis in spreadsheet format. Issues it solves includes filling in gaps of data and aligning the recording time of the data. It also works for other types of time-series data as well. Check the website and the repository for more information over [here](https://howardcheung.github.io/data-preprocessing-helper/). The project is mainly built in Python.

![](../raw_img/DataPreprocessingHelper/DataPreprocessingHelper.png "Data Preprocessing Helper")

### Previous
#### [Openstudio fault models](https://github.com/nrel/openstudio-fault-models)                        {#OpenStudioFaultModel}
I worked on this project previously to create models of faults (e.g. deviation from design) of building equipment for building simulation in [OpenStudio](https://www.openstudio.net/). You can download the OpenStudio and EnergyPlus measure scripts in the repository to model the impact of different types of building equipment faults on building thermal performance and energy consumption. You can also read the details of the models I made in the technical report [Development of Fault Models for Hybrid Fault Detection and Diagnostics Algorithm](http://www.nrel.gov/docs/fy16osti/65030.pdf) or conference paper [Hybrid Model-Based and Data-Driven Fault Detection and Diagnostics for Commercial Buildings](http://www.nrel.gov/docs/fy16osti/65924.pdf). The measure scripts are built by Ruby with post-processing being conducted by R.

## Research projects

### Current

#### Data center energy management solution
I am working on energy management solutions such as design and controls of cooling systems in data centers to reduce their cooling system energy consumption. Currently, I have built a model in building simulation programs to estimate the changes of data center power consumption with the status of the computing equipment in a data center.

![](../raw_img/DataCenterCooling/CombinedDiagram2.png "Two building simulation case results showing how server processor utilization rate changes cooling load of a data center")

And I'll move forward to use the information to optimize the designs and controls of data center cooling systems with the model. If you're interested in collaboration, feel free to contact me at <howard.at@gmail.com>!

#### Building energy assessment
I am working on examining the energy-saving potentials and faults in various building systems to reduce their energy consumption. Issues like chiller and pump sequencing, overcooling, low-Delta-T syndromes are being examined, and their control systems are being configured to reduce the unnecessary energy consumption caused by these issues.

![](../raw_img/BuildingEnergyAssessment/ChillerSequencing.png "Histogram showing a chiller plant can run one less chiller according to the BMS analysis")

#### Uncertainty calculation for thermal system applications
I have spent quite some time to work on calculation of uncertainties due to various factors such as regression data measurement uncertainties, choice of regression data, model structure, etc. for thermal system models. There are some publications about the research for compressor models, and the project is still on-going for other thermal applications. If you want to know more, you can look it up at my publication list or contact me directly at <howard.at@gmail.com>!

![](../raw_img/UncertaintyCalculation/CompUncertaintyCalculation.png "Uncertainty calculation that predicts if a model is extrapolating")

### Previous
I am still organizing this section and haven't listed everything yet. In the meantime, check out [my publication list](../publications) for more information!

#### Evaluating performance of a building audit tool
I worked on an evaluation project of the performance of an automatic building audit tool for small commercial buildings. The tool estimates the type of energy uses in a building and diagnoses operation issues that burdens the building energy bills unnecessarily, and building owners can fix the issues to save some money. To know if the tool performance meets its claims, I evaluated its accuracy and reliabililty to estimate the end uses and to conduct the diagnoses using more than 2,000 building simulation scenarios on the cloud. More details can be found at the technical report [Methodology to Assess No Touch Audit Software Using Simulated Building Utility Data](http://www.nrel.gov/docs/fy17osti/66001.pdf).

![](../raw_img/EvaluationBuildingAudit/UncertaintyVSBias.png "A plot of uncertainty vs bias. A point closer to the origin means a more accurate and reliable estimation.")

#### Modeling of HVAC equipment faults in energy models of commercial buildings
Please refer to the development of the open-source software [Openstudio fault models](#OpenStudioFaultModel). In case you don't know, HVAC means heating, ventilating and air conditioning ([Wikipedia](https://en.wikipedia.org/wiki/HVAC)).

#### Inverse modeling to simulate fault impacts for air conditioning equipment
This is my PhD thesis project related to the study of the impact of air conditioner faults on the performance of air-conditioners. How do faults affect the operation mechanisms and hence increase the operation cost of the air conditioners? The faults modeled include

* Under- and over-charging (i.e. too little or too much refrigerant)
* Heat exchanger fouling
* Refrigerant pipeline blockages (i.e. refrigerant pipeline blockages)
* Compressor valve leakages
* Electronic valve opereation failure
* Non-vacuumed air conditioner before charging

and they all show adverse effect to both the cooling capacity and efficiency of the air conditioners. In other words, they increase the operation cost of your ACs. For example, the diagrams below show that air (non-condensable) inside the air conditioner can significantly increase the power consumption, and the lack of charge (refrigerant) can significantly reduce the amount of cooling an air conditioner can deliver.

![](../raw_img/InverseModeling/FaultImpactAirConditioner.png "How air in air conditioner or lack of refrigerant worsen the air conditioner performance.")

The modeling was mainly conducted in MATLAB with a few dynamic libraries written in C++.

#### Low-cost virtual power meter for rooftop units
I developed a low-cost estimator of power consumption of rooftop air conditioners using temperature readings only. With the virtual power meter, only temperature sensors are needed to estimate the power consumption of an air conditioner correctly, and no expensive power meters are needed. This helps the manufacturer to provide power readings of their air conditioners during operation and helps to monitor their energy consumption for building energy management more cost effectively.

#### Testing and Modeling of Dual-Unit Ductless Heat Pump System
I tested the performance of multiple ductless heat pump systems, including one with two indoor units, in psychrometric chambers. This helped to validate the field testing results of these systems for a comparison of their energy efficiency with that of conventional heating systems. I also created empirical models of these systems using the test results to help modeling their performance in building simulation programs, including their performance under defrost operation. To understand how they operated, I also modeled their operation using mechanistic models to examine how the refrigerant flows are controlled inside the indoor units, especially when multiple indoor units are involved.

![](../raw_img/DHPTesting/FrostBuildUp.jpg "Testing the effect of low temperature on heat pump performance.")

### Relevant publications

Here is a listed of publications ordered according to the nature of the projects instead of the type of publication. Note that a publication can appear in this list multiple times if it is related to multiple projects. For a clean list of publications, please read [here](../publications).

#### Building energy assessment
* Cheung, H., Shan, K., Wang, S., (2017), A fault-tolerant control method of balancing valves for condenser fouling in water-cooled chillers, _9th International Conference on Applied Energy_, Cardiff, UK, [[Postprint hosted here]](../raw_files/ICAE-2017-FaultTolerantCtrl.pdf)

#### Data center energy management solution
* Cheung, H., Wang, S., Zhaung, C., (2017), Development of a simple power consumption model of information technology (IT) equipment for building simulation, _9th International Conference on Applied Energy_, Cardiff, UK, [[Postprint hosted here]](../raw_files/ICAE-2017-DataCenterModel.pdf)

#### OpenStudio fault modeling/ Modeling of HVAC equipment faults in energy models of commercial buildings
* Frank, S., Heaney, M., Jin, X., Robertson, J., Cheung, H., Elmore, R. and Henze, G. (2016), Hybrid Model-Based and Data-Driven Fault Detection and Diagnostics for Commercial Buildings, _2016 ACEEE Summer Study on Energy Efficiency in Buildings_, Pacific Grove, California [[External link for a free preprint]](http://www.nrel.gov/docs/fy16osti/65924.pdf)

* Cheung, H. and Braun, J. E., (2015), _Development of Fault Models for Hybrid Fault Detection and Diagnostics Algorithm_, NREL/SR-5500-65030. Golden, CO: National Renewable Energy Laboratory [[External link for a free copy]](http://www.nrel.gov/docs/fy16osti/65030.pdf)

#### Uncertainty calculation for thermal system applications
* Cheung, H. and Wang, S., (2018), Impact of Dynamics on The Accuracies of Different Experimental Data Processing Methods for Steady-state Heat Transfer Rate Measurement, _Journal of Thermal Science and Engineering Applications_, [[DOI link]](http://dx.doi.org/10.1115/1.4037543)

* Cheung, H. and Wang, S., (2017), A comparison of the effect of empirical and physical modeling approaches to extrapolation capability of compressor models by uncertainty analysis: A case study with common semi-empirical compressor mass flow rate models, _International Journal of Refrigeration_, [[DOI link]](https://doi.org/10.1016/j.ijrefrig.2017.11.020)[[Postprint hosted here]](../raw_files/Postprint-withSupp-Cheung-2017-JIJR.pdf)

* Cheung, H., Sarfraz, O. and Bach, C. K., (2017), A method to calculate uncertainty of empirical compressor maps with the consideration of extrapolation effect and choice of training data, _Science and Technology for the Built Environment_, [[DOI link]](http://dx.doi.org/10.1080/23744731.2017.1372805) [[Postprint hosted here]](../raw_files/Postprint-Cheung-2017-STBE.pdf)

* Cheung, H. and Braun, J. E., (2016), Minimizing data collection for field calibration of steady-state virtual sensors for HVAC equipment, _International Journal of Refrigeration_, 69, 96-105, [[DOI link]](http://dx.doi.org/10.1016/j.ijrefrig.2016.05.007)

* Cheung, H. and Braun, J. E., (2016), A general method for calculating the uncertainty of virtual sensors for packaged air conditioners, _International Journal of Refrigeration_, 63, 225-236, [[DOI link]](http://www.sciencedirect.com/science/article/pii/S0140700715001917)

* Bach, C. K. and Cheung, H., (2016), Mapping of Vapor Injected Compressor with Consideration of Extrapolation Uncertainty, _Conference proceedings of ASHRAE Winter Conference 2016_, OR-16-C042 [[External link]](http://www.techstreet.com/products/1910166)

#### Evaluating performance of a building audit tool
* Cheung, H., Braun, J. E. and Langner, M. R., (2016), _Methodology to Assess No Touch Audit Software Using Simulated Building Utility Data_, NREL/SR-5500-66001. Golden, CO: National Renewable Energy Laboratory [[External link for a free copy]](http://www.nrel.gov/docs/fy17osti/66001.pdf)

#### Inverse modeling to simulate fault impacts for air conditioning equipment
* Cheung, H. and Braun, J. E., (2013), Simulation of Fault Impacts for Vapor Compression Systems by Inverse Modeling Part I: Component Modeling and Validation, _HVAC&R Research_, 19:7, 892-906, [[DOI link]](http://www.tandfonline.com/doi/abs/10.1080/10789669.2013.824800)

* Cheung, H. and Braun, J. E., (2013), Simulation of Fault Impacts for Vapor Compression Systems by Inverse Modeling Part II: System Modeling and Validation, _HVAC&R Research_ , 19:7, 907-921, [[DOI link]](http://www.tandfonline.com/doi/abs/10.1080/10789669.2013.819769)

* Yuill, D. P., Cheung, H. and Braun, J. E., (2014), Evaluation of Fault Detection and Diagnostics Tools by Simulation Results of Multiple Vapor Compression Systems. _Proceedings of the 15th International Refrigeration and Air Conditioning Conference at Purdue_, West Lafayette, Indiana [[External link for a free copy]](http://docs.lib.purdue.edu/iracc/1543/)

* Yuill, D. P., Cheung, H. and Braun, J. E., (2014), Validation of a Fault-Modeling Equipped Vapor Compression System Model Using a Fault Detection and Diagnostics Evaluation Tool. _Proceedings of the 15th International Refrigeration and Air Conditioning Conference at Purdue_, West Lafayette, Indiana [[External link for a free copy]](http://docs.lib.purdue.edu/iracc/1544/)

* Cheung, H. and Braun, J. E., (2014), Modeling of Fault Impacts for a Multi-split Ductless Heat Pump System. _Proceedings of the 11th IEA Heat Pump Conference 2014_, Montreal, Quebec [[Preprint]](../raw_files/2014 IEA HP - DHP Fault Modeling Paper.pdf)

* Cheung, H. (2014). Inverse modeling of vapor compression equipment to enable simulation of fault impacts (PhD Dissertation). Purdue University, West Lafayette, IN. [[External link]](http://docs.lib.purdue.edu/dissertations/AAI3668777/) [[File hosted here]]((../raw_files/Final_dissertation_edit.pdf))

* Cheung, H. and Braun, J. E., (2012), Inverse Modeling to Simulate Fault Impacts for Vapor Compression Equipment Part 2:  System Modeling and Validation, _Proceedings of 14th International Refrigeration and Air Conditioning Conference at Purdue_, West Lafayette, Indiana [[External link for a free copy]](http://docs.lib.purdue.edu/iracc/1167/)

* Cheung, H. and Braun, J. E., (2012), Performance Mapping for Variable Ductless Heat Pump Systems in Heating, Cooling and Defrost Operation, _Proceedings of 14th International Refrigeration and Air Conditioning Conference at Purdue_, West Lafayette, Indiana [[External link for a free copy]](http://docs.lib.purdue.edu/iracc/1240/)

#### Low-cost virtual power meter for rooftop units
* Cheung, H. and Braun, J. E., (2016), Minimizing data collection for field calibration of steady-state virtual sensors for HVAC equipment, _International Journal of Refrigeration_, 69, 96-105, [[DOI link]](http://dx.doi.org/10.1016/j.ijrefrig.2016.05.007)

* Cheung, H. and Braun, J. E., (2016), A general method for calculating the uncertainty of virtual sensors for packaged air conditioners, _International Journal of Refrigeration_, 63, 225-236, [[DOI link]](http://www.sciencedirect.com/science/article/pii/S0140700715001917)

* Cheung, H. and Braun, J. E., (2014), Virtual Power Consumption and Cooling Capacity Virtual Sensors for Rooftop Units. _Proceedings of the 15th International Refrigeration and Air Conditioning Conference at Purdue_, West Lafayette, Indiana [[External link for a free copy]](http://docs.lib.purdue.edu/iracc/1535/)

#### Testing and Modeling of Dual-Unit Ductless Heat Pump System
* Cheung, H. and Braun, J. E., (2014), Component-based, gray-box modeling of ductless multi-split heat pump systems, _International Journal of Refrigeration_, 38, 30-45, [[DOI link]](http://www.sciencedirect.com/science/article/pii/S0140700713002855)

* Cheung, H. and Braun, J. E., (2014), Performance Mapping for Variable-speed Ductless Heat Pump Systems in Heating and Defrost Operation, _HVAC&R Research_, 20:5, 545-558, [[DOI link]](http://www.tandfonline.com/doi/abs/10.1080/10789669.2014.917934)

* Cheung, H. and Braun, J. E., (2014), Performance Comparisons for Variable-Speed Ductless and Single-Speed Ducted Residential Heat Pumps, _International Journal of Refrigeration_,  47, 15-25, [[DOI link]](http://www.tandfonline.com/doi/abs/10.1080/10789669.2014.917934)

* Cheung, H., Nyika, S. and Braun, J. E., (2013), Development and Validation of a Mechanistic Model for Variable-Speed Multi-split Heat Pumps, _ASHRAE Transactions_, 119: B1 [[External link]](http://search.proquest.com/openview/d458a4cf287887485fe02d0889e8c1fa/1?pq-origsite=gscholar)

* Cheung, H. and Braun, J. E., (2012), Performance Mapping for Variable Ductless Heat Pump Systems in Heating, Cooling and Defrost Operation, _Proceedings of 14th International Refrigeration and Air Conditioning Conference at Purdue_, West Lafayette, Indiana [[External link for a free copy]](http://docs.lib.purdue.edu/iracc/1240/)

* Cheung, H. and Braun, J. E., (2010), Performance Characteristics and Mapping for a Variable-Speed Ductless Heat Pump, _Proceedings of 13th International Refrigeration and Air Conditioning Conference at Purdue_, West Lafayette, Indiana [[External link for a free copy]](http://docs.lib.purdue.edu/herrick/6/)

