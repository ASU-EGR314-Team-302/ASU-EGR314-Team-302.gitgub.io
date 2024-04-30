# Hardware Implementation

[Figure 13: Team Schematic](TeamSchematic3.pdf)

<object data="TeamSchematic3.pdf" width="900" height="900" type='application/pdf'></object>

__NOTE:__ for schematic Bill of Materials (BOM), see [Appendix E](Appendix/AppendixMain.md#bill-of-materials) <!-- update -->

## User Needs

Our design fits our user needs by creating a compact design that monitors temperature and humidity. In addition, our design can activate a fan to help regulate surrounding temperatures. This design is battery-operated and can be remotely monitored as a set-and-go design. 

## In-Depth Design Functionality

At the heart of our design is our microcontroller. The microcontroller communicates to a temperature sensor and a humidity sensor via I2C. These sensors and microcontroller are powered by a 4.5V battery pack which regulates the voltage down to 3.3 with a 3.3 volt regulator. We also used a motor driver to communicate with the microcontroller via SPI communications. The motor controller regulates a 12V battery input to our fan. The design is simple yet effective. 

## Team Design

We opted for choosing compact package sizes for our parts to give more flexibility to visual aspects later in the design process. In the end, we opted to create a larger housing area to show the scalability of the project as a whole. We also went with a battery-powered system that utilizes AA batteries as they provide a larger lifespan when compared to 9-volt batteries. Additionally, these are easy to find and are field-replaceable as needed. The ESP32 Wifi connector was provided to us to use in the course. 

The below figures show the front and back of our final PCB design.

<!--
The schematic design aligns with our user needs by incorporating all the essential features required to meet user specifications. It integrates a temperature sensor to measure the surrounding temperature and transmit the data to the microcontroller. Additionally, it includes a humidity sensor to monitor the humidity levels of the environment, also relaying this information to the microcontroller. 

The inclusion of a motor driver enhances the device's functionality beyond that of a mere thermometer, allowing for control of the fan. The fan serves to cool during elevated temperatures and features a manual switch for convenient on/off control. The microcontroller plays a pivotal role in orchestrating these components, enabling autonomous activation of the fan during elevated temperatures without user intervention. Furthermore, it facilitates data transmission to a server via Wi-Fi, courtesy of the ESP2 module connected to the microcontroller. 

In summary, the design comprehensively fulfills all user requirements by providing a device capable of temperature and humidity monitoring while effectively cooling the surroundings—an essential feature, particularly in hot regions like Arizona.
-->

![PCB Design Front](https://raw.githubusercontent.com/ASU-EGR314-Team-302/ASU-EGR314-Team-302.gitgub.io/main/docs/assets/images/PCBFront.jpg)

_Figure 14: PCB Front_

<br>

![PCB Design Back](https://raw.githubusercontent.com/ASU-EGR314-Team-302/ASU-EGR314-Team-302.gitgub.io/main/docs/assets/images/PCBBack.jpg)

_Figure 15: PCB Back_

<br>

## "Version 2.0"

If we were to create a "Version 2.0" of our hardware design we would do a overhaul for most of the components we selected. The package sizes for our microcontroller, humidity sensor, temperature sensor, and motor driver were very small and hard to work with. This resulted in a lot of troubleshooting of our PCB in order to get things to work. The team is unsure if the modifications we made are the cause for the errors we experienced with our software processing and we wish we had more time to get to the root of our problems. We also had trouble finding the proper footprint for the esp32 to fit properly on the board. Looking back this could have been solved if some of the team's time was spend making a custom footprint for the component. We would also find a fan with larger blades that provided better cooling capabilities while consuming less power so we could increase efficiency of the entire system.

Other issues we experienced included drill holes for headers that shorted to ground that had to be bypassed, and problems with the snap programmer due to the default programming voltage of our original microcontroller. This forced the team to find a last minute replacment for the controller and wire it in from an external board (pictured below). Looking back, selecting a microcontroller that fit our requirements while having a larger package size and a smaller amount of pins would have greatly benefited our progress on the project.

<img src="docs\assets\images\AssembledPCB.jpg" width="500" height="500">

<br>

### Links:

[Title Page](index.md)

[Appendix](/Appendix/AppendixMain.md)
