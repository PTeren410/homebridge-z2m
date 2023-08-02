---
title: "TuYa SPM02 Homebridge/HomeKit integration"
description: "Add HomeKit support to your TuYa SPM02, using Homebridge, Zigbee2MQTT and homebridge-z2m."
---
<!---
This file has been GENERATED using src/docgen/docgen.ts
DO NOT EDIT THIS FILE MANUALLY!
-->
# TuYa SPM02
> Smart energy monitor for 3P+N system


# Unsupported

This device is currently *UNSUPPORTED*.
Want to have this device supported? Please check the [GitHub issue section](https://github.com/itavero/homebridge-z2m/issues?q=SPM02) to see if a request already exists for this device.
If it doesn't exist yet, you can [open a new request](https://github.com/itavero/homebridge-z2m/issues/new?assignees=&labels=enhancement&template=device_support.yml&title=%5BDevice%5D+TuYa%20SPM02&model=TuYa%20SPM02&exposes=%5B%0A%20%20%7B%0A%20%20%20%20%22type%22%3A%20%22numeric%22%2C%0A%20%20%20%20%22name%22%3A%20%22voltage_X%22%2C%0A%20%20%20%20%22property%22%3A%20%22voltage_X%22%2C%0A%20%20%20%20%22access%22%3A%201%2C%0A%20%20%20%20%22unit%22%3A%20%22V%22%2C%0A%20%20%20%20%22description%22%3A%20%22Measured%20electrical%20potential%20value%20(phase%20X)%22%0A%20%20%7D%2C%0A%20%20%7B%0A%20%20%20%20%22type%22%3A%20%22numeric%22%2C%0A%20%20%20%20%22name%22%3A%20%22voltage_Y%22%2C%0A%20%20%20%20%22property%22%3A%20%22voltage_Y%22%2C%0A%20%20%20%20%22access%22%3A%201%2C%0A%20%20%20%20%22unit%22%3A%20%22V%22%2C%0A%20%20%20%20%22description%22%3A%20%22Measured%20electrical%20potential%20value%20(phase%20Y)%22%0A%20%20%7D%2C%0A%20%20%7B%0A%20%20%20%20%22type%22%3A%20%22numeric%22%2C%0A%20%20%20%20%22name%22%3A%20%22voltage_Z%22%2C%0A%20%20%20%20%22property%22%3A%20%22voltage_Z%22%2C%0A%20%20%20%20%22access%22%3A%201%2C%0A%20%20%20%20%22unit%22%3A%20%22V%22%2C%0A%20%20%20%20%22description%22%3A%20%22Measured%20electrical%20potential%20value%20(phase%20Z)%22%0A%20%20%7D%2C%0A%20%20%7B%0A%20%20%20%20%22type%22%3A%20%22numeric%22%2C%0A%20%20%20%20%22name%22%3A%20%22power_X%22%2C%0A%20%20%20%20%22property%22%3A%20%22power_X%22%2C%0A%20%20%20%20%22access%22%3A%201%2C%0A%20%20%20%20%22unit%22%3A%20%22W%22%2C%0A%20%20%20%20%22description%22%3A%20%22Instantaneous%20measured%20power%20(phase%20X)%22%0A%20%20%7D%2C%0A%20%20%7B%0A%20%20%20%20%22type%22%3A%20%22numeric%22%2C%0A%20%20%20%20%22name%22%3A%20%22power_Y%22%2C%0A%20%20%20%20%22property%22%3A%20%22power_Y%22%2C%0A%20%20%20%20%22access%22%3A%201%2C%0A%20%20%20%20%22unit%22%3A%20%22W%22%2C%0A%20%20%20%20%22description%22%3A%20%22Instantaneous%20measured%20power%20(phase%20Y)%22%0A%20%20%7D%2C%0A%20%20%7B%0A%20%20%20%20%22type%22%3A%20%22numeric%22%2C%0A%20%20%20%20%22name%22%3A%20%22power_Z%22%2C%0A%20%20%20%20%22property%22%3A%20%22power_Z%22%2C%0A%20%20%20%20%22access%22%3A%201%2C%0A%20%20%20%20%22unit%22%3A%20%22W%22%2C%0A%20%20%20%20%22description%22%3A%20%22Instantaneous%20measured%20power%20(phase%20Z)%22%0A%20%20%7D%2C%0A%20%20%7B%0A%20%20%20%20%22type%22%3A%20%22numeric%22%2C%0A%20%20%20%20%22name%22%3A%20%22current_X%22%2C%0A%20%20%20%20%22property%22%3A%20%22current_X%22%2C%0A%20%20%20%20%22access%22%3A%201%2C%0A%20%20%20%20%22unit%22%3A%20%22A%22%2C%0A%20%20%20%20%22description%22%3A%20%22Instantaneous%20measured%20electrical%20current%20(phase%20X)%22%0A%20%20%7D%2C%0A%20%20%7B%0A%20%20%20%20%22type%22%3A%20%22numeric%22%2C%0A%20%20%20%20%22name%22%3A%20%22current_Y%22%2C%0A%20%20%20%20%22property%22%3A%20%22current_Y%22%2C%0A%20%20%20%20%22access%22%3A%201%2C%0A%20%20%20%20%22unit%22%3A%20%22A%22%2C%0A%20%20%20%20%22description%22%3A%20%22Instantaneous%20measured%20electrical%20current%20(phase%20Y)%22%0A%20%20%7D%2C%0A%20%20%7B%0A%20%20%20%20%22type%22%3A%20%22numeric%22%2C%0A%20%20%20%20%22name%22%3A%20%22current_Z%22%2C%0A%20%20%20%20%22property%22%3A%20%22current_Z%22%2C%0A%20%20%20%20%22access%22%3A%201%2C%0A%20%20%20%20%22unit%22%3A%20%22A%22%2C%0A%20%20%20%20%22description%22%3A%20%22Instantaneous%20measured%20electrical%20current%20(phase%20Z)%22%0A%20%20%7D%2C%0A%20%20%7B%0A%20%20%20%20%22type%22%3A%20%22numeric%22%2C%0A%20%20%20%20%22name%22%3A%20%22energy%22%2C%0A%20%20%20%20%22property%22%3A%20%22energy%22%2C%0A%20%20%20%20%22access%22%3A%201%2C%0A%20%20%20%20%22unit%22%3A%20%22kWh%22%2C%0A%20%20%20%20%22description%22%3A%20%22Total%20forward%20active%20energy%22%0A%20%20%7D%2C%0A%20%20%7B%0A%20%20%20%20%22type%22%3A%20%22numeric%22%2C%0A%20%20%20%20%22name%22%3A%20%22produced_energy%22%2C%0A%20%20%20%20%22property%22%3A%20%22produced_energy%22%2C%0A%20%20%20%20%22access%22%3A%201%2C%0A%20%20%20%20%22unit%22%3A%20%22kWh%22%2C%0A%20%20%20%20%22description%22%3A%20%22Total%20reverse%20active%20energy%22%0A%20%20%7D%2C%0A%20%20%7B%0A%20%20%20%20%22type%22%3A%20%22numeric%22%2C%0A%20%20%20%20%22name%22%3A%20%22linkquality%22%2C%0A%20%20%20%20%22property%22%3A%20%22linkquality%22%2C%0A%20%20%20%20%22access%22%3A%201%2C%0A%20%20%20%20%22unit%22%3A%20%22lqi%22%2C%0A%20%20%20%20%22description%22%3A%20%22Link%20quality%20(signal%20strength)%22%2C%0A%20%20%20%20%22value_min%22%3A%200%2C%0A%20%20%20%20%22value_max%22%3A%20255%0A%20%20%7D%0A%5D) by filling in the _Device support_ issue template.

## Exposes

This is the information provided by Zigbee2MQTT for this device:

```json
[
  {
    "type": "numeric",
    "name": "voltage_X",
    "property": "voltage_X",
    "access": 1,
    "unit": "V",
    "description": "Measured electrical potential value (phase X)"
  },
  {
    "type": "numeric",
    "name": "voltage_Y",
    "property": "voltage_Y",
    "access": 1,
    "unit": "V",
    "description": "Measured electrical potential value (phase Y)"
  },
  {
    "type": "numeric",
    "name": "voltage_Z",
    "property": "voltage_Z",
    "access": 1,
    "unit": "V",
    "description": "Measured electrical potential value (phase Z)"
  },
  {
    "type": "numeric",
    "name": "power_X",
    "property": "power_X",
    "access": 1,
    "unit": "W",
    "description": "Instantaneous measured power (phase X)"
  },
  {
    "type": "numeric",
    "name": "power_Y",
    "property": "power_Y",
    "access": 1,
    "unit": "W",
    "description": "Instantaneous measured power (phase Y)"
  },
  {
    "type": "numeric",
    "name": "power_Z",
    "property": "power_Z",
    "access": 1,
    "unit": "W",
    "description": "Instantaneous measured power (phase Z)"
  },
  {
    "type": "numeric",
    "name": "current_X",
    "property": "current_X",
    "access": 1,
    "unit": "A",
    "description": "Instantaneous measured electrical current (phase X)"
  },
  {
    "type": "numeric",
    "name": "current_Y",
    "property": "current_Y",
    "access": 1,
    "unit": "A",
    "description": "Instantaneous measured electrical current (phase Y)"
  },
  {
    "type": "numeric",
    "name": "current_Z",
    "property": "current_Z",
    "access": 1,
    "unit": "A",
    "description": "Instantaneous measured electrical current (phase Z)"
  },
  {
    "type": "numeric",
    "name": "energy",
    "property": "energy",
    "access": 1,
    "unit": "kWh",
    "description": "Total forward active energy"
  },
  {
    "type": "numeric",
    "name": "produced_energy",
    "property": "produced_energy",
    "access": 1,
    "unit": "kWh",
    "description": "Total reverse active energy"
  },
  {
    "type": "numeric",
    "name": "linkquality",
    "property": "linkquality",
    "access": 1,
    "unit": "lqi",
    "description": "Link quality (signal strength)",
    "value_min": 0,
    "value_max": 255
  }
]
```

# Related
* [Other devices from TuYa](../index.md#tuya)
* [Zigbee2MQTT documentation for this device](https://www.zigbee2mqtt.io/devices/SPM02.html)