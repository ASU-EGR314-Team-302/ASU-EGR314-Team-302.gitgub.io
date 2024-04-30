<!--
Ask team for summaries for this page
-->

# Software Implementation

[Figure 16: Software Proposal](NewSoftwareProposal.pdf)

<object data="NewSoftwareProposal.pdf" width="900" height="900" type='application/pdf'></object>

## Functionality

We designed our system to be temperature-focused. The temperature is the indicator to turn on the fan when reaching the 86-degree threshold. Once the fan is in operation for 20 seconds, it is turned off (this would be 2 minutes if our design became a marketable product). The temperature and humidity are also recorded in the microcontroller and report the readings to the MQTT accordingly through the ESP32 wifi device.

## Design and Decision Making Process

We chose to make our system temperature-focused as when it comes to environmental control. We found this to be the most important as well as the most consistent in determining what the surrounding state is. We also chose the temperature point of 86 degrees as an activation point for the fan as that is where we felt that was a comfortable point here in Arizona during the summer. The fan cuts off after 20 seconds as this was acceptable for demonstration purposes, but 2 minutes would realistically be the cutoff when put to market.  

## Top Five Design Changes

* Rework the timer interrupt once sensors work, for more code fluidity.  
* Add code to manually turn the fan on different levels instead of solely utilizing automatic operation. 
* Rework temperature and humidity conversion equations from raw data.
* Utilize a single sensor to detect both humidity and temperature to reduce confusion in I2C communication. 
* We would also add some additional LEDs that act as error indicators for sensor failures or disconnections. 

## "Version 2.0"

If we were to make version 2.0, first, we would find out why we couldn’t communicate with our I2C sensors. Once we fix this issue we would remove some of the now unnecessary code used to simulate the sensor’s output. We would then utilize some of the commented-out code which would be used to read data from the sensors and output it accordingly. Aside from that, the other issue to be addressed is the SPI not being used. With more time we would properly connect our SPI pins to the motor driver and again, utilize the currently commented-out code to drive our motor according to our sensor’s output. These are the main problems we would address with the code. With all of this done along with the hardware 2.0, we would finally arrive at a product that works as intended and that our group could be more proud of marketing to campers, and other people in more rural areas with poor air conditioning solutions.



<!-- The main loop of our software starts by initializing the system and enabling interrupts. It then checks the humidity and displays it before returning to the start of the loop. Additionally, in that sequence, it checks the temperature and displays it. However, if it reads a temperature below 80 degrees Fahrenheit it will return a 0, it will then return to the start. Conversely, if the reading equals 80 degrees or more, it will return a 1, sending a digital signal to the motor driver, activating the fan for 2 minutes. After running for two minutes, it returns to the loop, allowing the fan to be activated frequently if the device is in a very hot area. 

The humidity sensor has the simplest loop; it initializes, reads the humidity, displays it, and then returns to the beginning loop. Similarly, the temperature sensor initializes the system, reads the temperature, and displays it. However, if the temperature reads as high, it sends a one to the main loop, and if it reads as low, it sends a zero before returning to the beginning. As for the motor driver, it has two actions: the first involves the main loop, where if it receives a digital signal, it activates the fan for 2 minutes before returning to the loop. The other action is for the manual switch of the fan; if the switch is on, it runs the fan, and if the switch is off, it ends the loop. If the switch remains on, it continues to run until it is flipped off. -->





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
