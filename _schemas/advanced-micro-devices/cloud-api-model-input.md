---
description: Request to deploy an AI model.
layout: schema
name: ModelInput
properties_list:
- description: ''
  name: name
  type: string
- description: Hugging Face model ID.
  name: modelId
  type: string
- description: ''
  name: framework
  type: string
- description: ''
  name: gpuType
  type: string
- description: ''
  name: gpuCount
  type: integer
provider_name: Advanced Micro Devices
provider_slug: advanced-micro-devices
schema_file: json-schema/cloud-api-model-input-schema.json
slug: cloud-api-model-input
source_filename: cloud-api-model-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ModelInput\",\n  \"description\": \"Request to deploy an AI model.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"modelId\",\n    \"framework\",\n    \"gpuType\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"modelId\": {\n      \"type\": \"string\",\n      \"description\": \"Hugging Face model ID.\"\n    },\n    \"framework\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"vLLM\",\n        \"TGI\",\n        \"TorchServe\",\n        \"Triton\"\n      ]\n    },\n    \"gpuType\": {\n      \"type\": \"string\"\n    },\n    \"gpuCount\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/advanced-micro-devices/refs/heads/main/json-schema/cloud-api-model-input-schema.json
tags:
- AI
- Cloud Computing
- GPU
- HPC
- Machine Learning
- Semiconductor
title: ModelInput
---
