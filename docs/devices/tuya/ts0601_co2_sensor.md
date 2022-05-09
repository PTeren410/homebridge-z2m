---
title: "TuYa TS0601_co2_sensor Homebridge/HomeKit integration"
description: "Add HomeKit support to your TuYa TS0601_co2_sensor, using Homebridge, Zigbee2MQTT and homebridge-z2m."
---
<!---
This file has been GENERATED using src/docgen/docgen.ts
DO NOT EDIT THIS FILE MANUALLY!
-->
# TuYa TS0601_co2_sensor
> NDIR co2 sensor


# Unsupported

This device is currently *UNSUPPORTED*.
Want to have this device supported? Please check the [GitHub issue section](https://github.com/itavero/homebridge-z2m/issues?q=TS0601_co2_sensor) to see if a request already exists for this device.
If it doesn't exist yet, you can [open a new request](https://github.com/itavero/homebridge-z2m/issues/new?assignees=&labels=enhancement&template=device_support.md&title=%5BDevice%5D+TuYa+TS0601_co2_sensor) by filling in the _Device support_ issue template.

## Exposes

```json
[
  {
    "type": "numeric",
    "name": "co2",
    "property": "co2",
    "access": 1,
    "unit": "ppm",
    "description": "The measured CO2 (carbon dioxide) value"
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
* [Zigbee2MQTT documentation for this device](https://www.zigbee2mqtt.io/devices/TS0601_co2_sensor.html)