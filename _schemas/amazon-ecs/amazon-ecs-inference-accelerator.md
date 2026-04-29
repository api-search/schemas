---
description: ''
layout: schema
name: InferenceAccelerator
properties_list:
- description: The Elastic Inference accelerator device name.
  name: deviceName
  type: string
- description: The Elastic Inference accelerator type to use.
  name: deviceType
  type: string
provider_name: Amazon ECS
provider_slug: amazon-ecs
schema_file: json-schema/amazon-ecs-inference-accelerator-schema.json
slug: amazon-ecs-inference-accelerator
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InferenceAccelerator\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deviceName\": {\n      \"type\": \"string\",\n      \"description\": \"The Elastic Inference accelerator device name.\"\n    },\n    \"deviceType\": {\n      \"type\": \"string\",\n      \"description\": \"The Elastic Inference accelerator type to use.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/json-schema/amazon-ecs-inference-accelerator-schema.json
tags:
- Amazon
- Aws
- Containers
- Docker
- Ecs
- Orchestration
title: InferenceAccelerator
---
