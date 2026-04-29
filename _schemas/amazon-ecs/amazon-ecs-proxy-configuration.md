---
description: ''
layout: schema
name: ProxyConfiguration
properties_list:
- description: The proxy type. The only supported value is APPMESH.
  name: type
  type: string
- description: The name of the container that will serve as the App Mesh proxy.
  name: containerName
  type: string
- description: ''
  name: properties
  type: array
provider_name: Amazon ECS
provider_slug: amazon-ecs
schema_file: json-schema/amazon-ecs-proxy-configuration-schema.json
slug: amazon-ecs-proxy-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ProxyConfiguration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The proxy type. The only supported value is APPMESH.\"\n    },\n    \"containerName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the container that will serve as the App Mesh proxy.\"\n    },\n    \"properties\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/json-schema/amazon-ecs-proxy-configuration-schema.json
tags:
- Amazon
- Aws
- Containers
- Docker
- Ecs
- Orchestration
title: ProxyConfiguration
---
