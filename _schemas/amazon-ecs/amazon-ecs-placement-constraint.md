---
description: ''
layout: schema
name: PlacementConstraint
properties_list:
- description: The type of placement constraint.
  name: type
  type: string
- description: A cluster query language expression.
  name: expression
  type: string
provider_name: Amazon ECS
provider_slug: amazon-ecs
schema_file: json-schema/amazon-ecs-placement-constraint-schema.json
slug: amazon-ecs-placement-constraint
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PlacementConstraint\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of placement constraint.\"\n    },\n    \"expression\": {\n      \"type\": \"string\",\n      \"description\": \"A cluster query language expression.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/json-schema/amazon-ecs-placement-constraint-schema.json
tags:
- Amazon
- Aws
- Containers
- Docker
- Ecs
- Orchestration
title: PlacementConstraint
---
