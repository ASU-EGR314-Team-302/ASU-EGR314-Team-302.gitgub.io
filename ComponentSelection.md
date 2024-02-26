<!--
Add appendix for other options that weren't chosen.
-->

# Component Selection

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
| - Inexpensive | Small package size; difficult to solder |
| - Simple footprint and datasheet | 30 week manufacture lead time |
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
| - Has a voltage input max of 14V which gives us more to work with in terms of battery voltage |  |
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

## Power Budget

[Link to Power Budget](Power%20Budget%20Example.html)

<!--
__NOTE:__ See [Appendix E](/Appendix/AppendixMain.md#appendix-e) for other component considerations. 
-->