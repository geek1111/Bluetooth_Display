# Bluetooth_Display
It's simple bluetooth display which can read strings sent through bluetooth via android mobile and write it on 20x4 LCD 

This system uses Arduino , Bluetooth HC-05 module & 20x4 LCD.

### Things we need
* Arduino Uno
* HC-05 Bluetooth Module
* 20x4 Liquid Crystal LCD
* some solderless Jumpers ,Breadboard.

### Arduino
* Upload Sketch "Bluetooth_Display.ino" in arduino uno.

### HC-05 Bluetooth Module
* Connect Blutooth module to arduino As shown in Schematic.
* Connect >> +5v Pin To >> Arduino 5v Pin.
* Connect >> GND Pin To >> Arduino GND Pin.
* Conncet >> TX Pin To >> Arduino RX Pin.
* Connect >> RX Pin To >> Arduino TX pin. 
[use Two registers to divide voltage] see Schematic.
* PLEASE NOTE THAT THIS (Voltage division) PROCESSES SHULD BE DONE ANY HOW OR IT WILL DAMAGE BLUETOOTH MODULE.

### 20x4 LCD 
* Connect 20x4 LCD to Arduino As shown in Schematic.
* Connect Pin 1 >> VSS Pin To >> GND
* Connect Pin 2 >> VDD Pin To >> +5V
* Connect Pin 3 >> V0 Pin To >> 10K Variable register
* Connect Pin 4 >> RS Pin To >> Arduino Pin 12
* Connect Pin 5 >> R/W Pin To >> GND
* Connect Pin 6 >> E Pin To >> Arduino Pin 11
* N/C Pin 7 >> DB0 Pin To >> N/C
* N/C Pin 8 >> DB1 Pin To >> N/C
* N/C Pin 9 >> DB2 Pin To >> N/C
* N/C Pin 10 >> DB3 Pin To >> N/C
* Connect Pin 11 >> DB4 Pin To >> Arduino Pin 2
* Connect Pin 12 >> DB5 Pin To >> Arduino Pin 3
* Connect Pin 13 >> DB6 Pin To >> Arduino Pin 4
* Connect Pin 14 >> DB7 Pin To >> Arduino Pin 5
* Connect Pin 15 >> LED+ Pin To >> +5v Through resistor
* Connect Pin 16 >> LED- Pin To >> GND

For Better understanding Please see Schematic.
Please note that schematic is created using Atmega 328-p 
So If you're using arduino you dont need 78xx voltage regulator.
and not even crystal and releted capacitors

