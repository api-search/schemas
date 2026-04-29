---
description: ''
layout: schema
name: RuntimePlatform
properties_list:
- description: The CPU architecture.
  name: cpuArchitecture
  type: string
- description: The operating system.
  name: operatingSystemFamily
  type: string
provider_name: Amazon ECS
provider_slug: amazon-ecs
schema_file: json-schema/amazon-ecs-runtime-platform-schema.json
slug: amazon-ecs-runtime-platform
source_filename: amazon-ecs-runtime-platform-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RuntimePlatform\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cpuArchitecture\": {\n      \"type\": \"string\",\n      \"description\": \"The CPU architecture.\"\n    },\n    \"operatingSystemFamily\": {\n      \"type\": \"string\",\n      \"description\": \"The operating system.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/json-schema/amazon-ecs-runtime-platform-schema.json
tags:
- Amazon
- Aws
- Containers
- Docker
- Ecs
- Orchestration
title: RuntimePlatform
---
