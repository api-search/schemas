---
description: The network configuration for a task or service.
layout: schema
name: NetworkConfiguration
properties_list:
- description: ''
  name: awsvpcConfiguration
  type: object
provider_name: Amazon ECS
provider_slug: amazon-ecs
schema_file: json-schema/amazon-ecs-network-configuration-schema.json
slug: amazon-ecs-network-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NetworkConfiguration\",\n  \"type\": \"object\",\n  \"description\": \"The network configuration for a task or service.\",\n  \"properties\": {\n    \"awsvpcConfiguration\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/json-schema/amazon-ecs-network-configuration-schema.json
tags:
- Amazon
- Aws
- Containers
- Docker
- Ecs
- Orchestration
title: NetworkConfiguration
---
