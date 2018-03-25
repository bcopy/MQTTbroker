# ESP8266 WebSocket MQTT Broker for IoTmanager

Library for direct connection of IoTmanager'a to ESP8266 through WebSocket without intermediaries, such as cloudmqtt.com. ESP acts as a Wi-Fi access point and serves as an MQTT broker, so you do not need Internet access to communicate with the smartphone.

## Composition

- [MQTTbroker.h] imitation of the broker's work for several clients (with the control of subscriptions)
- [MQTTbroker_lite.h] only for direct communication with IoTmanager (without control of subscriptions)

## Examples

In the library there are several examples of work with both the lite version and the full version. See File -> Examples -> MQTTbroker

## Restrictions

- The broker uses version 3.1.1 of the MQTT protocol
- Used WebSocket without SSL / TLS
- Connects only using the Paho.js library
- Publications are only possible with QoS = 0

## Tested with

Written and tested under ESP8266

## Known Issues

The library is still a draft, in some cases, the settings of the widgets cause the IoTmanager's reconnection, the cause of which I can not find yet

## Versions

v.0.1.0 - minimum working version
