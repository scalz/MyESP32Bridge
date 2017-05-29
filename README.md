# MyESP32Bridge For Mysensors

**MyESP32 Bridge is a fun, rechargeable and versatile board for Mysensors and your home automation.**

<img src="https://raw.githubusercontent.com/scalz/MyESP32Bridge/master/Img/MyESP32Bridge_top_ring.png" alt="MyESP32Bridge top 3d view"> 

<img src="https://raw.githubusercontent.com/scalz/MyESP32Bridge/master/Img/MyESP32Bridge_bottom.png" alt="MyESP32Bridge bottom 3d view"> 

This is a work in progress project.


### The board
------

A year ago, i designed a fun project. This was a rechargeable gesture mote with RGB led ring ATSAM mcu based.
But when ESP32 has been announced, I secretly waited for its release.. I also wanted to improve a bit the concept, and cost by more modularity.

Finally, i知 happy to show you MyESP32 Bridge, not really fancy name though :)

<img src="https://raw.githubusercontent.com/scalz/MyESP32Bridge/master/Img/MyESP32Bridge_top_assembled.jpg" alt="MyESP32Bridge assembled top"> 

<img src="https://raw.githubusercontent.com/scalz/MyESP32Bridge/master/Img/MyESP32Bridge_bottom_assembled.jpg" alt="MyESP32Bridge assembled bottom"> 

For those who don稚 know yet about ESP32, I知 using ESP32-WROOM which is 

- **FCC, CE, IC, MIC, KCC, NCC certified module**
- Xtensa dual-core, 32-bit LX6 processor. One core for radio, one core for application firmware
- Wi-Fi: 802.11b/g/n/e/i
- Bluetooth: v4.2 BR/EDR and BLE
- 12-bit SAR ADC up to 18 channels
- 2 ﾗ 8-bit DACs
- 10 ﾗ touch sensors
- Temperature sensor
- 4 ﾗ SPI (but one is used by internal flash memory)
- 2 ﾗ IｲS
- 2 ﾗ IｲC
- 3 ﾗ UART
- 1 SD/SDIO/MMC host
- 1 slave (SDIO/SPI)
- Ethernet MAC interface with dedicated DMA and IEEE 1588 support
- CAN bus 2.0
- IR (TX/RX)
- Motor PWM
- Built in remote peripheral up to eight channels
- Hall effect sensor
- Ultra low power, analog pre-amplifier
- Supports all IEEE 802.11 standard security features, including WFA, WPA/WPA2 and WAPI
- Secure boot
- Flash encryption
- 1024-bit OTP, up to 768-bit for customers
- Cryptographic hardware acceleration: AES, SHA-2, RSA, ECC, random number generator (RNG)


So what is my board capable of ?
- **Serial Gateway**, 
- **Wifi** Gateway, 
- **Bluetooth/BLE** Gateway, 
- **CAN bus** Gateway, 
- **Sniffer with visual feedback**, 
- **IR** blaster, 
- **rechargeable** for example for **backup power**
- can use extension board with **MYSX connector**, so a **development board** too
- and so one, i知 sure i知 missing usecases :)

More detailed specifications:
- **Wifi or Bluetooth/BLE** thanks to ESP32 mcu
- **NRF24 footprint**
- **RFM69/95** footprint
- **NRF24 and RFMs radio can be used at same time**, each one on their distinct SPI Bus, or on same SPI Bus (configurable via smd jumpers)
- **CAN bus with voltage source selection** (3.3 or 5v)
- **Onboard IR emitter and receiver **
- **IR emitter pinheader for a blaster extension** (just needs the diodes, circuit is onboard)
- **USB interface with onboard CP2104** for programming and serial stuff
- **2x onboards RGB Leds** 
- and **2x right angle tactile switches** : Reset and User button
- **Pinheader for connecting a cheap RGB led ring from aliexpress** (12x leds version), saving costs of rgb leds assembly. 
- **Cutoff for RGB leds circuit** by load switch
- **Lipo rechargeable** (decided to use LIPO instead of LifePO4 because of RGB leds voltage levels during battery lifetime) with JST connector
- **Battery voltage sensing**
- Step down converter with filtering for 3.3v
- ESD and load protection for USB
- Auto switch between USB and battery if usb is disconnected for example
- JTAG lines pinheader
- for quick compatibility with Mysensors, and as ESP32 arduino core is in dev, i have added an I2C EEprom for routing table etc, and ATSHA204A for signing
- 3x holes for holding the board in enclosure
- 4x holes for holding the aliexpress 12x RGB leds ring


### Known issues
------ 

### TODO
------
- Upload files, be patient please :)
- etc.

### Donations
------

I'm trying to make opensource projects. I do this for free and sharing spirit. I don't do ads etc..
But if you think information here is worth of some money, or want to reward me, feel free to send any amount through paypal.

[![](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=PWVDL2P64FDVU)  

Or you can also order pcb here :
I will earn a little percentage that will allow me to order others prototypes and share more fun design.

Or pay me a protein smoothie if you see me! oh well, a beer is ok too :)

### Contributors
------
Special thanks to 
- tekka from Mysensors Core Team, for feedbacks and motivating me
- Mysensors Core Team :)
- Adafruit, Sparkfun, TI, Atmel, ESP32 forum etc.. for all educational infos they share


### Links, reference and license 
------
- 

Copyright Scalz (2017). released under the CERN Open Hardware Licence v1.2
