---
title: "Bosch BSIR-EZ Homebridge/HomeKit integration"
description: "Add HomeKit support to your Bosch BSIR-EZ, using Homebridge, Zigbee2MQTT and homebridge-z2m."
---
<!---
This file has been GENERATED using src/docgen/docgen.ts
DO NOT EDIT THIS FILE MANUALLY!
-->
# Bosch BSIR-EZ
> Outdoor siren


# Services and characteristics
The following HomeKit Services and Characteristics are exposed by
the Bosch BSIR-EZ

* [Battery](../../battery.md)
  * Battery Level
  * Charging State
  * Status Low Battery



## Exposes

This is the information provided by Zigbee2MQTT for this device:

```json
[
  {
    "name": "alarm_state",
    "label": "Alarm state",
    "access": 7,
    "type": "binary",
    "property": "alarm_state",
    "description": "Alarm turn ON/OFF",
    "value_on": "ON",
    "value_off": "OFF"
  },
  {
    "name": "light_delay",
    "label": "Light delay",
    "access": 7,
    "type": "numeric",
    "property": "light_delay",
    "description": "Flashing light delay",
    "unit": "s",
    "value_max": 30,
    "value_min": 0,
    "value_step": 1
  },
  {
    "name": "siren_delay",
    "label": "Siren delay",
    "access": 7,
    "type": "numeric",
    "property": "siren_delay",
    "description": "Siren alarm delay",
    "unit": "s",
    "value_max": 30,
    "value_min": 0,
    "value_step": 1
  },
  {
    "name": "siren_duration",
    "label": "Siren duration",
    "access": 7,
    "type": "numeric",
    "property": "siren_duration",
    "description": "Duration of the alarm siren",
    "unit": "m",
    "value_max": 15,
    "value_min": 1,
    "value_step": 1
  },
  {
    "name": "light_duration",
    "label": "Light duration",
    "access": 7,
    "type": "numeric",
    "property": "light_duration",
    "description": "Duration of the alarm light",
    "unit": "m",
    "value_max": 15,
    "value_min": 1,
    "value_step": 1
  },
  {
    "name": "siren_volume",
    "label": "Siren volume",
    "access": 7,
    "type": "enum",
    "property": "siren_volume",
    "description": "Volume of the alarm",
    "values": [
      "low",
      "medium",
      "high"
    ]
  },
  {
    "name": "siren_and_light",
    "label": "Siren and light",
    "access": 7,
    "type": "enum",
    "property": "siren_and_light",
    "description": "Siren and Light behaviour during alarm ",
    "values": [
      "only_light",
      "only_siren",
      "siren_and_light"
    ]
  },
  {
    "name": "power_source",
    "label": "Power source",
    "access": 7,
    "type": "enum",
    "property": "power_source",
    "description": "Siren power source",
    "values": [
      "solar_panel",
      "ac_power_supply",
      "dc_power_supply"
    ]
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
      }
    ]
  },
  {
    "name": "test",
    "label": "Test",
    "access": 1,
    "type": "binary",
    "property": "test",
    "description": "Indicates whether the device is being tested",
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
    "value_on": true,
    "value_off": false
  },
  {
    "name": "battery",
    "label": "Battery",
    "access": 1,
    "type": "numeric",
    "property": "battery",
    "description": "Remaining battery in %, can take up to 24 hours before reported.",
    "unit": "%",
    "value_max": 100,
    "value_min": 0
  },
  {
    "name": "voltage",
    "label": "Voltage",
    "access": 1,
    "type": "numeric",
    "property": "voltage",
    "description": "Voltage of the battery in millivolts",
    "unit": "mV"
  },
  {
    "name": "battery_low",
    "label": "Battery low",
    "access": 1,
    "type": "binary",
    "property": "battery_low",
    "description": "Indicates if the battery of this device is almost empty",
    "value_on": true,
    "value_off": false
  },
  {
    "name": "ac_status",
    "label": "Ac status",
    "access": 1,
    "type": "binary",
    "property": "ac_status",
    "description": "Is the device plugged in",
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
    "unit": "lqi",
    "value_max": 255,
    "value_min": 0
  }
]
```

# Related
* [Other devices from Bosch](../index.md#bosch)
* [Zigbee2MQTT documentation for this device](https://www.zigbee2mqtt.io/devices/BSIR-EZ.html)