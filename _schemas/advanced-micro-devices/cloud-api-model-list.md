---
description: List of deployed AI models.
layout: schema
name: ModelList
properties_list:
- description: Array of models.
  name: models
  type: array
provider_name: Advanced Micro Devices
provider_slug: advanced-micro-devices
schema_file: json-schema/cloud-api-model-list-schema.json
slug: cloud-api-model-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ModelList\",\n  \"description\": \"List of deployed AI models.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"models\": {\n      \"type\": \"array\",\n      \"description\": \"Array of models.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Model\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/advanced-micro-devices/refs/heads/main/json-schema/cloud-api-model-list-schema.json
tags:
- AI
- Cloud Computing
- GPU
- HPC
- Machine Learning
- Semiconductor
title: ModelList
---
