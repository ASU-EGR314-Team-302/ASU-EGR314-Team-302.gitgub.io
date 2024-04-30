<!--
    Things to update:
        *software Implementation
        *block diagram varification table
        *Proof-Read everything
-->

# Uniform Climate Control


## Team 302 Members:

* Alijah Williams
* Jason Klinkbeil 
* Evan Lininger
* Justin Hanson

## Preparation Date: 4/29/2024

<!--
[Table of Contents](#table-of-contents)  
example of link to a header

[Link to Example Header](page1.md#example-header)
Link to header on other page
-->



## Arizona State University - EGR314 Spring '24 - Professor Kevin Nichols 

# Introduction

<!-- This semester, our team was assigned with creating a mobile weather station that utilizes two different weather condition sensors to record and operate a motor via wifi connection. The allowed sensors are:

* Temperature
* Humidity
* Atmospheric Pressure
* Wind Speed

The motor must additionally be controlled by a motor controller communicating over the I2C or SPI-based protocol. Once completed, the assigned projects will then be displayed at an innovation showcase where a working model is required. -->

This semester, our team embarked on an exciting project tasked with the creation of a portable climate control station designed to provide real-time weather/environmental data and manipulate the surrounding environment. The objective is to incorporate two distinct weather condition sensors capable of accurately measuring a range of environmental parameters such as temperature, humidity, atmospheric pressure, and wind speed. Through a wifi connection, these sensors will transmit data to a central processing unit which will then execute commands to operate a motor. This motor, crucial to the functionality of the Uniform Climate Control device, will be controlled by a motor controller utilizing information produced by the sensors (I2C or SPI-based protocol for communication) to then control the climate in the vicinity. As the culmination of our efforts, the completed project will be displayed at ASU's innovation showcase.

## Table of Contents

1. [Team Organization](TeamOrganization.md)

    1. [Team Charter](TeamOrganization.md#team-charter)

    2. [Mission Statement](TeamOrganization.md#Mission-Statement)

2. [User Needs, Benchmarking, and Rquirements](UserNeeds.md)

    1. [Establishing User Needs and Benchmarcks](UserNeeds.md#establishing-user-needs-and-benchmarks)

    2. [Product Requirements](UserNeeds.md#product-requirements)

3. [Design Ideation](DesignIdeation.md)

4. [Presentation 1](Presentation1.md)

5. [Selected Design](SelectedDesign.md)

    1. [Design Revisions](SelectedDesign.md#design-revisions)

6. [Block Diagram](BlockDiagram.md)

7. [Component Selection](ComponentSelection.md)

    1. [Power Source](ComponentSelection.md#power-source)

    2. [Temperature Sensor](ComponentSelection.md#temperature-sensor)

    3. [Fan Motor](ComponentSelection.md#fan-motor)

    4. [Humidity Sensor](ComponentSelection.md#humidity-sensor)

    5. [Voltage Regulator](ComponentSelection.md#voltage-regulator)

    6. [Motor Controller](ComponentSelection.md#motor-controller)

    7. [Power Budget](ComponentSelection.md#power-budget)

    8. [Microcontroller](ComponentSelection.md#microcontroller)

8. [Hardware Implementation](HardwareImplementation.md)

    1. [User Needs](HardwareImplementation.md#user-needs)

    2. [In-Depth Design Functionality](HardwareImplementation.md#in-depth-design-functionality)

    3. [Team Design](HardwareImplementation.md#team-design)

    4. ["Version 2.0"](HardwareImplementation.md#version-20)

9. [Software Implementation](SoftwareImplementation.md)

    1. [Functionality](SoftwareImplementation.md#functionality)

    2. [Design and Decision Making Process](SoftwareImplementation.md#design-and-decision-making-process)

    3. [Top Five Design Changes](SoftwareImplementation.md#top-five-design-changes)

    4. ["Version 2.0"](SoftwareImplementation.md#version-2.0)

10. [System Verification](SystemVerification.md)

11. [Lessons Learned](LessonsLearned.md)

12. [Future Recommendations](FutureRecommendations.md)

13. [Appendix](Appendix/AppendixMain.md)

<br>

## Table of Figures

1. [Figure 1:  User Needs Part 1.0](UserNeeds.md#establishing-user-needs-and-benchmarks)

2. [Figure 2: User Needs Part 1.1](UserNeeds.md#establishing-user-needs-and-benchmarks)

3. [Figure 3: User Needs Part 2.1](UserNeeds.md#establishing-user-needs-and-benchmarks)

4. [Figure 4: User Needs Part 2.2](UserNeeds.md#establishing-user-needs-and-benchmarks)

5. [Figure 5: User Needs Part 2.3](UserNeeds.md#establishing-user-needs-and-benchmarks)

6. [Figure 6: Ideation Organization - Appearance and Power](DesignIdeation.md)

7. [Figure 7: Ideation Organization - Funcitonality](DesignIdeation.md)

8. [Figure 8: Design 1](DesignIdeation.md)

9. [Figure 9: Design 2](DesignIdeation.md)

10. [Figure 10: Design 3](DesignIdeation.md)

11. [Figure 11: Selected Design](SelectedDesign.md)

12. [Figure 12: Block Diagram Image](BlockDiagram.md)

13. [Figure 13: Team Schematic](HardwareImplementation.md)

14. [Figure 14: PCB Front](HardwareImplementation.md)

15. [Figure 15: PCB Back](HardwareImplementation.md)

16. [Figure 16: Software Implementation](SoftwareImplementation.md)

17. [System Verification Table](SystemVerification.pdf)



<!--

# Team 302 <br> Presentation 1:


[![Presentation 1](https://raw.githubusercontent.com/ASU-EGR314-Team-302/ASU-EGR314-Team-302.gitgub.io/main/docs/assets/images/Checkpoint%201.png)](http://www.youtube.com/watch?v=8Q0dBRQYoR4)

-->
