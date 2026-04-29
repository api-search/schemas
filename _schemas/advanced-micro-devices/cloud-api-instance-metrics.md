---
description: Real-time performance metrics for a GPU instance.
layout: schema
name: InstanceMetrics
properties_list:
- description: ''
  name: instanceId
  type: string
- description: GPU utilization %.
  name: gpuUtilization
  type: number
- description: Memory used GB.
  name: memoryUsed
  type: number
- description: Total memory GB.
  name: memoryTotal
  type: number
- description: Temperature Celsius.
  name: temperature
  type: integer
- description: Power draw watts.
  name: powerDraw
  type: number
provider_name: Advanced Micro Devices
provider_slug: advanced-micro-devices
schema_file: json-schema/cloud-api-instance-metrics-schema.json
slug: cloud-api-instance-metrics
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InstanceMetrics\",\n  \"description\": \"Real-time performance metrics for a GPU instance.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"instanceId\": {\n      \"type\": \"string\"\n    },\n    \"gpuUtilization\": {\n      \"type\": \"number\",\n      \"description\": \"GPU utilization %.\"\n    },\n    \"memoryUsed\": {\n      \"type\": \"number\",\n      \"description\": \"Memory used GB.\"\n    },\n    \"memoryTotal\": {\n      \"type\": \"number\",\n      \"description\": \"Total memory GB.\"\n    },\n    \"temperature\": {\n      \"type\": \"integer\",\n      \"description\": \"Temperature Celsius.\"\n    },\n    \"powerDraw\": {\n      \"type\": \"number\",\n      \"description\": \"Power draw watts.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/advanced-micro-devices/refs/heads/main/json-schema/cloud-api-instance-metrics-schema.json
tags:
- AI
- Cloud Computing
- GPU
- HPC
- Machine Learning
- Semiconductor
title: InstanceMetrics
---
