# EMUS to MQTT
 Transfers Data from EMUS BMS to MQTT

- Emus https://emusbms.com/
- Mqtt https://mqtt.org/

This Project intends to receive data about the Battery from the EMUS BMS via can and publish it as MQTT topics for homeautomation or similar things.

Specifically, we want to connect the battery to our OpenWB Wallbox (https://github.com/snaptec/openWB), so it is shown in the Interface.
![Speicherkonfiguration](https://drive.google.com/file/d/1NCPgrapo3fchzq4CyDbatXIcZFaGIkxg/view?usp=share_link)

Until now, connection to the MCP2515 CAN Bus module works and the mqtt broker (builtin OpenWB) is also reached.

Next task will be to connect to EMUS BMS and try to extract the data.

