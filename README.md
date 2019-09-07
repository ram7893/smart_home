# smart_home
         Smart Home clearly stands out, ranking as highest Internet of Things application on all measured channels. More than 60,000 people 
currently search for the term “Smart Home” each month. This is not a surprise. The IoT Analytics company database for Smart Home includes 
256 companies and startups. More companies are active in smart home than any other application in the field of IoT. The total amount of 
funding for Smart Home startups currently exceeds $2.5bn. This list includes prominent startup names such as Nest or Alert Me as well as 
a number of multinational corporations like Philips, Haier, or Belkin.

         In this project, we will design our own automation control of home appliances using NodeMCU and relays. The main components required
are:
1. NodeMCU : 
It is an open source IoT platform. It is permanent software programmed into a read only memory which runs on ESP8266 Wi-Fi SoC from 
Expressive systems, and hardware based on ESP12 module.  The features of wifi module ESP8266 are as follows:
Processor: L106 32-bit RISC microprocessor core based on the Tensilica Xtensa
Diamond Standard 106Micro running at 80 MHz†
 Memory:
32 KB instruction RAM
32 KB instruction cache RAM
80 KB user data RAM
16 KB ETS system data RAM
 External QSPI flash: up to 16 MB is supported (512 KB to 4 MB typically included)
 IEEE 802.11 b/g/n Wi-Fi
 Integrated TR switch, balun, LNA, power amplifier and matching network
 WEP or WPA/WPA2 authentication, or open networks
 16 GPIO pins
 SPI
 I²C (software implementation)[5]
 I²S interfaces with DMA (sharing pins with GPIO)
 UART on dedicated pins, plus a transmit-only UART can be enabled on GPIO2
 10-bit ADC (successive approximation ADC)

  The working of the wifi module ESP8266 is as follows, the wifi module can be controlled from your local WiFi network or from the 
internet. The ESP-01 module has GPIO pins that can be programmed to turn an LED or a relay ON/OFF through the internet. The module can 
be programmed using an Arduino/USB-TO-TTL CONVERTER THROUGH THE SERIAL PINS(RX,TX).


2. Relay Module : Here in this project we use 4 channel relay board in order to control 4 different loads in a smart home. this relay module allows you to combine the processing power of arduino to devices
that use high current and voltages. The specifications of the relay board are mentioned below.
 5V relay module
 Max allowable voltage: 250VAC/110V.
 Indication LED for relay status.
 Temperature: -30C TO +85C
 Max allowable current: 10A

3. Serial UART : The USB TTL serial cables are a range of USB to serial converter cables which provide connectivity between USB and 
serial UART interfaces. A range of cables are  available offering connectivity at 5V, 3.3V or user specified signal levels with various 
connector interfaces. 

Hardware Implementation: Node MCU is the heart of the project it consist of 30 pins among them we use D0 to D3 pins and ground pin, these D0 to D3 
pins are connected to the 4 channel relay control port terminals IN1 to IN4, this relay needs 5v supply and 15 to 20 mA driver current so
that we use serial UART to provide 5v supply to the relay board from USB port which is connected to adaptor or computer system. This 
serial UART consists of 6 pins among them we use +5v pin and ground pin for the connection to relay Vcc terminals. Any electrical 
appliances of up to 250v/10A AC and 30v/10A DC are connected to the relay output terminals, each channel consists of 3 output terminals 
the load will be connected in between 2 and 3 terminals. Ground terminals of each component are must be connected together.

Blynk App: In order to communicate with wifi module we need an smart phone installed with Blynk app so that the relay module can be controlled.
Build a basic GUI for NodeMCU using the app.

Integrating with IFTTT : Use the IFTTT app to integrate the voice control (Google Assistant) to the project.


Future Work : We will soon see an updated version of the project.



Note: This project is 3 years old, just uploaded in GitHub.






