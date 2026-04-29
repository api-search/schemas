---
description: Request to create a GPU compute instance.
layout: schema
name: InstanceInput
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: gpuType
  type: string
- description: ''
  name: gpuCount
  type: integer
- description: ''
  name: imageId
  type: string
- description: ''
  name: region
  type: string
provider_name: Advanced Micro Devices
provider_slug: advanced-micro-devices
schema_file: json-schema/cloud-api-instance-input-schema.json
slug: cloud-api-instance-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InstanceInput\",\n  \"description\": \"Request to create a GPU compute instance.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"gpuType\",\n    \"gpuCount\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"gpuType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"mi300x\",\n        \"mi250\",\n        \"mi210\"\n      ]\n    },\n    \"gpuCount\": {\n      \"type\": \"integer\"\n    },\n    \"imageId\": {\n      \"type\": \"string\"\n    },\n    \"region\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/advanced-micro-devices/refs/heads/main/json-schema/cloud-api-instance-input-schema.json
tags:
- AI
- Cloud Computing
- GPU
- HPC
- Machine Learning
- Semiconductor
title: InstanceInput
---
