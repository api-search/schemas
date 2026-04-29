---
description: ''
layout: schema
name: PlacementStrategy
properties_list:
- description: The type of placement strategy.
  name: type
  type: string
- description: The field to apply the placement strategy against.
  name: field
  type: string
provider_name: Amazon ECS
provider_slug: amazon-ecs
schema_file: json-schema/amazon-ecs-placement-strategy-schema.json
slug: amazon-ecs-placement-strategy
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PlacementStrategy\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of placement strategy.\"\n    },\n    \"field\": {\n      \"type\": \"string\",\n      \"description\": \"The field to apply the placement strategy against.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/json-schema/amazon-ecs-placement-strategy-schema.json
tags:
- Amazon
- Aws
- Containers
- Docker
- Ecs
- Orchestration
title: PlacementStrategy
---
