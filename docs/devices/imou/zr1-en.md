---
title: "IMOU ZR1-EN Homebridge/HomeKit integration"
description: "Add HomeKit support to your IMOU ZR1-EN, using Homebridge, Zigbee2MQTT and homebridge-z2m."
---
<!---
This file has been GENERATED using src/docgen/docgen.ts
DO NOT EDIT THIS FILE MANUALLY!
-->
# IMOU ZR1-EN
> Zigbee ZR1 siren


# Services and characteristics
The following HomeKit Services and Characteristics are exposed by
the IMOU ZR1-EN

* [Battery](../../battery.md)
  * Battery Level
  * Charging State
  * Status Low Battery



## Exposes

This is the information provided by Zigbee2MQTT for this device:

```json
[
  {
    "name": "battery",
    "label": "Battery",
    "access": 5,
    "type": "numeric",
    "property": "battery",
    "description": "Remaining battery in %",
    "category": "diagnostic",
    "unit": "%",
    "value_max": 100,
    "value_min": 0
  },
  {
    "name": "warning",
    "label": "Warning",
    "access": 2,
    "type": "composite",
    "property": "warning",
    "features": [
      {
        "name": "mode",
        "label": "Mode",
        "access": 2,
        "type": "enum",
        "property": "mode",
        "description": "Mode of the warning (sound effect)",
        "values": [
          "stop",
          "burglar",
          "fire",
          "emergency",
          "police_panic",
          "fire_panic",
          "emergency_panic"
        ]
      },
      {
        "name": "level",
        "label": "Level",
        "access": 2,
        "type": "enum",
        "property": "level",
        "description": "Sound level",
        "values": [
          "low",
          "medium",
          "high",
          "very_high"
        ]
      },
      {
        "name": "strobe_level",
        "label": "Strobe level",
        "access": 2,
        "type": "enum",
        "property": "strobe_level",
        "description": "Intensity of the strobe",
        "values": [
          "low",
          "medium",
          "high",
          "very_high"
        ]
      },
      {
        "name": "strobe",
        "label": "Strobe",
        "access": 2,
        "type": "binary",
        "property": "strobe",
        "description": "Turn on/off the strobe (light) during warning",
        "value_on": true,
        "value_off": false
      },
      {
        "name": "strobe_duty_cycle",
        "label": "Strobe duty cycle",
        "access": 2,
        "type": "numeric",
        "property": "strobe_duty_cycle",
        "description": "Length of the flash cycle",
        "value_max": 10,
        "value_min": 0
      },
      {
        "name": "duration",
        "label": "Duration",
        "access": 2,
        "type": "numeric",
        "property": "duration",
        "description": "Duration in seconds of the alarm",
        "unit": "s"
      }
    ]
  },
  {
    "name": "alarm",
    "label": "Alarm",
    "access": 1,
    "type": "binary",
    "property": "alarm",
    "description": "Indicates whether the alarm is triggered",
    "value_on": true,
    "value_off": false
  },
  {
    "name": "tamper",
    "label": "Tamper",
    "access": 1,
    "type": "binary",
    "property": "tamper",
    "description": "Indicates whether the device is tampered",
    "category": "diagnostic",
    "value_on": true,
    "value_off": false
  },
  {
    "name": "battery_low",
    "label": "Battery low",
    "access": 1,
    "type": "binary",
    "property": "battery_low",
    "description": "Indicates whether the battery of the device is almost empty",
    "category": "diagnostic",
    "value_on": true,
    "value_off": false
  },
  {
    "name": "linkquality",
    "label": "Linkquality",
    "access": 1,
    "type": "numeric",
    "property": "linkquality",
    "description": "Link quality (signal strength)",
    "category": "diagnostic",
    "unit": "lqi",
    "value_max": 255,
    "value_min": 0
  }
]
```

# Related
* [Other devices from IMOU](../index.md#imou)
* [Zigbee2MQTT documentation for this device](https://www.zigbee2mqtt.io/devices/ZR1-EN.html)