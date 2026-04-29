---
description: ''
layout: schema
name: Attachment
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: details
  type: array
provider_name: Amazon ECS
provider_slug: amazon-ecs
schema_file: json-schema/amazon-ecs-attachment-schema.json
slug: amazon-ecs-attachment
source_filename: amazon-ecs-attachment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Attachment\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"details\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/json-schema/amazon-ecs-attachment-schema.json
tags:
- Amazon
- Aws
- Containers
- Docker
- Ecs
- Orchestration
title: Attachment
---
