---
description: ''
layout: schema
name: ServiceConnectConfiguration
properties_list:
- description: Whether Service Connect is enabled for this service.
  name: enabled
  type: boolean
- description: The namespace name or ARN of the Cloud Map namespace for the service.
  name: namespace
  type: string
- description: ''
  name: services
  type: array
- description: ''
  name: logConfiguration
  type: object
provider_name: Amazon ECS
provider_slug: amazon-ecs
schema_file: json-schema/amazon-ecs-service-connect-configuration-schema.json
slug: amazon-ecs-service-connect-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ServiceConnectConfiguration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether Service Connect is enabled for this service.\"\n    },\n    \"namespace\": {\n      \"type\": \"string\",\n      \"description\": \"The namespace name or ARN of the Cloud Map namespace for the service.\"\n    },\n    \"services\": {\n      \"type\": \"array\"\n    },\n    \"logConfiguration\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/json-schema/amazon-ecs-service-connect-configuration-schema.json
tags:
- Amazon
- Aws
- Containers
- Docker
- Ecs
- Orchestration
title: ServiceConnectConfiguration
---
