---
description: A physical or virtual device discovered and monitored by EcoStruxure IT Expert, including UPS, PDU, CRAC, and other data center infrastructure equipment.
layout: schema
name: EcoStruxure IT Device
properties_list:
- description: Unique identifier for the device.
  name: id
  type: string
- description: Display name of the device.
  name: name
  type: string
- description: Device type classification (e.g., UPS, PDU, CRAC, Server, Network).
  name: type
  type: string
- description: Current operational status of the device.
  name: status
  type: string
- description: The location where this device is installed.
  name: location
  type: object
- description: IP address of the device.
  name: ipAddress
  type: string
- description: MAC address of the device.
  name: macAddress
  type: string
- description: Firmware version installed on the device.
  name: firmwareVersion
  type: string
- description: Manufacturer serial number.
  name: serialNumber
  type: string
- description: Manufacturer model number.
  name: modelNumber
  type: string
- description: Sensors attached to or reported by this device.
  name: sensors
  type: array
- description: Active alarms for this device.
  name: alarms
  type: array
- description: Timestamp of the most recent data update from this device.
  name: lastUpdated
  type: string
provider_name: Schneider Electric Exchange
provider_slug: schneider-electric-exchange
schema_file: json-schema/ecostruxure-it-device-schema.json
slug: ecostruxure-it-device
source_filename: ecostruxure-it-device-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.ecostruxureit.com/schemas/device\",\n  \"title\": \"EcoStruxure IT Device\",\n  \"description\": \"A physical or virtual device discovered and monitored by EcoStruxure IT Expert, including UPS, PDU, CRAC, and other data center infrastructure equipment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the device.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the device.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Device type classification (e.g., UPS, PDU, CRAC, Server, Network).\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"normal\", \"warning\", \"critical\", \"unknown\"],\n      \"description\": \"Current operational status of the device.\"\n    },\n    \"location\": {\n\
  \      \"$ref\": \"#/$defs/LocationRef\",\n      \"description\": \"The location where this device is installed.\"\n    },\n    \"ipAddress\": {\n      \"type\": \"string\",\n      \"description\": \"IP address of the device.\"\n    },\n    \"macAddress\": {\n      \"type\": \"string\",\n      \"description\": \"MAC address of the device.\"\n    },\n    \"firmwareVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Firmware version installed on the device.\"\n    },\n    \"serialNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Manufacturer serial number.\"\n    },\n    \"modelNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Manufacturer model number.\"\n    },\n    \"sensors\": {\n      \"type\": \"array\",\n      \"description\": \"Sensors attached to or reported by this device.\",\n      \"items\": { \"$ref\": \"#/$defs/SensorRef\" }\n    },\n    \"alarms\": {\n      \"type\": \"array\",\n      \"description\": \"Active alarms for this\
  \ device.\",\n      \"items\": { \"$ref\": \"#/$defs/AlarmRef\" }\n    },\n    \"lastUpdated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the most recent data update from this device.\"\n    }\n  },\n  \"required\": [\"id\", \"name\", \"type\"],\n  \"$defs\": {\n    \"LocationRef\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": { \"type\": \"string\" },\n        \"name\": { \"type\": \"string\" }\n      }\n    },\n    \"SensorRef\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": { \"type\": \"string\" },\n        \"label\": { \"type\": \"string\" },\n        \"unit\": { \"type\": \"string\" }\n      }\n    },\n    \"AlarmRef\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": { \"type\": \"string\" },\n        \"severity\": { \"type\": \"string\", \"enum\": [\"critical\", \"warning\", \"info\"] },\n        \"description\": { \"type\": \"string\" }\n\
  \      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schneider-electric-exchange/refs/heads/main/json-schema/ecostruxure-it-device-schema.json
tags:
- Building Automation
- Commerce APIs
- EcoStruxure
- Energy Management
- Industrial IoT
- Schneider Electric
title: EcoStruxure IT Device
---
