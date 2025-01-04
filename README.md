### NAME:Vishvanandh N
### REG NO:24005857

# Experiment:2 -CONTROL RELAY USING IOT CONTROLLER
##  AIM:
To control the Relay using Arduino controller

## Software required:
Arduino IDE </br>
Proteus

## PROCEDURE:
### Arduino IDE
Step1:Open the Arduino IDE </br>
Step2: Go to file and select new file option </br>
Step3:Type the program </br>
Step4:Go to file and select save option to save the program </br>
Step5:Go to sketch and select verify or compile options </br>
Step6:If no error Hex file will be generated in the temporary folder </br>

### Proteus
Step7:Open the Proteus software </br>
Step8:Go to file select new design and click ok button </br>
Step9:Select component mode and click pick devices from the library </br>
Step10:Type the component name in the keyword to select the components and click ok button </br>
Step11:Design the circuit as per the diagram </br>
Step12:Double click the Arduino controller and upload the hex file generated by Arduino IDE </br>
Step13:Click start button and check the output

## THEORY:
LED Blinking is a very common and almost first program for every embedded learner or beginner. In which we blink an LED with having some delay. So today we are here with the same project but here we will use an AC bulb instead of normal LED and will blink an AC bulb.Whenever we need to connect any AC Appliance in our embedded circuits, we use a Relay. So in this arduino relay control tutorial we will simply learn How to interface a Relay with Arduino. Here we are not using any Relay Driver IC like ULN2003 and will only use an NPN transistor to control relay.
Relay is an electromagnetic switch, which is controlled by small current, and used to switch ON and OFF relatively much larger current. Means by applying small current we can switch ON the relay which allows much larger current to flow. A relay is a good example of controlling the AC (alternate current) devices, using a much smaller DC current.  Commonly used Relay is Single Pole Double Throw (SPDT) Relay, it has five terminals as below

<img src="https://github.com/anishkumar-Embedded/Control-of-Relay-Using-IoT-controller/assets/71547910/7883ec9f-4adc-4033-9acf-f16809fd73eb" width="600" height="500"/>

When there is no voltage applied to the coil, COM (common) is connected to NC (normally closed contact). When there is some voltage applied to the coil, the electromagnetic field produced, which attracts the Armature (lever connected to spring), and COM and NO (normally open contact) gets connected, which allow a larger current to flow. Relays are available in many ratings, here we used 6V operating voltage relay, which allows 7A-250VAC current to flow.The relay is always configured by using a small Driver circuit which consists a Transistor, Diode and a resistor. Transistor is used to amplify the current so that full current (from the DC source – 9v battery) can flow through a coil to fully energies it. The resistor is used to provide biasing to the transistor. And Diode is used to prevent reverse current flow, when the transistor is switched OFF. Every Inductor coil produces equal and opposite EMF when switched OFF suddenly, this may cause permanent damage to components, so Diode must be used to prevent reverse current.Here to turn on the Relay with Arduino we just need to make that Arduino Pin High (A0 in our case) where Relay module is connected

<img src="https://github.com/anishkumar-Embedded/Control-of-Relay-Using-IoT-controller/assets/71547910/208c5221-8e60-4880-a5c8-cae317d7f211" width="600" height="500"/>

In this Arduino  Relay Control Circuit we have used Arduino to control the relay via a BC547 transistor. We have connected transistor base to Arduino pin A0 through a 1k resistor. An AC bulb is used for demonstration.Working is simple, we need to make the RELAY Pin (PIN A0) high to make the Relay module ON and make the RELAY pin low to turn off the Relay Module. The AC light will also turn on and off according to Relay.

## PROGRAM:
<img src="https://github.com/user-attachments/assets/ecd38424-54bb-4590-b2ea-a43625f08233" width="600" height="500"/>

## CIRCUIT DIAGRAM:
<img src="https://github.com/user-attachments/assets/a6dd1746-d5f2-4810-a84e-0150661022b8" width="600" height="500"/>

## OUTPUT:
### Lamp off:

<img src="https://github.com/user-attachments/assets/6ecde2d5-53af-43f2-8d79-26dde0d74973" width="600" height="500"/>

### Lamp on:
<img src="https://github.com/user-attachments/assets/91be19e3-8839-43e7-8cbc-cf5be94e57b6" width="600" height="500"/>

## RESULT:
Thus the relay is controlled using Arduino controller.
