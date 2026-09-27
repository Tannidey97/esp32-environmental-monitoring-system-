# Day-3-(27/9/2026)

During exploring ESP-32 I felt like after the microcontroller one of the important part of the board are pin headers. Honestly it was the hardest part to know each pin properly since still I hasn't started practical uses of these pins. Maybe when I will finally 
start to use those pins I will be more cleared up. From the official datasheets and with the help of AI I got to know the meaning of some names such as **GPIO**, **DAC**, **A#**, **TX0**, **RX0**, **SPI**,**SDA**, **T#**, **VIN**, **D#**, **I2C**, **I2S**etc. At the beginning, these names were 
seeming like super strange but now after knowing about these, it feels more easier to understand.  

## Brief explanation of each one :

***GPIO-*** It stands for General Purpose of Input or Output. A GPIO pin like a basic on/off switch or sensor wire that code controls. The number after it (GPIO13, GPIO14, GPIO27, etc.) is just an ID label. Basically it does two general job 
turn something on/off or read whether something on/off.  

***DAC-*** DAC is digital to analog converter. These pins can output an analog voltage.  

***ADC-*** This is opposite of DAC. Converts an analog voltage into digital voltage signal like a varying signal from sensors, so that the ESP-32 microcontroller can read and process.  

***T#-*** = T1, T2, T3... = this pin can act as a touch sensor — can detect finger touching a wire, no button needed.  

***I2S (Inter-IC Sound) —*** a protocol specifically designed for transmitting digital audio data, commonly used to connect microphones, speakers, or audio codecs.    

***I2C (Inter-Integrated Circuit) —*** a communication protocol that lets multiple devices talk to the microcontroller using just 2 wires (SDA for data, SCL for clock).  

***VIN —*** lets you power the board from an external power source (like a battery) instead of USB.  

***TX0(Transmit) —*** sends data OUT from the ESP-32.  

***RX0 (Receive) —*** receives data IN to the ESP-32.  
[specifically, these two are the same wires that talk to the computer through the USB cable.]  

**So basically we can say there are three types of pins in the board some uses for power supply, some are for communicate to other devices and some are for input/output.  






