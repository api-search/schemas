---
description: A deployed AI model for inference serving.
layout: schema
name: Model
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: framework
  type: string
- description: ''
  name: status
  type: string
- description: Inference endpoint URL.
  name: endpoint
  type: string
provider_name: Advanced Micro Devices
provider_slug: advanced-micro-devices
schema_file: json-schema/cloud-api-model-schema.json
slug: cloud-api-model
source_filename: cloud-api-model-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Model\",\n  \"description\": \"A deployed AI model for inference serving.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"framework\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"vLLM\",\n        \"TGI\",\n        \"TorchServe\",\n        \"Triton\"\n      ]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"deploying\",\n        \"serving\",\n        \"stopped\",\n        \"failed\"\n      ]\n    },\n    \"endpoint\": {\n      \"type\": \"string\",\n      \"description\": \"Inference endpoint URL.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/advanced-micro-devices/refs/heads/main/json-schema/cloud-api-model-schema.json
tags:
- AI
- Cloud Computing
- GPU
- HPC
- Machine Learning
- Semiconductor
title: Model
---
