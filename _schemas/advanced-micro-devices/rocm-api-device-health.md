---
description: Health status of an AMD GPU device.
layout: schema
name: DeviceHealth
properties_list:
- description: ''
  name: deviceId
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: temperature
  type: integer
- description: ''
  name: fanSpeed
  type: integer
- description: ''
  name: powerDraw
  type: number
- description: ''
  name: eccErrors
  type: integer
provider_name: Advanced Micro Devices
provider_slug: advanced-micro-devices
schema_file: json-schema/rocm-api-device-health-schema.json
slug: rocm-api-device-health
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeviceHealth\",\n  \"description\": \"Health status of an AMD GPU device.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deviceId\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"healthy\",\n        \"warning\",\n        \"critical\",\n        \"unknown\"\n      ]\n    },\n    \"temperature\": {\n      \"type\": \"integer\"\n    },\n    \"fanSpeed\": {\n      \"type\": \"integer\"\n    },\n    \"powerDraw\": {\n      \"type\": \"number\"\n    },\n    \"eccErrors\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/advanced-micro-devices/refs/heads/main/json-schema/rocm-api-device-health-schema.json
tags:
- AI
- Cloud Computing
- GPU
- HPC
- Machine Learning
- Semiconductor
title: DeviceHealth
---
