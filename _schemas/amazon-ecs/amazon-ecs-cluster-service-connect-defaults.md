---
description: ''
layout: schema
name: ClusterServiceConnectDefaults
properties_list:
- description: The namespace name or ARN of the Cloud Map namespace that is used when a service is created without specifying a Service Connect configuration.
  name: namespace
  type: string
provider_name: Amazon ECS
provider_slug: amazon-ecs
schema_file: json-schema/amazon-ecs-cluster-service-connect-defaults-schema.json
slug: amazon-ecs-cluster-service-connect-defaults
source_filename: amazon-ecs-cluster-service-connect-defaults-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ClusterServiceConnectDefaults\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"namespace\": {\n      \"type\": \"string\",\n      \"description\": \"The namespace name or ARN of the Cloud Map namespace that is used when a service is created without specifying a Service Connect configuration.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/json-schema/amazon-ecs-cluster-service-connect-defaults-schema.json
tags:
- Amazon
- Aws
- Containers
- Docker
- Ecs
- Orchestration
title: ClusterServiceConnectDefaults
---
