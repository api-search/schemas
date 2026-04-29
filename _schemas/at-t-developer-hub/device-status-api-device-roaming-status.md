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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/json-schema/device-status-api-device-roaming-status-schema.json\",\n  \"title\": \"DeviceRoamingStatus\",\n  \"description\": \"DeviceRoamingStatus schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"roaming\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the device is roaming\",\n      \"example\": false\n    },\n    \"countryCode\": {\n      \"type\": \"integer\",\n      \"nullable\": true,\n      \"description\": \"Country code where device is roaming (ITU-T E.164)\",\n      \"example\": null\n    },\n    \"countryName\": {\n      \"type\": \"array\",\n      \"nullable\": true,\n      \"description\": \"Country name(s) where device is roaming\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": null\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/json-schema/device-status-api-device-roaming-status-schema.json
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
