---
description: ''
layout: schema
name: ClusterSetting
properties_list:
- description: The name of the cluster setting (e.g., containerInsights).
  name: name
  type: string
- description: The value of the cluster setting.
  name: value
  type: string
provider_name: Amazon ECS
provider_slug: amazon-ecs
schema_file: json-schema/amazon-ecs-cluster-setting-schema.json
slug: amazon-ecs-cluster-setting
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ClusterSetting\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the cluster setting (e.g., containerInsights).\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The value of the cluster setting.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/json-schema/amazon-ecs-cluster-setting-schema.json
tags:
- Amazon
- Aws
- Containers
- Docker
- Ecs
- Orchestration
title: ClusterSetting
---
