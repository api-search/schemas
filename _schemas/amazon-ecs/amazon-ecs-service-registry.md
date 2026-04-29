---
description: ''
layout: schema
name: ServiceRegistry
properties_list:
- description: The ARN of the Cloud Map service registry.
  name: registryArn
  type: string
- description: ''
  name: port
  type: integer
- description: ''
  name: containerName
  type: string
- description: ''
  name: containerPort
  type: integer
provider_name: Amazon ECS
provider_slug: amazon-ecs
schema_file: json-schema/amazon-ecs-service-registry-schema.json
slug: amazon-ecs-service-registry
source_filename: amazon-ecs-service-registry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ServiceRegistry\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"registryArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the Cloud Map service registry.\"\n    },\n    \"port\": {\n      \"type\": \"integer\"\n    },\n    \"containerName\": {\n      \"type\": \"string\"\n    },\n    \"containerPort\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/json-schema/amazon-ecs-service-registry-schema.json
tags:
- Amazon
- Aws
- Containers
- Docker
- Ecs
- Orchestration
title: ServiceRegistry
---
