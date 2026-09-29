# Day-4-(28-9-2026)

As the part of the project I found an opportunity to know about an electronic tool called **sensor**. Honestly I hadn't any idea about sensor before. It was totally mystery to me that how a hardware can sense.
But now I got a little but the main idea of how a sensor actually works, in other words actually what physics works in this case.  

### what I understood about sensors?  

Whatever I felt about sensors is, sensor is an electrical tool that works through some laws of physics. For the example, resistor's resistance changes with the changing of temperature. If the temperature increases, resistance also increases with the temperature and if the temperature decreases, resistance also decreases. So basically we can say a hardware called resistor can sense temperature. All the sensors that has discovered till now like sound sensor, motion sensor etc. works using this types of relationship of physics.  

## DHT22 Sensor 

Since the goal of my project is to know the environmental condition such as temperature, humidity of the surrounding, I needed to be introduced with a sensor called **DHT22**. Through the official datasheet by **Aosong Electronics Co.,Ltd**
I got to know that **DHT22** also named as **AM2302** and inside it there are a capacitor and a resistor. The capacitor has a humidity sensitive dielectric between the two capacitor plate which changes with the changing of humidity around it and causes changing in capacitance of the capacitor. This changing capacitance causes changing in voltage across the capacitor. While the thermistor changes it's resistance with the changing temperature which causes voltage change across it. So basically there are two types of voltage changes happens inside the sensor which are catched by the 8-pin chip microcontroller. Microcontroller takes the analog type data information of temperature change and humidity change as the form of voltage and convert it into digital bits **0** and **1** based on time.  

#### The MCU and DHT22 Communication 

At first **MCU** sends a low voltage signal to the **DHT22** and keep it for 1ms to awake it and ask for data. Then wait for **20-40us** to get response from **DHT22**. When **DHT22** detect the start signal, **DHT22** will send out low-voltage-level signal and this signal last 80us as response signal, then program of **DHT22** transform data-bus's voltage level from low to high level and last **80us** for **DHT22's** preparation to send data. When **DHT22** is sending data to **MCU**, every bit's transmission begin with low-voltage-level that last 50us, the following high-voltage-level signal's length decide the bit is **"1"** or **"0"**.













