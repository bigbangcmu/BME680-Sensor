https://github.com/bigbangcmu/bigbang/blob/bigbangcmu/BME680%20Sensor/%5B%20Multi%20%5D%20-%20BME680%20Sensor.jpg?raw=true

# BME680-Sensor
**The BME680 Sensor** is a compact 4-in-1 environmental sensor capable of measuring temperature, humidity, air pressure, and air quality (gas). It is ideal for weather and air quality monitoring applications, offering low power consumption and reliable performance. The sensor communicates with microcontrollers such as Arduino, ESP8266, and ESP32 via the I²C interface and operates on a supply voltage of 3.3–5 V.

## This sensor is suitable for:
- Air quality monitors and weather stations
- Smartwatches and wearable devices
- Fitness and health tracking, HVAC systems, and smart home solutions
- Indoor navigation and GPS enhancement

## Specifications
|Parameter|Value|
|-|-|
|**Model**| BME680|
|**Temperature**|-40 to +85°C|
|**Humidity**|0–100% RH|
|**Humidity Accuracy**|±3% RH|
|**Pressure**|300–1,100 hPa|
|**Pressure Accuracy**|±0.12 hPa (±1 m altitude)|
|**Average Current**|2.1–3.7 µA @ 1Hz|
|**Interface**|I²C / SPI|

![Description](https://github.com/bigbangcmu/bigbang/blob/bigbangcmu/Ultrasonic%20Sensor/Example%20code.png?raw=true){{{width="250" height="auto"}}} 
[**Download the working code here**](https://code.gogoboard.org/#/program/6998fe0c-6609-4efa-aaa4-e1605b7e0e9a)

## Block Code Reference
|![](https://github.com/bigbangcmu/bigbang/blob/bigbangcmu/Gas/BME680%20code%207.png?raw=true){{{width="210" height="auto"}}}| Use this block to read the dew point from the sensor in degrees Celsius (°C).|
|-|-|
|![](https://github.com/bigbangcmu/bigbang/blob/bigbangcmu/Gas/BME680%20code%204.png?raw=true){{{width="210" height="auto"}}}|**Use this block to read the ambient temperature from the sensor in degrees Celsius (°C).**|
|![](https://github.com/bigbangcmu/bigbang/blob/bigbangcmu/Gas/BME680%20code%206.png?raw=true){{{width="200" height="auto"}}}|**Use this block to read the relative humidity from the sensor in percent (%).**|
|![](https://github.com/bigbangcmu/bigbang/blob/bigbangcmu/Gas/BME680%20code%205.png?raw=true){{{width="200" height="auto"}}}|**Use this block to read the air pressure from the sensor in hectopascals (hPa).**|
|![](https://github.com/bigbangcmu/bigbang/blob/bigbangcmu/Gas/BME680%20code%208.png?raw=true){{{width="190" height="auto"}}}|**Use this block to read the gas resistance from the sensor in kilohms (kΩ), which is used to estimate indoor air quality.**|

## **Required Equipment**
|BME680 Sensor|![Description](https://github.com/bigbangcmu/bigbang/blob/bigbangcmu/Gas/gas%20sensor.png?raw=true){{{width="200" height="auto"}}}|
|-|-|
|**Grove cable**|![Description](https://github.com/bigbangcmu/bigbang/blob/bigbangcmu/Ultrasonic%20Sensor/only%20grove%20(test).png?raw=true){{{width="200" height="auto"}}}|
|**Computer or Tablet**|![Description](https://github.com/bigbangcmu/bigbang/blob/bigbangcmu/Ultrasonic%20Sensor/computer%20or%20tablet.png?raw=true){{{width="200" height="auto"}}}|
|**GoGo Board and USB-C cable**|![Description](https://github.com/bigbangcmu/bigbang/blob/bigbangcmu/Ultrasonic%20Sensor/gogoboard%20and%20usb.png?raw=true){{{width="200" height="auto"}}}|

## **How to use**
**1. Connect the GoGo Board**
- Connect the GoGo Board to your computer or tablet via USB-C cable or Wi-Fi
![](https://github.com/thegogoboard/gogodoc/blob/main/Automation/Image%20(91).jpg?raw=true){{{width="500" height="auto"}}}

**2. Connect the  Sensor**
There are two ways to connect the Gas sensor:
**Option 1:** Using a Grove Connector
- Connect the Gas Sensor to a Grove cable, then plug the cable into the purple Multi Port on the GoGo Board.

|![](https://github.com/bigbangcmu/bigbang/blob/bigbangcmu/Gas/BME680.gif?raw=true){{{width="500" height="auto"}}}|![](https://github.com/bigbangcmu/bigbang/blob/bigbangcmu/Gas/gas%20with%20board.png?raw=true){{{width="500" height="auto"}}}|
|-|-|

**Option 2:** Using Jumper Wires (Dupont Wires)
- If you don’t have a Grove connector, you can use jumper wires to connect the sensor directly to the pins on the GoGo Board.

## Getting Started with the BME680 Sensor on GoGo Code 

**1. Visit the GoGo Code website:**
- Go to [GoGo Code](https://code.gogoboard.org/#/program) to start programming and controlling your device.

**2. Add the Air Pressure Sensor extension:**
- Click on the **Add Extension** category

![](https://github.com/bigbangcmu/bigbang/blob/bigbangcmu/Gas/BME680%20code%201.gif?raw=true){{{width="1000" height="auto"}}}

- Select **Official**, then click the **[Multi] - BME680 Sensor** card. The system will automatically return to the main page.

![](https://github.com/bigbangcmu/bigbang/blob/bigbangcmu/Gas/BME680%20code%202.gif?raw=true){{{width="1000" height="auto"}}}

**3. Add sensor command blocks:**
- Click on the **[Multi] - BME680 Sensor** category. You will see five available blocks:

![](https://github.com/bigbangcmu/bigbang/blob/bigbangcmu/Gas/BME680%20code%203.gif?raw=true){{{width="1000" height="auto"}}}

**4. Write a simple program to display sensor data:**
- Use the show number block from the **Built-in Display** category and place it inside the start block.
- Insert the **"Gas of BME680 (kΩ)"** block into the show number block.
- To display the value continuously, place everything inside the **“forever do each time wait…”** block from the **Loops** category. You can also set how often the value is updated (e.g., every 1 second).

![](https://github.com/bigbangcmu/bigbang/blob/bigbangcmu/Gas/BME680%20code%209.png?raw=true){{{width="500" height="auto"}}}

**5. Download and test your code:**
- Click **Download**, then click **Run Code** to start running your program

![](https://github.com/bigbangcmu/bigbang/blob/bigbangcmu/Gas/BME680%20code%2010.gif?raw=true){{{width="1000" height="auto"}}}

::: details Additional information
  **Buy online:** [BME680 Sensor ](https://www.arduitronics.com/product/6156/bme680-sensor-arduino-arduino-esp8266-esp32)
  
  **Cautions**
- Avoid modifying wires or connecting them incorrectly, as this may damage the device.
- Do not touch the sensor head while it is operating, as it may affect detection accuracy.
- If the sensor does not work, check the voltage and wiring connections.
:::
