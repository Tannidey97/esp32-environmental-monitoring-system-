# Day-2-(26-9-2026)

From the day when I bought the hardwares for the project to till now I have been trying to understand every component thoroughly to got the answer of a question which is why am I using this and how it will actually work. To be honest some AI like cluade chatgpt helped me in the case of understanding and find the sources 
which can really help me in my research.

After reading some datasheets of Espressif and finding answers of thousand confusions I got a little knowledge about the ESP-32 circuit board. At first when I saw it for the first time I felt like is the mystery of this board will ever be solvable by me? But I feel a little confident about the concept of this circuit board now. 
According to the official datasheets from Espressif, my esp-32 is not the real official one. I found so many mismatch with the original version. Initially, I thought the circuit board I bought is the official ESP32-DevKitC from Espressif, but eventually I realized I bought the clone version of ESP32 DevKit V1. So my actual board is basically 
ESP32 DevKit V1 (30-pin, DOIT-style generic clone, CH340C USB-UART chip).  

## The photo of the original board that I bought :  
https://github.com/Tannidey97/esp32-environmental-monitoring-system-/blob/main/IMG_20260926_231238_590.jpg

**Through datasheets I got to know about the every individual component on the board such as the ESP-32 microcontroller, pin headers, USB-to-UART bridge chip, AMS1117 voltage regulator, EN button and Boot button.**  

### The ESP-32 module or the main component(microcontroller)  

In one word this is the brain of the whole circuit board which is shielded by a square shaped steel on the board. It works using thousand of transistors, does a specific task repeatedly based on what code is written on it. We can say this is the simplest form of Laptop/Computer. It can run a code, it has a memory also it can catch radio frequency.  

The other components around it supports this to do it's job. Components like___  

***The 8-pin chip labeled "CH340C"***

This is the USB-to-UART bridge chip. It converts USB data from your computer into the serial format the ESP32 understands, and vice versa.

***The 3-pin component labeled "1117 3.3V"***     

This is the **AMS1117** voltage regulator. Its job: take the incoming 5V from USB (or VIN) and step it down to a stable 3.3V, since the ESP32 chip requires 3.3V to operate safely.  

***Two push buttons(EN & Boot)***

**Boot Button -**  used to put the board into "Firmware Download mode." You hold this button down, then briefly press EN, to manually force the board to accept new code being uploaded via serial.

**EN Button —** this is the reset button (EN = "Enable"). Pressing it restarts the chip.  

***I/O Connector*** 

the pin headers where most of the ESP32's pins are broken out, so you can use functions like PWM, ADC (analog input), DAC (analog output), I2C, I2S, and SPI (these are all communication protocols/features for connecting sensors and peripherals).  


**The others components are resistors, capacitors, PWR to check power supply etc.**  


