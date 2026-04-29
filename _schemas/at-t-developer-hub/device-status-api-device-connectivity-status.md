---
description: DeviceConnectivityStatus schema
layout: schema
name: DeviceConnectivityStatus
properties_list:
- description: Current device connectivity state
  name: connectivityStatus
  type: string
- description: Whether the device is currently roaming
  name: roaming
  type: boolean
provider_name: AT&T Developer Hub
provider_slug: at-t-developer-hub
schema_file: json-schema/device-status-api-device-connectivity-status-schema.json
slug: device-status-api-device-connectivity-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/json-schema/device-status-api-device-connectivity-status-schema.json\",\n  \"title\": \"DeviceConnectivityStatus\",\n  \"description\": \"DeviceConnectivityStatus schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"connectivityStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Current device connectivity state\",\n      \"enum\": [\n        \"CONNECTED_DATA\",\n        \"CONNECTED_SMS\",\n        \"NOT_CONNECTED\"\n      ],\n      \"example\": \"CONNECTED_DATA\"\n    },\n    \"roaming\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the device is currently roaming\",\n      \"example\": false\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/json-schema/device-status-api-device-connectivity-status-schema.json
tags:
- 5G
- Network APIs
- CAMARA
- Connectivity
- Telecommunications
- Edge Computing
- Device Status
- SIM Swap
title: DeviceConnectivityStatus
---
