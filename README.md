# ESPHome Hybrid Inverter (2341)
This project forked from https://github.com/odya/esphome-powmr-hybrid-inverter 

ESPHome config to monitor and management various PowMr Hybrid Inverter models and Inverters that supported by the [**WIFI-VM (WiFi Plug Pro)**](https://powmr.com/products/powmr-wifi-module-with-rs232-remote-monitoring-solution-wifi-vm) device and `SmartESS` cloud application.

## Protocol
Protocol is Modbus RTU via RS232. Protocol ID (SmartESS) : `2341` (hex 0925). Slave ID : `5`. 

Registers map

1) [registers-map.md from original project](/docs/registers-map.md)
2) [0925.json](/docs/0925.json) in JSON fromat from offical app `SmartESS.apk`
3) [registers-map-SmartESS.md](/docs/registers-map-SmartESS.md) - compilated from `0925.json`

## Connection
![PowMr ESP32 connection diagram](images/powmr_esp32_connection.png "PowMr ESP32 connection diagram")

## Usage
1) Copy the contents of the `src` repo folder to your ESPHome configuration directory
2) Edit substitutions & customize `powmr-inverter.yaml` & `main.yaml`
3) Flash firmware to your ESP32

Note. Some registers (like "Machine Type", "Main CPU Version", etc) are commented out in `/modules/inverter.yaml` because I don't need them.

## Inverter card
For easy integration into Home Assistant, you can use the [following snippet](/examples/inverter-card-example.yaml).  
The following custom plugins are required: [sunsynk-power-flow-card](https://github.com/slipx06/sunsynk-power-flow-card), [stack-in-card](https://github.com/custom-cards/stack-in-card), [canary](https://github.com/jcwillox/lovelace-canary).

## References
- https://github.com/odya/esphome-powmr-hybrid-inverter
- https://github.com/leodesigner/powmr_comm 
- https://github.com/syssi/esphome-smg-ii
- https://github.com/syssi/esphome-pipsolar
- https://github.com/alexeyden/openess