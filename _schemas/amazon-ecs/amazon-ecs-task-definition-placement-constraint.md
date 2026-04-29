---
description: ''
layout: schema
name: TaskDefinitionPlacementConstraint
properties_list:
- description: The type of constraint.
  name: type
  type: string
- description: A cluster query language expression to apply to the constraint.
  name: expression
  type: string
provider_name: Amazon ECS
provider_slug: amazon-ecs
schema_file: json-schema/amazon-ecs-task-definition-placement-constraint-schema.json
slug: amazon-ecs-task-definition-placement-constraint
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TaskDefinitionPlacementConstraint\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of constraint.\"\n    },\n    \"expression\": {\n      \"type\": \"string\",\n      \"description\": \"A cluster query language expression to apply to the constraint.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/json-schema/amazon-ecs-task-definition-placement-constraint-schema.json
tags:
- Amazon
- Aws
- Containers
- Docker
- Ecs
- Orchestration
title: TaskDefinitionPlacementConstraint
---
