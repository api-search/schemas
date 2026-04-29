---
description: List of security devices.
layout: schema
name: DeviceList
properties_list:
- description: Array of devices.
  name: devices
  type: array
provider_name: ADT
provider_slug: adt
schema_file: json-schema/platform-api-device-list-schema.json
slug: platform-api-device-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/json-schema/platform-api-device-list-schema.json\",\n  \"title\": \"DeviceList\",\n  \"description\": \"List of security devices.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"devices\": {\n      \"type\": \"array\",\n      \"description\": \"Array of devices.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A security device (sensor, camera, lock, or smart home device).\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"Unique identifier of the device.\",\n            \"example\": \"dev-001\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Display name of the device.\",\n            \"example\": \"Front Door Sensor\"\n          },\n          \"type\": {\n      \
  \      \"type\": \"string\",\n            \"description\": \"Type of device.\",\n            \"enum\": [\n              \"sensor\",\n              \"camera\",\n              \"lock\",\n              \"thermostat\",\n              \"light\",\n              \"doorbell\",\n              \"smoke_detector\",\n              \"flood_sensor\"\n            ],\n            \"example\": \"sensor\"\n          },\n          \"status\": {\n            \"type\": \"string\",\n            \"description\": \"Current status of the device.\",\n            \"example\": \"closed\"\n          },\n          \"zone\": {\n            \"type\": \"string\",\n            \"description\": \"Security zone the device belongs to.\",\n            \"example\": \"Zone 1 - Entry\"\n          },\n          \"batteryLevel\": {\n            \"type\": \"integer\",\n            \"description\": \"Battery level percentage (0-100) for battery-powered devices.\",\n            \"example\": 85\n          },\n          \"lastActivity\"\
  : {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"Timestamp of last device activity.\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/json-schema/platform-api-device-list-schema.json
tags:
- Access Control
- Automation
- Home Security
- IoT
- Monitoring
- Security
- Smart Home
title: DeviceList
---
