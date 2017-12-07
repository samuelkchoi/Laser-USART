# Laser USART
This final project for CS122A at UCR was programmed in C with Atmel Studio 7.0.  

### Major Components
  * **2 x ATmega1284:** *Microcontrollers to communicate with via USART.*
  * **Schmitt Trigger (2N3904 Transistor):** *A Schmitt Trigger is a comparator circuit that acts as a switch. This is a circuit ideal in applications where noisy input signals are present but the output needs to be a clean square wave. The input signal is compared to a reference voltage thus creating a threshold that the input must achieve in order to trigger the circuit. In the case of Laser USART communication, the output signal has a value of 5V when high and 0V when low. By using the CMOS Inverter below, we can invert the signal to be 0V when high and 5V when low. When the laser hits the photoresistor in the Schmitt Trigger circuit, it varies the resistance in the voltage divider and allows the input voltage to surpass the threshold thus activating the switch. This circuit is shown below.* 
  ![schmitt](https://user-images.githubusercontent.com/9040611/33705611-d537e2a2-dae5-11e7-8a60-93f6f63c9f89.jpg)
  * **CMOS Inverter:** *As mentioned above, typical USART signals are pulled low (0V) when data is being transmitted. To prevent the laser diode from burning out, this circuit inverts the signal so that when data is being transmitted, the signal is being pulled high (5V). When the signal is high, the laser is activated and hits the photoresistor in the Schmitt Trigger circuit. This circuit is shown below.*
  ![cmos](https://user-images.githubusercontent.com/9040611/33705663-093cde2c-dae6-11e7-9753-11be53aa5a84.jpg)
  * **650nm 5V Laser Dot Diode & GM5539 Photoresistor** *Laser and Photoresistor used as transmitter and receiver respectively.*
  
### Project Description
   * *Lorem Ipsum*
###### Original Work Statement
*I acknowlegde all content contained herin, excluding template or example code, is my own original work.*
