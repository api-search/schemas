---
description: Schema for a decoded BLE advertising packet (ADV_IND or ADV_NONCONN_IND)
layout: schema
name: BLE Advertising Packet
properties_list:
- description: BLE device MAC address
  name: address
  type: string
- description: ''
  name: addressType
  type: string
- description: Received signal strength indicator in dBm
  name: rssi
  type: integer
- description: Complete or shortened local name
  name: localName
  type: string
- description: Advertised service UUIDs
  name: serviceUUIDs
  type: array
- description: ''
  name: manufacturerData
  type: object
- description: Transmit power level in dBm
  name: txPowerLevel
  type: integer
- description: Whether device accepts connections
  name: connectable
  type: boolean
provider_name: BLE
provider_slug: ble
schema_file: json-schema/ble-advertising-packet-schema.json
slug: ble-advertising-packet
source_filename: ble-advertising-packet-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ble/main/json-schema/ble-advertising-packet-schema.json\",\n  \"title\": \"BLE Advertising Packet\",\n  \"description\": \"Schema for a decoded BLE advertising packet (ADV_IND or ADV_NONCONN_IND)\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"address\": {\n      \"type\": \"string\",\n      \"description\": \"BLE device MAC address\",\n      \"pattern\": \"^([0-9A-Fa-f]{2}:){5}[0-9A-Fa-f]{2}$\"\n    },\n    \"addressType\": {\n      \"type\": \"string\",\n      \"enum\": [\"public\", \"random_static\", \"random_private_resolvable\", \"random_private_non_resolvable\"]\n    },\n    \"rssi\": {\n      \"type\": \"integer\",\n      \"description\": \"Received signal strength indicator in dBm\",\n      \"minimum\": -127,\n      \"maximum\": 0\n    },\n    \"localName\": { \"type\": \"string\", \"description\": \"Complete or shortened local name\"\
  \ },\n    \"serviceUUIDs\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\" },\n      \"description\": \"Advertised service UUIDs\"\n    },\n    \"manufacturerData\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"companyId\": { \"type\": \"integer\", \"description\": \"Bluetooth SIG-assigned company identifier\" },\n        \"data\": { \"type\": \"string\", \"description\": \"Hex-encoded manufacturer specific data\" }\n      }\n    },\n    \"txPowerLevel\": { \"type\": \"integer\", \"description\": \"Transmit power level in dBm\" },\n    \"connectable\": { \"type\": \"boolean\", \"description\": \"Whether device accepts connections\" }\n  },\n  \"required\": [\"address\", \"rssi\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ble/refs/heads/main/json-schema/ble-advertising-packet-schema.json
tags:
- BLE
- Bluetooth
- Embedded
- IoT
- Protocols
- Standards
- Wireless
title: BLE Advertising Packet
---
