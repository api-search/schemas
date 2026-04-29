---
description: An AMD GPU compute instance.
layout: schema
name: Instance
properties_list:
- description: Instance identifier.
  name: id
  type: string
- description: Instance display name.
  name: name
  type: string
- description: GPU hardware type.
  name: gpuType
  type: string
- description: Number of GPUs.
  name: gpuCount
  type: integer
- description: Instance status.
  name: status
  type: string
- description: Deployment region.
  name: region
  type: string
- description: ROCm image.
  name: imageId
  type: string
- description: Creation timestamp.
  name: createdAt
  type: string
provider_name: Advanced Micro Devices
provider_slug: advanced-micro-devices
schema_file: json-schema/cloud-api-instance-schema.json
slug: cloud-api-instance
source_filename: cloud-api-instance-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Instance\",\n  \"description\": \"An AMD GPU compute instance.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Instance identifier.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Instance display name.\"\n    },\n    \"gpuType\": {\n      \"type\": \"string\",\n      \"description\": \"GPU hardware type.\",\n      \"enum\": [\n        \"mi300x\",\n        \"mi250\",\n        \"mi210\",\n        \"rx7900xtx\"\n      ]\n    },\n    \"gpuCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of GPUs.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Instance status.\",\n      \"enum\": [\n        \"running\",\n        \"stopped\",\n        \"pending\",\n        \"terminated\"\n      ]\n    },\n    \"region\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Deployment region.\"\n    },\n    \"imageId\": {\n      \"type\": \"string\",\n      \"description\": \"ROCm image.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Creation timestamp.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/advanced-micro-devices/refs/heads/main/json-schema/cloud-api-instance-schema.json
tags:
- AI
- Cloud Computing
- GPU
- HPC
- Machine Learning
- Semiconductor
title: Instance
---
