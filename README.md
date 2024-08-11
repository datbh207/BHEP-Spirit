
# Title

This is the code of the `Spirit` device from the [BHEP](https://github.com/datbh207/BHEP-Demo) project. Spirit is a device used to measure health by monitoring the following 3 indicators:
- Temperature
- Blood Oxygen
- Heart Rate

## Device

- `0.96inch OLED`: Display Health parameters measured from the sensors
- `ESP32`: Process the data then create a connection address between ESP32 and Phone and send the data.
- `GY-906 MLX90614ESF`: Temperature sensor
- `MAX30102`: Heart Rate and Blood Oxygen Sensor
- `BRC 18650 6800mAh`: Supply 3.7V
- `MT3608 2A`: The booster circuit increases 3.7V to 5V to provide enough power for the circuit.

Complete Device:
![Spirit](https://github.com/user-attachments/assets/3dbfccd0-d7bc-4586-b1fd-a1268e45668b)

## Library
- [Wire.h](https://www.arduino.cc/reference/en/language/functions/communication/wire/): Allows to communicate with I2C devices.
- [WiFiManager.h](https://www.arduino.cc/reference/en/libraries/wifimanager/): Library for configuring ESP8266/ESP32 modules WiFi credentials and custom parameters at runtime with captive portal.
- [FirebaseESP32.h](https://reference.arduino.cc/reference/en/libraries/firebase-arduino-client-library-for-esp8266-and-esp32/): Google Firebase Arduino Client Library for Espressif ESP8266 and ESP32.
- [MAX30105.h](https://www.arduino.cc/reference/en/libraries/sparkfun-max3010x-pulse-and-proximity-sensor-library/): Library for MAX30105 heart rate and blood oxygen sensor.
- [heartRate.h](https://projecthub.arduino.cc/SurtrTech/measure-heart-rate-and-spo2-with-max30102-eb4f74): Library or algorithm for calculating heart rate.
