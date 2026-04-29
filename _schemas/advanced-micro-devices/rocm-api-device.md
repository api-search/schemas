---
description: An AMD GPU device.
layout: schema
name: Device
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: model
  type: string
- description: ''
  name: vbios
  type: string
- description: ''
  name: driverVersion
  type: string
- description: Total GPU memory GB.
  name: memoryTotal
  type: integer
- description: ''
  name: pcieBusId
  type: string
- description: ''
  name: computeUnits
  type: integer
provider_name: Advanced Micro Devices
provider_slug: advanced-micro-devices
schema_file: json-schema/rocm-api-device-schema.json
slug: rocm-api-device
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Device\",\n  \"description\": \"An AMD GPU device.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"model\": {\n      \"type\": \"string\"\n    },\n    \"vbios\": {\n      \"type\": \"string\"\n    },\n    \"driverVersion\": {\n      \"type\": \"string\"\n    },\n    \"memoryTotal\": {\n      \"type\": \"integer\",\n      \"description\": \"Total GPU memory GB.\"\n    },\n    \"pcieBusId\": {\n      \"type\": \"string\"\n    },\n    \"computeUnits\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/advanced-micro-devices/refs/heads/main/json-schema/rocm-api-device-schema.json
tags:
- AI
- Cloud Computing
- GPU
- HPC
- Machine Learning
- Semiconductor
title: Device
---
