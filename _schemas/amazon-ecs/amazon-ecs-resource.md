---
description: ''
layout: schema
name: Resource
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: doubleValue
  type: number
- description: ''
  name: longValue
  type: integer
- description: ''
  name: integerValue
  type: integer
- description: ''
  name: stringSetValue
  type: array
provider_name: Amazon ECS
provider_slug: amazon-ecs
schema_file: json-schema/amazon-ecs-resource-schema.json
slug: amazon-ecs-resource
source_filename: amazon-ecs-resource-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Resource\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"doubleValue\": {\n      \"type\": \"number\"\n    },\n    \"longValue\": {\n      \"type\": \"integer\"\n    },\n    \"integerValue\": {\n      \"type\": \"integer\"\n    },\n    \"stringSetValue\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/json-schema/amazon-ecs-resource-schema.json
tags:
- Amazon
- Aws
- Containers
- Docker
- Ecs
- Orchestration
title: Resource
---
