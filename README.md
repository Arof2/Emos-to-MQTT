# EMUS to MQTT
 Transfers Data from EMUS BMS to MQTT

- Emus https://emusbms.com/
- Mqtt https://mqtt.org/

This Project intends to receive data about the Battery from the EMUS BMS via can and publish it as MQTT topics for homeautomation or similar things.

It is a fork of Jojo-A's outstanding project: https://github.com/Jojo-A/MQTT-CAN-Gateway

Specifically, we want to connect the battery to our OpenWB Wallbox (https://github.com/snaptec/openWB), so it is shown in the Interface.
![Speicherkonfiguration](https://drive.google.com/file/d/1NCPgrapo3fchzq4CyDbatXIcZFaGIkxg/view?usp=share_link)

Until now, connection to the MCP2515 CAN Bus module works and the mqtt broker (builtin OpenWB) is also reached.
The MCP2515 module (https://www.azdelivery.de/products/mcp2515-can-bus-modul) works and retrieves the CAN messages from the BMS.

Next task is to sort out which information was provided from the BMS and send request messages to also get the information not provided regulary by the BMS.
