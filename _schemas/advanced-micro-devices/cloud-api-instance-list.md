---
description: List of GPU compute instances.
layout: schema
name: InstanceList
properties_list:
- description: Array of instances.
  name: instances
  type: array
- description: Total count.
  name: total
  type: integer
provider_name: Advanced Micro Devices
provider_slug: advanced-micro-devices
schema_file: json-schema/cloud-api-instance-list-schema.json
slug: cloud-api-instance-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InstanceList\",\n  \"description\": \"List of GPU compute instances.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"instances\": {\n      \"type\": \"array\",\n      \"description\": \"Array of instances.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Instance\"\n      }\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total count.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/advanced-micro-devices/refs/heads/main/json-schema/cloud-api-instance-list-schema.json
tags:
- AI
- Cloud Computing
- GPU
- HPC
- Machine Learning
- Semiconductor
title: InstanceList
---
