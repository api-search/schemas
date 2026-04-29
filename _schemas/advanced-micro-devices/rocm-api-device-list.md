---
description: List of AMD GPU devices.
layout: schema
name: DeviceList
properties_list:
- description: Array of devices.
  name: devices
  type: array
provider_name: Advanced Micro Devices
provider_slug: advanced-micro-devices
schema_file: json-schema/rocm-api-device-list-schema.json
slug: rocm-api-device-list
source_filename: rocm-api-device-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeviceList\",\n  \"description\": \"List of AMD GPU devices.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"devices\": {\n      \"type\": \"array\",\n      \"description\": \"Array of devices.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Device\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/advanced-micro-devices/refs/heads/main/json-schema/rocm-api-device-list-schema.json
tags:
- AI
- Cloud Computing
- GPU
- HPC
- Machine Learning
- Semiconductor
title: DeviceList
---
