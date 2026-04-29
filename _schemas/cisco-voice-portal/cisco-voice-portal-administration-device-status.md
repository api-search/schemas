---
description: ''
layout: schema
name: DeviceStatus
properties_list:
- description: ''
  name: deviceId
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: services
  type: array
- description: CPU usage percentage
  name: cpuUsage
  type: number
- description: Memory usage percentage
  name: memoryUsage
  type: number
- description: Number of active calls on this device
  name: activeCalls
  type: integer
- description: ''
  name: timestamp
  type: string
provider_name: Cisco Voice Portal
provider_slug: cisco-voice-portal
schema_file: json-schema/cisco-voice-portal-administration-device-status-schema.json
slug: cisco-voice-portal-administration-device-status
source_filename: cisco-voice-portal-administration-device-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeviceStatus\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deviceId\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"services\": {\n      \"type\": \"array\"\n    },\n    \"cpuUsage\": {\n      \"type\": \"number\",\n      \"description\": \"CPU usage percentage\"\n    },\n    \"memoryUsage\": {\n      \"type\": \"number\",\n      \"description\": \"Memory usage percentage\"\n    },\n    \"activeCalls\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of active calls on this device\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/json-schema/cisco-voice-portal-administration-device-status-schema.json
tags:
- Contact Center
- IVR
- Telephony
- Voice
- VXML
title: DeviceStatus
---
