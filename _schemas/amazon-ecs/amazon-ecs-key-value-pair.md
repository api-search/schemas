---
description: ''
layout: schema
name: KeyValuePair
properties_list:
- description: The name of the key-value pair.
  name: name
  type: string
- description: The value of the key-value pair.
  name: value
  type: string
provider_name: Amazon ECS
provider_slug: amazon-ecs
schema_file: json-schema/amazon-ecs-key-value-pair-schema.json
slug: amazon-ecs-key-value-pair
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"KeyValuePair\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the key-value pair.\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The value of the key-value pair.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/json-schema/amazon-ecs-key-value-pair-schema.json
tags:
- Amazon
- Aws
- Containers
- Docker
- Ecs
- Orchestration
title: KeyValuePair
---
