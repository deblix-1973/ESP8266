# ESP8266_PN532_RFID
## PN532 RFID Card Reader with status LED
 ![ESP8266_PN532_RGB_LED](https://github.com/user-attachments/assets/2d58c870-f208-4522-9f30-01b68ebd8101)
## How To

### Step 1
Flash your ESP8266 with tasmota-sensor.bin. Reboot and connect to your Wifi.
### Step 2
Open the Web UI and go to Configuration > Module > Generic(18)

RX GPIO3	LedLink\
D2 GPIO4	PN532 Rx\
D1 GPIO5	PN532 Tx\
D6 GPIO12	Relay1\
D7 GPIO13	Relay2\
D5 GPIO14	Relay3\
and save your configuration.
### Step 3
In the Web UI got to Configuration > MQTT and set up MQTT.\
done!\
You can now communicate with your ESP8266 via MQTT and get Card IDs (UID) from your PN532.
