CC-mega328 Breakout Board
========================================

![CC-mega328 Breakout](mdContents/cc-mega328_1.png)  
The CC-mega328 Breakout Board is breakout for the Atmel ATMEGA328P with prototyping area.  
This board shape is dirfferent from Arduino UNO, but it has Arduino Uno V3 style headers.  
There are only the minimal set of parts for running microcontroller. When you make your own circuit boards, this board might be helpful.

### Some highlights of the CC-mega328 Breakout Board:
 1. Main core: [ATMEGA328P](http://www.atmel.com/devices/atmega328p.aspx)
 2. Volatage regulator can be mounted in the extra prototyping area.
 3. Prototyping area 43.94mm(1730mil) x 53.34mm(2100mil)
 4. Measures 99.82mm(3930mil) x 53.34mm(2100mil)


Repository Contents
-------------------
* **/Hardware** - All Eagle design files (.brd, .sch)


Description(Pin Interfaces)
-------------------
![TopView](mdContents/cc-mega328_2.png)

### CN1 Pin Descriptions:
This connector is for Flashing a program microcontroller.  
If you change BOOT MODE, To be selected BOOT MODE before connecting the power supply.  
And also, you can Communicate with ATMEGA328P using "Serial" function.
- **VCC:** Restrictly 5.0VDC or 3.3VDC
- **TX:** PD1 used as UART TX.
- **RX:** PD0 used as UART RX.
- **GND:** GND.
- **RESET:** Reset input to microcontroller.
- **EN:** Connected to 3-stete-buffer gate pin H:Enable RESET input L:Disable RESET input(normally)

If you are interested in more useful uart module, please see the [General Serial Communication Board](https://github.com/NaoNaoMe/General-Serial-Communication-Board).

### CN2 Pin Descriptions:
This connector is as power supply.
You can mount a voltage regulator in the extra prototyping area near the connector.
- **VIN:** Depending on the voltage regulator requirements.
- **GND:** GND.


How to burn bootloader and upload sketch
-------------------
See [this page](BurnBootloader.md)


License
-------------------
The repository is released under [Creative Commons ShareAlike 4.0 International](https://creativecommons.org/licenses/by-sa/4.0/).

Distributed as-is; no warranty is given.
