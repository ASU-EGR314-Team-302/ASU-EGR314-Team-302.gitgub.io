# Hardware Implementation

[Figure 13: Team Schematic](TeamSchematic3.pdf)

<object data="TeamSchematic3.pdf" width="900" height="900" type='application/pdf'></object>

__NOTE:__ for schematic Bill of Materials (BOM), see [Appendix E](Appendix/AppendixMain.md#bill-of-materials) <!-- update -->

Our design fits our user needs of creating a compact design that monitors temperature as well as humidity. In addition, our design can activate a fan to help regulate surrounding temperatures. This design is battery operated and can be remotely monitored as a set and go design. 

At the heart of our design is our microcontroller. The microcontroller communicates to a temperature sensor as well as a humidity sensor via I2C. These sensors and microcontroller are powered by a 3.2 volt regulator which is powered from a 4.5 battery pack. We also used a motor driver that communicates with the microcontroller via SPI communications. The motor controller regulates a 12V battery input to our fan. The design is simple yet effective.

We tried to choose compact packages in our parts in order to give more flexibility to visual aspects later in the design process. In the end we opted to create a larger housing area to show the scalability of the project as a whole. We also went with a battery powered system that utilizes AA batteries as they provide a larger lifespan when compared to 9 volt batteries. Additionally these are easy to find and are field replaceable as needed. The ESP32 Wifi connector was provided to us to use in the course. 

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

Upon the process of the entire design ideation, we learned many lessons. Overall, our biggest issue was the microcontroller. The controller that we selected wasn’t the best fit for what we actually needed. Since this was the first time the team could select a microcontroller we wanted all the bells and whistles that come with a compact microcontroller. The flaws to this is it required a 5 volt programmer that we couldn’t get to work. If we could go back, we would select a microcontroller that fit our requirements while being simplistic. Additionally, our microcontroller had a small footprint with 48 pins making soldering a challenge. 

<br>

### Links:

[Title Page](index.md)

[Appendix](/Appendix/AppendixMain.md)
