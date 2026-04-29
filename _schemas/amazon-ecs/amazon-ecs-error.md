---
description: ''
layout: schema
name: Error
properties_list:
- description: The error type.
  name: __type
  type: string
- description: A human-readable description of the error.
  name: message
  type: string
provider_name: Amazon ECS
provider_slug: amazon-ecs
schema_file: json-schema/amazon-ecs-error-schema.json
slug: amazon-ecs-error
source_filename: amazon-ecs-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"__type\": {\n      \"type\": \"string\",\n      \"description\": \"The error type.\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable description of the error.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/json-schema/amazon-ecs-error-schema.json
tags:
- Amazon
- Aws
- Containers
- Docker
- Ecs
- Orchestration
title: Error
---
