---
description: Schema representing a Bluetooth GATT service definition as assigned by the Bluetooth SIG
layout: schema
name: BLE GATT Service
properties_list:
- description: 16-bit or 128-bit UUID assigned by Bluetooth SIG or custom
  name: uuid
  type: string
- description: Human-readable service name
  name: name
  type: string
- description: Whether this is a SIG-assigned or custom service
  name: type
  type: string
- description: GATT characteristics included in this service
  name: characteristics
  type: array
provider_name: BLE
provider_slug: ble
schema_file: json-schema/ble-gatt-service-schema.json
slug: ble-gatt-service
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ble/main/json-schema/ble-gatt-service-schema.json\",\n  \"title\": \"BLE GATT Service\",\n  \"description\": \"Schema representing a Bluetooth GATT service definition as assigned by the Bluetooth SIG\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"uuid\": {\n      \"type\": \"string\",\n      \"description\": \"16-bit or 128-bit UUID assigned by Bluetooth SIG or custom\",\n      \"examples\": [\"0x180D\", \"0000180d-0000-1000-8000-00805f9b34fb\"]\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable service name\",\n      \"examples\": [\"Heart Rate\", \"Battery Service\", \"Device Information\"]\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"org.bluetooth.service\", \"custom\"],\n      \"description\": \"Whether this is a SIG-assigned or custom service\"\n    },\n    \"\
  characteristics\": {\n      \"type\": \"array\",\n      \"description\": \"GATT characteristics included in this service\",\n      \"items\": {\n        \"$ref\": \"#/$defs/GattCharacteristic\"\n      }\n    }\n  },\n  \"required\": [\"uuid\", \"name\"],\n  \"$defs\": {\n    \"GattCharacteristic\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"uuid\": { \"type\": \"string\" },\n        \"name\": { \"type\": \"string\" },\n        \"properties\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\",\n            \"enum\": [\"Read\", \"Write\", \"Write Without Response\", \"Notify\", \"Indicate\", \"Broadcast\", \"Extended Properties\"]\n          }\n        },\n        \"format\": { \"type\": \"string\", \"description\": \"Data format descriptor\" },\n        \"unit\": { \"type\": \"string\", \"description\": \"Unit of measurement (GATT unit UUID)\" }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ble/refs/heads/main/json-schema/ble-gatt-service-schema.json
tags:
- BLE
- Bluetooth
- Embedded
- IoT
- Protocols
- Standards
- Wireless
title: BLE GATT Service
---
