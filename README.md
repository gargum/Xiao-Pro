# Xiao-Pro
A Xiao to Pro Micro conversion board

# Features
- Solder jumpers allow this board to be reversible
- Compatible with several versions of the Xiao microcontroller
- Reset pins connected to a reset button
- Broken out battery contacts
- Broken out NFC contacts
- Switch (SPDT) connecting the batteries to the Xiao's on-board battery charger
- Broken out contacts one can use to wire the output of a TP4056 instead of using the on-board battery charger
- All 6 SWD pins broken out

# Pinout Conversion
| Xiao  | Pro Micro |
| A0  | P21 |
| A1  | P20 |
| A2  | P19 |
| A3  | P18 |
| A4  | SDA |
| A5  | SCL |
| A6  | TX  |
| A7  | RX  |
| A8  | P6  |
| A9  | P5  |
| A10 | P4  |
| GND | GND |
| 3V3 | VCC |
| 5V  | RAW |

# Notes
- Only 2 of 3 GND pins are connected, hence why there are solder jumpers to bridge these pins.
- Although SPI technically is connected, it occupies P4, P5, and P6 just below the I2C pins.
- A TP4056 is bigger than this board, and therefore cannot be used as a shield for it.
- All SMD pads are slightly undersized. Doing this was necessary in order to connect everything.
- This board is too small to be ordered individually, and instead must be ordered as a sheet.

# How to Build/Buy
In this repository, there should be a ZIP file. This contains all of the gerber files necessary to order this PCB through PCBWay or JLCPCB.
If one wishes to see what exactly is inside that ZIP file, a folder with all of its contents is also contained in this repository.
If one wishes to modify this project, all Kicad project files are included in this repository.
