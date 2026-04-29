---
description: ''
layout: schema
name: Tag
properties_list:
- description: The tag key (up to 128 characters).
  name: key
  type: string
- description: The tag value (up to 256 characters).
  name: value
  type: string
provider_name: Amazon ECS
provider_slug: amazon-ecs
schema_file: json-schema/amazon-ecs-tag-schema.json
slug: amazon-ecs-tag
source_filename: amazon-ecs-tag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Tag\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The tag key (up to 128 characters).\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The tag value (up to 256 characters).\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/json-schema/amazon-ecs-tag-schema.json
tags:
- Amazon
- Aws
- Containers
- Docker
- Ecs
- Orchestration
title: Tag
---
