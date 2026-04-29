---
description: ROCm platform version information.
layout: schema
name: RocmVersion
properties_list:
- description: ''
  name: rocmVersion
  type: string
- description: ''
  name: hipVersion
  type: string
- description: ''
  name: driverVersion
  type: string
- description: ''
  name: kernelVersion
  type: string
provider_name: Advanced Micro Devices
provider_slug: advanced-micro-devices
schema_file: json-schema/rocm-api-rocm-version-schema.json
slug: rocm-api-rocm-version
source_filename: rocm-api-rocm-version-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RocmVersion\",\n  \"description\": \"ROCm platform version information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"rocmVersion\": {\n      \"type\": \"string\"\n    },\n    \"hipVersion\": {\n      \"type\": \"string\"\n    },\n    \"driverVersion\": {\n      \"type\": \"string\"\n    },\n    \"kernelVersion\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/advanced-micro-devices/refs/heads/main/json-schema/rocm-api-rocm-version-schema.json
tags:
- AI
- Cloud Computing
- GPU
- HPC
- Machine Learning
- Semiconductor
title: RocmVersion
---
