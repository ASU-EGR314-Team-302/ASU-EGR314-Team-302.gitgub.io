# Block Diagram

Our approach to creating our block diagram began with determining the sensors needed for our project, as two were required. We opted for a temperature sensor and a humidity sensor, given their complementary nature. Both sensors utilize analog signals and are thus connected to ADC pins on our microcontroller. Additionally, we incorporated a motor driver into the system, linking it to both the PWM pin and a digital output pin on our microcontroller.

To ensure compatibility, we selected components designed to operate on 3.3 volts, facilitated by a voltage regulator. These components include the microcontroller, ESP2 Module, humidity sensor, temperature sensor, and motor driver. Notably, our system comprises two power supplies, with the 12-volt battery pack dedicated to powering our fan/motor. The inclusion of the ESP2 module in our block diagram is crucial as it enables Wi-Fi connectivity. We integrated a push button into the diagram to facilitate manual on/off control, connected to a digital input pin. Lastly, the snap programmer, essential for debugging purposes, is connected to the ICSP pin.

<br>

[_Figure 12: Block Diagram Image_](https://github.com/ASU-EGR314-Team-302/ASU-EGR314-Team-302.gitgub.io/blob/main/docs/assets/images/BlockDiagram.jpg?raw=true)

<object data="BlockDiagram.pdf" width="900" height="900" type='application/pdf'></object>
<!--
<img src="https://raw.githubusercontent.com/ASU-EGR314-Team-302/ASU-EGR314-Team-302.gitgub.io/main/docs/assets/images/BlockDiagram.jpg" witdth="599" height="622">
-->

### Links:

[Title Page](index.md)