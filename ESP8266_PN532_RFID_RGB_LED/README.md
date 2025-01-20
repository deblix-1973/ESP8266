# ESP8266_PN532_RFID
## PN532 RFID Card Reader with status LED
![ESP8266_PN532_RGB_LED_](https://github.com/user-attachments/assets/56326733-48b0-4a3a-93d6-238d36900ec3)
## How To

### Step 1
Flash your ESP8266 with tasmota-sensor.bin. Reboot and connect to your Wifi.
### Step 2
Open the Web UI and go to Configuration > Module > Generic(18)

3.3V   > VCC
GND    > GND
GPIO03 > LedLink (for MQTT Status)\
GPIO04 > PN532 Rx\
GPIO05 > PN532 Tx\
GPIO12 > Relay1 (not relevant here - used for other purpose in my project)\
GPIO13 > Relay2 (not relevant here - used for other purpose in my project)\
GPIO14 > Relay3 (not relevant here - used for other purpose in my project)\
and save your configuration.
### Step 3
In the Web UI go to Configuration > MQTT and set up MQTT.

#### Done!
You can now communicate with your ESP8266 via MQTT and get Card IDs (UID) from your PN532.
#### Config
```{"NAME":"Generic","GPIO":[1,1,1,1,1,1,1,1,1,1,1,1,1,1],"FLAG":0,"BASE":18}```
