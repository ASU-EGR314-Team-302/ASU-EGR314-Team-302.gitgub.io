# Hardware Proposal

[Figure 13: Team Schematic](TeamSchematic3.pdf)

<object data="TeamSchematic3.pdf" width="900" height="900" type='application/pdf'></object>

__NOTE:__ for schematic Bill of Materials (BOM), see [Appendix E](Appendix/AppendixMain.md#bill-of-materials) <!-- update -->

The schematic design aligns with our user needs by incorporating all the essential features required to meet user specifications. It integrates a temperature sensor to measure the surrounding temperature and transmit the data to the microcontroller. Additionally, it includes a humidity sensor to monitor the humidity levels of the environment, also relaying this information to the microcontroller. 

The inclusion of a motor driver enhances the device's functionality beyond that of a mere thermometer, allowing for control of the fan. The fan serves to cool during elevated temperatures and features a manual switch for convenient on/off control. The microcontroller plays a pivotal role in orchestrating these components, enabling autonomous activation of the fan during elevated temperatures without user intervention. Furthermore, it facilitates data transmission to a server via Wi-Fi, courtesy of the ESP2 module connected to the microcontroller. 

In summary, the design comprehensively fulfills all user requirements by providing a device capable of temperature and humidity monitoring while effectively cooling the surroundings—an essential feature, particularly in hot regions like Arizona.

![PCB Design Front](https://raw.githubusercontent.com/ASU-EGR314-Team-302/ASU-EGR314-Team-302.gitgub.io/main/docs/assets/images/PCBFront.jpg)

_Figure 14: PCB Front_

<br>

![PCB Design Back](https://raw.githubusercontent.com/ASU-EGR314-Team-302/ASU-EGR314-Team-302.gitgub.io/main/docs/assets/images/PCBBack.jpg)

_Figure 15: PCB Back_


<br>

### Links:

[Title Page](index.md)

[Appendix](/Appendix/AppendixMain.md)
