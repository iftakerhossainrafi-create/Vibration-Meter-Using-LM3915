# Vibration-Meter-Using-LM3915
Overview

A vibration monitoring system using a piezoelectric sensor and LM3915 LED driver IC. The system converts mechanical vibrations into electrical signals and displays vibration intensity through a 10-level LED bar graph.
__________________________
Components Used
1. LM3915 IC
2. Piezoelectric Transducer
3. LEDs (10)
4. Resistors
5. Capacitors
6. Power Supply 12V and 3.3V
7. Wires for connection
___________________________
Circuit Diagram

<img width="523" height="493" alt="Circuit Diagram" src="https://github.com/user-attachments/assets/28416ccb-9497-41c3-91a7-a33af183560c" />

_____________________________
Detailed Working Principle of The Project Circuit

The circuit uses LM3915 IC. LM3915 is a led driver chip which is capable of supplying steady current to LED and eliminates the need for resistors. The LM3915 is an 18 pin DIP. In which pin 10 pins are dedicated to drive LED's by sinking current from it. The working of this vibration meter circuit starts with Piezo elec-tric transducer detects the vibrations created on any surface it is place. The vibrations it experience will produce a voltage across it. Capacitor C1 and Resistor R2 stabilizes the voltage develop by the transducer. The signal pin 5 of LM3915 takes the input voltage from the piezo electric transducer and feed it to the inverting terminal of the comparator that is within the IC LM3915. The high reference voltage is fixed to 1.25V which is the internal ref-erence voltage of LM3915. This is because piezo electric trans-ducer is unlikely to develop higher voltage levels and 0 to 1.25V will give us a good working range to detect vibrations. Pin 8 is used to change the reference voltage. Here we do not intend to use this pin, so it is connected to ground and reference voltage remains the same 1.25V. We can change the reference voltage by keeping a voltage divider circuit to pin 8. When the voltage developed across piezo electric transducer is greater than voltage that is fixed at non inverting pins of internal comparators. The output of the comparator goes low, this will allow to sink the current from LEDs into the output pins. And therefore the LEDs light up. The Iring up sequence goes from pin 1, 18, 17, ...pin 10 a 4/10 je across the piezo goes up. This in turn will make the court to operate as a vibration meter that progres-sively lights up LED's as vibration intensity goes up. The step voltage to light up each LED's from pin 1, 18,17...10 is given in the below table-

<img width="530" height="230" alt="Table" src="https://github.com/user-attachments/assets/29e6243c-344b-4a22-9ee5-22c77317ca45" />

As stated earlier LM3915 led driver chip delivers steady current through the LED's. Also it provides the option to fix the amount of current that it draws. In LM3915 IC the current delivered to LED's is equal to 10 times the current from reference out pin (i.e. Pin 7). To calculate the current out from the reference out we have used a 625 ohm resistor in series to it. We know that the voltage at reference out pin is 1.25V. So we can calculate cur-rent by using ohms law. Current Voltage/Resistance ST
1-1.25/625
= 2mA current.
It means the current through 625 ohm resistor is 2mA. Therefore current through LED's will be 10 times that of ohm res current through 625 ohm. It means LM3915 will deliver 10*2 mA or 20mA current to LED's. It is equal to 20mA current.
________________________________________
Project Picture

<img width="346" height="412" alt="Project Picture" src="https://github.com/user-attachments/assets/5f5857e2-026f-4cb2-aefb-3163975dc0fc" />
_______________________________________________
IC Data Sheet and Pin Diagram

<img width="532" height="492" alt="IC LM3915" src="https://github.com/user-attachments/assets/f830d2e3-5176-4b1e-9d65-03dac8f5dd07" />

The circuit uses LM3915 IC. LM3915 is a LED Driver Chip which is capable of supplying steady current to LED and eliminates the need for resistors. The LM3915 is an 18 pin DIP in which10 pins are dedicated to drive LED's by sinking current from it. Pin 5 is the actual signal input pin through which it will take analog input voltage from sensors or other signal source. This input voltage is fed to terminals of series of comparators. And this will be compared to the voltage at non-inverting terminals which is fixed using voltage dividers made using different value of resistors. Pin 4 is RLO pin (signal low level), it is used to set the lower limit of the input signal level at pin 5. Here we connect it to ground which tells that any voltage which is greater than OV should fall within acceptable range. Pin 6 is RHI is signal high level, it is used to set the higher limit of the input signal level. LM3915 has been wired to have a internal reference voltage of 1.25V. This reference voltage will be useful to determine the step size at which each LED from pin 1 to pin 18 will be activated. The step size is given by means of -30dB to OdB. We can change the reference voltage applied to pin 8 by using a resistor voltage divider at pin 8. If we intend to use The same internal voltage reference we can connect this pin to ground.

Specifications:

1. Analog LED Driver IC With Logarithmic output
2. LED incremented by one step for every 3dB
3. Monitor upto 30dB using 10 LEDs
4. Number of controllable LEDs: 10
5. Operating Voltage: 3V to 25V
6. Reference Voltage: 1.2V to 12V
7. LED sink current: 1mA to 30mA (programmable)
8. Both Dot/Bar mode available
9. Available in 18-pin DIP, PLCC package 7/10
__________________________________
Sensor Details

Construction:

A piezo transducer consists of a piezoelectric material, usually a ceramic or crystal, sandwiched between two electrodes. When voltage is applied across the electrodes, the piezoelectric material changes shape, produc-ing mechanical vibrations or acoustic waves, which can be used for vari-ous purposes like generating sound or measuring pressure. This con-struction allows for efficient conversion between electrical and mechani-cal energy.

<img width="370" height="237" alt="Piezo Electric Transducer" src="https://github.com/user-attachments/assets/00689b22-0d3b-4a14-949d-8060772216b8" />

Description:

A piezo transducer is a type of electronic component that converts elec-trical energy into mechanical vibrations or acoustic waves, and vice versa. It typically comprises a piezoelectric material, often a ceramic or crystal, positioned between two electrodes. When an electric voltage is applied to the electrodes, the piezoelectric material undergoes deforma-tion, causing it to expand or contract. This deformation generates me-chanical vibrations or acoustic waves that can be utilized for functions such as generating sound, detecting pressure changes, or producing precise movements in various devices and applications. Piezo transduc-ers are valued for their efficiency, reliability, and versatility in transform-ing energy between electrical and mechanical forms.

Piezo Element (35mm) Data Sheet

<img width="520" height="346" alt="Piezo Element Data Sheet" src="https://github.com/user-attachments/assets/c70a4192-07e8-40bf-ba90-4ca0f28fd366" />
___________________________________
Practical Applications

Vibration meter is used in manufacturing for machine condition monitoring, product testing and quality assurance. Many ma-chine maintenance technicians use vibration meter devices in tandem with sound level meters to analyze frequency. A vibra-tion meter also can be used in civil ngineering to measure the vibration of structures such as buildings, roads, bridges, railway tracks, airport quarries and other heavy industrial areas. Along with this building experiences vibration due to natural causes such as wind, weather, earthquakes, or internal components like elevator, ventilation and HVAC systems. Thus, vibration testing helps to identify building areas that are at higher risk due to vibration. In addition, specialized vibration meter devices can be used to measure the vibration of the human body. Any vibration meter will measure one or more of the following parameters: vibration acceleration, vibration velocity (speed) and/or vibra-tion displacement.
