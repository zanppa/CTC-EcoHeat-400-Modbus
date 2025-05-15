# CTC Ecoheat 400 Modbus
This repository contains my notes on how to do a custom adapter and configuration to 
connect CTC Ecoheat 400 heat pump to home automation system with Modbus and MQTT.

This repository is based on earlier work by [Kasper-73](https://github.com/kasper-73/CTC-GSi-8---Homeassistant) and 
[Spangsberg](https://github.com/Spangsberg/CTC-EcoHeat400---Homeassistant).

The register map file provided is designed to be used with [Spicier modbus2mqtt](https://github.com/mbs38/spicierModbus2mqtt).

Run using command like
```modbus2mqtt --rtu /dev/ttyUSB0 --rtu-baud 9600 --rtu-parity none --config ecoheat400.csv --mqtt-host <address> --mqtt-port <port> --mqtt-user <username> --mqtt-pass <password> --mqtt-topic ecoheat400 --always-publish```
though I recommend using serial device from ```/dev/serial/by-id/```.
