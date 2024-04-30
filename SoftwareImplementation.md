<!--
Ask team for summaries for this page
-->

# Software Implementation

The main loop of our software starts by initializing the system and enabling interrupts. It then checks the humidity and displays it before returning to the start of the loop. Additionally, in that sequence, it checks the temperature and displays it. However, if it reads a temperature below 80 degrees Fahrenheit it will return a 0, it will then return to the start. Conversely, if the reading equals 80 degrees or more, it will return a 1, sending a digital signal to the motor driver, activating the fan for 2 minutes. After running for two minutes, it returns to the loop, allowing the fan to be activated frequently if the device is in a very hot area. 

The humidity sensor has the simplest loop; it initializes, reads the humidity, displays it, and then returns to the beginning loop. Similarly, the temperature sensor initializes the system, reads the temperature, and displays it. However, if the temperature reads as high, it sends a one to the main loop, and if it reads as low, it sends a zero before returning to the beginning. As for the motor driver, it has two actions: the first involves the main loop, where if it receives a digital signal, it activates the fan for 2 minutes before returning to the loop. The other action is for the manual switch of the fan; if the switch is on, it runs the fan, and if the switch is off, it ends the loop. If the switch remains on, it continues to run until it is flipped off.

Below is a PDF showcasing the flow of the systems.

<br>

[Figure 16: Software Proposal](NewSoftwareProposal.pdf)

<object data="NewSoftwareProposal.pdf" width="900" height="900" type='application/pdf'></object>

<!-- <img src="https://github.com/ASU-EGR314-Team-302/ASU-EGR314-Team-302.gitgub.io/blob/main/docs/assets/images/SoftwareDiagram/MainLoop.drawio.png?raw=true" width="732" height="1358">

_Figure 1: Main Loop System_

<br>

<img src="https://github.com/ASU-EGR314-Team-302/ASU-EGR314-Team-302.gitgub.io/blob/main/docs/assets/images/SoftwareDiagram/Humidity.drawio.png?raw=true" width="732" height="1040.38137">

_Figure 2: Humidity Sensor System_

<br>

<img src="https://github.com/ASU-EGR314-Team-302/ASU-EGR314-Team-302.gitgub.io/blob/main/docs/assets/images/SoftwareDiagram/TempSensor.drawio.png?raw=true" width="732" height="1332.50299">

_Figure 3: Temperature Sensor System_

<br>

<img src="https://github.com/ASU-EGR314-Team-302/ASU-EGR314-Team-302.gitgub.io/blob/main/docs/assets/images/SoftwareDiagram/Motor_Fan.drawio.png?raw=true" width="732" height="978.848249">

_Figure 4: Motor/Fan System_ -->




### Links:

[Title Page](index.md)
