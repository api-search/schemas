---
description: Performance counters for an AMD GPU device.
layout: schema
name: DevicePerformance
properties_list:
- description: ''
  name: deviceId
  type: string
- description: ''
  name: gpuUtilization
  type: number
- description: ''
  name: memoryUtilization
  type: number
- description: ''
  name: memoryBandwidth
  type: number
- description: ''
  name: computeThroughput
  type: number
provider_name: Advanced Micro Devices
provider_slug: advanced-micro-devices
schema_file: json-schema/rocm-api-device-performance-schema.json
slug: rocm-api-device-performance
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DevicePerformance\",\n  \"description\": \"Performance counters for an AMD GPU device.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deviceId\": {\n      \"type\": \"string\"\n    },\n    \"gpuUtilization\": {\n      \"type\": \"number\"\n    },\n    \"memoryUtilization\": {\n      \"type\": \"number\"\n    },\n    \"memoryBandwidth\": {\n      \"type\": \"number\"\n    },\n    \"computeThroughput\": {\n      \"type\": \"number\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/advanced-micro-devices/refs/heads/main/json-schema/rocm-api-device-performance-schema.json
tags:
- AI
- Cloud Computing
- GPU
- HPC
- Machine Learning
- Semiconductor
title: DevicePerformance
---
