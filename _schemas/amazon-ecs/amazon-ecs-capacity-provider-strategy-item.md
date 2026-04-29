---
description: ''
layout: schema
name: CapacityProviderStrategyItem
properties_list:
- description: The short name of the capacity provider.
  name: capacityProvider
  type: string
- description: The weight value designating the relative percentage of the total number of tasks launched that should use the capacity provider (0-1000).
  name: weight
  type: integer
- description: The number of tasks, at a minimum, to run on the specified capacity provider (0-100000).
  name: base
  type: integer
provider_name: Amazon ECS
provider_slug: amazon-ecs
schema_file: json-schema/amazon-ecs-capacity-provider-strategy-item-schema.json
slug: amazon-ecs-capacity-provider-strategy-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CapacityProviderStrategyItem\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"capacityProvider\": {\n      \"type\": \"string\",\n      \"description\": \"The short name of the capacity provider.\"\n    },\n    \"weight\": {\n      \"type\": \"integer\",\n      \"description\": \"The weight value designating the relative percentage of the total number of tasks launched that should use the capacity provider (0-1000).\"\n    },\n    \"base\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of tasks, at a minimum, to run on the specified capacity provider (0-100000).\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/json-schema/amazon-ecs-capacity-provider-strategy-item-schema.json
tags:
- Amazon
- Aws
- Containers
- Docker
- Ecs
- Orchestration
title: CapacityProviderStrategyItem
---
