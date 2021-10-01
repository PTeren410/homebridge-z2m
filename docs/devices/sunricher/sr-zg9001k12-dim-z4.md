---
title: "Sunricher SR-ZG9001K12-DIM-Z4 Homebridge/HomeKit integration"
description: "Add HomeKit support to your Sunricher SR-ZG9001K12-DIM-Z4, using Homebridge, Zigbee2MQTT and homebridge-z2m."
---
<!---
This file has been GENERATED using src/docgen/docgen.ts
DO NOT EDIT THIS FILE MANUALLY!
-->
# Sunricher SR-ZG9001K12-DIM-Z4
> 4 zone remote and dimmer


## White-label models
* [RGB Genie](../index.md#rgb_genie) ZGRC-KEY-013

# Services and characteristics
The following HomeKit Services and Characteristics are exposed by
these devices

* [Battery](../../battery.md)
  * BatteryLevel
  * ChargingState
  * StatusLowBattery



## Exposes

```json
[
  {
    "type": "numeric",
    "name": "battery",
    "property": "battery",
    "access": 1,
    "unit": "%",
    "description": "Remaining battery in %",
    "value_min": 0,
    "value_max": 100
  },
  {
    "type": "enum",
    "name": "action",
    "property": "action",
    "access": 1,
    "values": [
      "brightness_move_up",
      "brightness_move_down",
      "brightness_stop",
      "on",
      "off",
      "recall_*"
    ],
    "description": "Triggered action (e.g. a button click)"
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
* [Other devices from Sunricher](../index.md#sunricher)
* [Zigbee2MQTT documentation for this device](https://www.zigbee2mqtt.io/devices/SR-ZG9001K12-DIM-Z4.html)