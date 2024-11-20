![image](https://github.com/user-attachments/assets/9d98dc86-e902-4664-aeb9-d621c2f77926)
# Title

This is the code of the `Spirit` device from the [BHEP](https://github.com/datbh207/BHEP)  project. Spirit is a device used to measure health by monitoring the following 3 indicators:
- Temperature
- Blood Oxygen
- Heart Rate

## Device

- `0.96inch OLED`: Display Health parameters measured from the sensors
  ![image](https://github.com/user-attachments/assets/5bbddf2a-a5a7-4b26-9df7-10943144e649)

- `ESP32`: Process the data then create a connection address between ESP32 and Phone and send the data.
  ![image](https://github.com/user-attachments/assets/a6109ad9-a4d3-45f3-bb05-b760ac6c1d9d)

- `GY-906 MLX90614ESF`: Temperature sensor
  ![image](https://github.com/user-attachments/assets/3cd324be-af16-4b5c-9cd7-cd037c328611)

- `MAX30102`: Heart Rate and Blood Oxygen Sensor
  ![image](https://github.com/user-attachments/assets/5c24ea5a-cb95-42e7-b281-2fff0d7f182e)

- `BRC 18650 6800mAh`: Supply 3.7V
  ![image](https://github.com/user-attachments/assets/f28c92c3-b63f-4355-a90a-63af631d4643)

- `MT3608 2A`: The booster circuit increases 3.7V to 5V to provide enough power for the circuit.
  ![image](https://github.com/user-attachments/assets/c792bf61-ce79-466c-b2d0-ca5a56956550)

Complete Device:
![Spirit](Image/Spirit.jpg)

## Library
- [Wire.h](https://www.arduino.cc/reference/en/language/functions/communication/wire/): Allows to communicate with I2C devices.
- [WiFiManager.h](https://www.arduino.cc/reference/en/libraries/wifimanager/): Library for configuring ESP8266/ESP32 modules WiFi credentials and custom parameters at runtime with captive portal.
- [FirebaseESP32.h](https://reference.arduino.cc/reference/en/libraries/firebase-arduino-client-library-for-esp8266-and-esp32/): Google Firebase Arduino Client Library for Espressif ESP8266 and ESP32.
- [MAX30105.h](https://www.arduino.cc/reference/en/libraries/sparkfun-max3010x-pulse-and-proximity-sensor-library/): Library for MAX30105 heart rate and blood oxygen sensor.
- [heartRate.h](https://projecthub.arduino.cc/SurtrTech/measure-heart-rate-and-spo2-with-max30102-eb4f74): Library or algorithm for calculating heart rate.
