---
description: Schema for a Samsung SmartThings connected device entity as returned by the SmartThings REST API. Represents any device connected to the SmartThings platform including Samsung appliances, lights, locks, thermostats, sensors, and third-party Works with SmartThings devices.
layout: schema
name: Samsung SmartThings Device
properties_list:
- description: Unique device identifier (UUID).
  name: deviceId
  type: string
- description: Device display name set by the user or manufacturer.
  name: name
  type: string
- description: User-assigned label for the device.
  name: label
  type: string
- description: Name of the device manufacturer.
  name: manufacturerName
  type: string
- description: Device presentation identifier for UI rendering.
  name: presentationId
  type: string
- description: Manufacturer-assigned device type code.
  name: deviceManufacturerCode
  type: string
- description: ID of the SmartThings location this device belongs to.
  name: locationId
  type: string
- description: ID of the user account that owns the device.
  name: ownerId
  type: string
- description: ID of the room this device is assigned to.
  name: roomId
  type: string
- description: Device components, each representing a functional sub-unit (e.g., main, sub).
  name: components
  type: array
- description: Device integration type.
  name: type
  type: string
- description: Restriction level for the device.
  name: restrictionTier
  type: integer
- description: List of allowed actions on this device.
  name: allowed
  type: array
provider_name: Samsung
provider_slug: samsung
schema_file: json-schema/samsung-smartthings-device-schema.json
slug: samsung-smartthings-device
source_filename: samsung-smartthings-device-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"samsung-smartthings-device-schema.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Samsung SmartThings Device\",\n  \"description\": \"Schema for a Samsung SmartThings connected device entity as returned by the SmartThings REST API. Represents any device connected to the SmartThings platform including Samsung appliances, lights, locks, thermostats, sensors, and third-party Works with SmartThings devices.\",\n  \"type\": \"object\",\n  \"required\": [\"deviceId\", \"name\", \"manufacturerName\", \"presentationId\"],\n  \"properties\": {\n    \"deviceId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique device identifier (UUID).\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Device display name set by the user or manufacturer.\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"User-assigned label for the device.\"\
  \n    },\n    \"manufacturerName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the device manufacturer.\"\n    },\n    \"presentationId\": {\n      \"type\": \"string\",\n      \"description\": \"Device presentation identifier for UI rendering.\"\n    },\n    \"deviceManufacturerCode\": {\n      \"type\": \"string\",\n      \"description\": \"Manufacturer-assigned device type code.\"\n    },\n    \"locationId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"ID of the SmartThings location this device belongs to.\"\n    },\n    \"ownerId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the user account that owns the device.\"\n    },\n    \"roomId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"ID of the room this device is assigned to.\"\n    },\n    \"components\": {\n      \"type\": \"array\",\n      \"description\": \"Device components, each representing a functional\
  \ sub-unit (e.g., main, sub).\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"Component ID (main, sub, etc.).\"\n          },\n          \"label\": {\n            \"type\": \"string\",\n            \"description\": \"Human-readable component label.\"\n          },\n          \"capabilities\": {\n            \"type\": \"array\",\n            \"description\": \"SmartThings capabilities supported by this component.\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"id\": {\n                  \"type\": \"string\",\n                  \"description\": \"Capability identifier (e.g., switch, temperatureMeasurement, motionSensor).\"\n                },\n                \"version\": {\n                  \"type\": \"integer\",\n                  \"description\": \"Capability version.\"\n                }\n     \
  \         }\n            }\n          },\n          \"categories\": {\n            \"type\": \"array\",\n            \"description\": \"Device category classifications.\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"name\": {\n                  \"type\": \"string\",\n                  \"description\": \"Category name (e.g., Light, Thermostat, Lock).\"\n                },\n                \"categoryType\": {\n                  \"type\": \"string\",\n                  \"enum\": [\"manufacturer\", \"user\"]\n                }\n              }\n            }\n          }\n        }\n      }\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Device integration type.\",\n      \"enum\": [\"ENDPOINT_APP\", \"DTH\", \"MOBILE\", \"VIPER\", \"MATTER\", \"LAN\", \"BLE\", \"ZWave\", \"Zigbee\", \"IR_OCF\", \"HUB\"]\n    },\n    \"restrictionTier\": {\n      \"type\": \"integer\",\n      \"description\"\
  : \"Restriction level for the device.\",\n      \"minimum\": 0\n    },\n    \"allowed\": {\n      \"type\": \"array\",\n      \"description\": \"List of allowed actions on this device.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/samsung/refs/heads/main/json-schema/samsung-smartthings-device-schema.json
tags:
- Consumer Electronics
- Developer Platform
- IoT
- Mobile
- Smart Home
- Smart TV
- Wearables
title: Samsung SmartThings Device
---
