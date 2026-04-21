---
description: DeviceRoamingStatus schema
layout: schema
name: DeviceRoamingStatus
properties_list:
- description: Whether the device is roaming
  name: roaming
  type: boolean
- description: Country code where device is roaming (ITU-T E.164)
  name: countryCode
  type: integer
- description: Country name(s) where device is roaming
  name: countryName
  type: array
provider_name: AT&T Developer Hub
provider_slug: at-t-developer-hub
schema_file: json-schema/device-status-api-device-roaming-status-schema.json
slug: device-status-api-device-roaming-status
tags:
- 5G
- Network APIs
- CAMARA
- Connectivity
- Telecommunications
- Edge Computing
- Device Status
- SIM Swap
title: DeviceRoamingStatus
---
