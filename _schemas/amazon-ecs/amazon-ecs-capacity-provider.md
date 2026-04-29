---
description: ''
layout: schema
name: CapacityProvider
properties_list:
- description: ''
  name: capacityProviderArn
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: updateStatus
  type: string
- description: ''
  name: updateStatusReason
  type: string
- description: ''
  name: tags
  type: array
provider_name: Amazon ECS
provider_slug: amazon-ecs
schema_file: json-schema/amazon-ecs-capacity-provider-schema.json
slug: amazon-ecs-capacity-provider
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CapacityProvider\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"capacityProviderArn\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"updateStatus\": {\n      \"type\": \"string\"\n    },\n    \"updateStatusReason\": {\n      \"type\": \"string\"\n    },\n    \"tags\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/json-schema/amazon-ecs-capacity-provider-schema.json
tags:
- Amazon
- Aws
- Containers
- Docker
- Ecs
- Orchestration
title: CapacityProvider
---
