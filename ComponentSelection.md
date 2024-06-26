<!--
Add appendix for other options that weren't chosen.
-->

# Component Selection

__NOTE:__ See [Appendix G](/Appendix/AppendixMain.md#appendix-g) for other components considered.

## Power Source


<img src="https://github.com/ASU-EGR314-Team-302/ASU-EGR314-Team-302.gitgub.io/blob/main/docs/assets/images/ComponentSelection/Battery3.png?raw=true" width="241" height="178">

### [Energizer Replacable AA Batteries](https://www.digikey.com/en/products/detail/energizer-battery-company/EN91/704822)

__Price:__ $0.69 each

<br>

| Pros | Cons |
|    ---    |    ---    |
| - Low cost | - Multiple required to reach higher voltages (1.5V each)
| - Compact | - Non-rechargable
| - High capacity (2000mAH each) | - More expensive over time

<br>

__Rationale:__ 

The Energizer AA batteries are the best inexpensive choice for our design. Also, When creating a mobile station, having an easy-to-move, lightweight power solution is vital to the design. Additionally, replacement batteries readily available in the consumer market.

<br>

## Temperature Sensor


<img src="https://github.com/ASU-EGR314-Team-302/ASU-EGR314-Team-302.gitgub.io/blob/main/docs/assets/images/ComponentSelection/Temp3.png?raw=true" width="250" height="250">

### [SENSOR DIGITAL -40C-125C SOT23-5](https://www.digikey.com/en/products/detail/microchip-technology/TC74A4-3-3VCTTR/443268)

__Price:__ $1.15

<br>

| Pros | Cons |
|----------|----------|
| - Inexpensive | - Small package size; difficult to solder |
| - Simple footprint and datasheet | - 30 week manufacture lead time |
| - Easy to implement in a system |  |

<br>

__Rationale:__ 

The rationale behind choosing this device is the fact that it is easy to work with and executes the ideal function that we need it to. It is easy to incorporate into our system compared to other sensors that will need to be baked on and it is easy to code with on top of that. Additionally, it is inexpensive so more can be purchased to experiment designs.

<br>


## Fan Motor


<img src="https://github.com/ASU-EGR314-Team-302/ASU-EGR314-Team-302.gitgub.io/blob/main/docs/assets/images/ComponentSelection/Fan1.png?raw=true" width="250" height="250">

### [P/N : FAN AXIAL 80X25MM 12VDC WIRE](https://www.digikey.com/en/products/detail/sunon-fans/MF80251V1-1000U-A99/6198742)

__Price:__ $5.35

<br>

| Pros | Cons |
|----------|----------|
| - Large fan to maximize air flow (80mm x 80mm) | - Large Power Consumption at 1.44W (preferred 1 W) |
| - Large Voltage range at 4.5 ~ 13.8VDC | - Missing fan guards, would need to be purchased/made separately |
| - Fan and motor come as one unit.  | - Large, Rectangular design could be hard to design around |

<br>

__Rationale:__ 

When comparing the current draw, this option stands out as the most efficient choice, offering significant advantages over alternatives. Additionally, the square box design not only enhances aesthetics but also facilitates a smoother mounting experience, ensuring seamless integration into various setups. Moreover, the two-wire design simplifies installation procedures, further enhancing its appeal for users seeking convenience and ease of use. 

<br>

## Humidity Sensor


<img src="https://github.com/ASU-EGR314-Team-302/ASU-EGR314-Team-302.gitgub.io/blob/main/docs/assets/images/ComponentSelection/Humidity1.png?raw=true" width="250" height="250">

### [SHT40-AD1B-R3 SENSOR HUMIDITY 100 RH SMD](https://www.digikey.com/en/products/detail/sensirion-ag/SHT40-AD1B-R3/14322745?utm_adgroup=&utm_source=google&utm_medium=cpc&utm_campaign=PMax%20Shopping_Product_High%20ROAS%20Categories&utm_term=&utm_content=&gad_source=1&gclid=Cj0KCQiA2eKtBhDcARIsAEGTG41s33z3UHhaN_Wfv7frLkhKEVcCBNEsK3b1XG1w6-CIsAzgrqwDjcsaAtFmEALw_wcB)

__Price:__ $2.49

<br>

| Pros | Cons |
|----------|----------|
| - Ability to measure humidity from 0 degrees Celsius to 100 degrees Celsius. | - It can only operate at a maximum voltage of 3.6V. |
| - Can operate at a voltage as low as 1.08V. | - Very difficult to solder as there are no pins, necessitates soldering with heat pad. |
| - Can measure both humidity and temperature |  |

<br>

__Rationale:__ 

The reasoning behind this choice is that it has the most informative data sheet, is the cheapest of the options, and still retains similar, if not better quality when compared to the other options. It complies with the requirements for a surface mount environmental sensor and works best at 3.3V which is the necessary voltage for the sensors used for this project. 

<br>

## Voltage Regulator


<img src="https://github.com/ASU-EGR314-Team-302/ASU-EGR314-Team-302.gitgub.io/blob/main/docs/assets/images/ComponentSelection/Voltage2.png?raw=true" width="250" height="250">

### [IC REG LIN POS ADJ 1A/1A HRP-5](https://www.digikey.com/en/products/detail/rohm-semiconductor/BA3259HFP-TR/2673685?s=N4IgjCBcoGwJxVAYygMwIYBsDOBTANCAPZQDaIALAAxwDMdIAuoQA4AuUIAymwE4CWAOwDmIAL6EArAHZaiECkgYcBYmRBxp1OcxDtOPASPGEwFAEwJoCtFjyESkcmC1gwkpqw6RufIaLEJEHN1WgA6WgA1AAIANyJMNnRhXGjeXGEAV0x0NiJeJjEgA)

__Price:__ $0.84

<br>

| Pros | Cons |
|----------|----------|
| - Outputs 3.3V which is required for the project. | - If there is any different voltage requirements this regulator will most likely not work |
| - Has a voltage input max of 14V which gives us more to work with in terms of battery voltage | - Being surface mount it may be difficult to solder for our project |
| - Inexpensive |  |

<br>

__Rationale:__ 

This regulator was selected because it suits most of our power supply needs as for the microcontroller we need 3.3V. Additionally, this device has a voltage input max of 14V which allows us to be far more flexible without batteries and power supply which is important when we consider what it might take to power the fan.

<br>

## Motor Controller


<img src="https://github.com/ASU-EGR314-Team-302/ASU-EGR314-Team-302.gitgub.io/blob/main/docs/assets/images/ComponentSelection/MotorCon1.png?raw=true" width="250" height="250">

### [P/N: IC MOTOR DRVR UNIPLR 8SO PWRPAD](https://www.digikey.com/en/products/detail/texas-instruments/DRV8870DDAR/5428828)

__Price:__ $2.13

<br>

| Pros | Cons |
|----------|----------|
| - High current rating (3.6A) | - Voltage output may be larger than what we need. |
| - Outputs a large range of voltage. (6.5 - 45V) | - Requires additional input for low current. |
| - Compact Design | - Requires a large ground. |

<br>

__Rationale:__ 

We choose this motor controller because it is small and easier to integrate into our system through soldering. Rather than having to bake it on or solder a lot of pins it works with only 8 pins. Additionally, it has ecad and footprint models in digikey which allows us to implement it into our schematic and PCB’s far more easily. Meets the requirements of what we need in a motor driver for our product.

<br>

## Microcontroller

<img src="https://github.com/ASU-EGR314-Team-302/ASU-EGR314-Team-302.gitgub.io/blob/main/docs/assets/images/ComponentSelection/PIC18F57K42.jpg?raw=true" width="250" height="250">

### [PIC16F1847-I/PT](https://www.digikey.com/en/products/detail/microchip-technology/pic18f57k42-i-pt/7561735)

__Price:__ $2.84

|  |  |
| --- | --- |
| GPIO Pins | 44 |
| ADC Pins | 43 |
| PWM's | 4 |
| I2C/SPI | 5/3 |
| UART | 4 |
| Supply Voltage Range | 2.3-5.5V |
| Absolute Max Current | 350mA |
| Max GPIO Current | +-50mA |
| Bit Architecture | 8-bit |
| Overall Pros | Has a PWM and gives us many options for future growth |
| Overall Cons | - Has more pins than we would need<br>- Has higher current draw than similar products |

<br>

__Rationale:__ 

Choosing this microcontroller allows us to have future expansion options while only requiring a minimal increase in current draw when compared to other microcontrollers. Having several PWMs as well as more I2Cs than we need will cover any changes in the design at a later date.

__NOTE:__ See [Appendix F](/Appendix/AppendixMain.md#appendix-f) for other microcontroller considerations.

<br>


### Controller Used in Final Assembly

<img src="https://raw.githubusercontent.com/ASU-EGR314-Team-302/ASU-EGR314-Team-302.gitgub.io/main/docs/assets/images/ComponentSelection/PIC18LF26K40.jpg" width="250" height="250">

### [PIC18LF26K40](https://www.digikey.com/en/products/detail/microchip-technology/PIC18LF26K40-I-SO/6623494)

__Price:__ $1.86

|  |  |
| --- | --- |
| GPIO Pins | 25 |
| ADC Pins | 24 |
| PWM's | 2 10-Bit |
| I2C/SPI | 2 |
| UART | 2 |
| Supply Voltage Range | 1.8-3.6V |
| Absolute Max Current | 350mA |
| Max GPIO Current | +-50mA |
| Bit Architecture | 8-bit |
| Overall Pros | Has a PWM and gives us many options for future growth as well as being easy to solder and work with |
| Overall Cons | - Has as smaller supply voltage range than previous microcontroller<br>- Has fewer I2C and SPI pins |
<br>

## Power Budget

Our power budget includes two power supplies as we have a component that requires more
than 3.3 volts. Our first power supply utilizes a 4.5 volt battery pack that is regulated down to 3.3
volts utilizing our voltage regulator. The systems that run off the 3.3 volt regulator are the
temperature sensor, Humidity sensor, the microcontroller, and the motor driver . The reason for
this is that all of the devices have an operating range between around 3 and 6 volts and thus
belong on the same power rail. 

Our second power supply utilizes 12 volts connected to a 12 volt
regulator and is for our fan as its operating range is above 3.3 volts and its max operating
voltage is 14 volts so to get the most out of it we utilized 12 volts. The battery life of both these
systems is 2.5 hours for the 4.5 volt battery pack and 2 hours for the 12 volt battery pack.


[Link to Power Budget](PowerBudget.pdf)

<object data="PowerBudget.pdf" width="900" height="900" type='application/pdf'></object>


### Links:

[Title Page](index.md)

[Appendix](/Appendix/AppendixMain.md)


