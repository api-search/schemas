---
description: GPU credit balance and usage.
layout: schema
name: Credits
properties_list:
- description: ''
  name: balance
  type: number
- description: ''
  name: used
  type: number
- description: ''
  name: total
  type: number
- description: ''
  name: currency
  type: string
- description: ''
  name: expiresAt
  type: string
provider_name: Advanced Micro Devices
provider_slug: advanced-micro-devices
schema_file: json-schema/cloud-api-credits-schema.json
slug: cloud-api-credits
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Credits\",\n  \"description\": \"GPU credit balance and usage.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"balance\": {\n      \"type\": \"number\"\n    },\n    \"used\": {\n      \"type\": \"number\"\n    },\n    \"total\": {\n      \"type\": \"number\"\n    },\n    \"currency\": {\n      \"type\": \"string\"\n    },\n    \"expiresAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/advanced-micro-devices/refs/heads/main/json-schema/cloud-api-credits-schema.json
tags:
- AI
- Cloud Computing
- GPU
- HPC
- Machine Learning
- Semiconductor
title: Credits
---
