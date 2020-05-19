# IR Translator
A system which recieves IR transmissions, decodes them, re-interprets them, and then relays the translation.
### Using Arduino, the infrared transceiver will enable:
- [ ] Universal Remote-like features
- [ ] Advanced macros & IR control routines
- [ ] [Consumer IR functions](https://en.wikipedia.org/wiki/Consumer_IR)
## System:
#### Microprocessor dev board
Based on the ATtiny85, the [Adafruit Trinket](https://www.adafruit.com/product/1500) fits the needs perfectly. The Trinket has reached end of life, *and is inexpesive,* due to its usage of "bit-bang USB". This usage is not an issue in our deployment.
The 3.3V version was selected as if 5V was ever needed it could be aquired easily off usb.
#### IR Reciever
Most TV IR is tuned to a 38khz carrier frequency and is on the 930-950nm wavelength. The TSOP58238-ND was selected as adequate and due to it being inexpensive at the time of purchase.
#### IR LED
The IR LED was selected to be on the 930-950nm wavelength as the carrier frequency would be reproduced in code. The OED-EL-8L was selected due to it being inexpensive at the time.
#### Other Parts
- A couple kilo ohm resistor is needed to reduce power to led. 
- A switch will be used to toggle power to the device. 
  - *(these can easily be harvested from other old electronic devices.)*
- A Powersupply ranging from 5v to 12v
  -  *(the Trinket has a battery input)*
