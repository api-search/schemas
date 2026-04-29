---
description: ''
layout: schema
name: Failure
properties_list:
- description: The ARN of the failed resource.
  name: arn
  type: string
- description: The reason for the failure.
  name: reason
  type: string
- description: The details of the failure.
  name: detail
  type: string
provider_name: Amazon ECS
provider_slug: amazon-ecs
schema_file: json-schema/amazon-ecs-failure-schema.json
slug: amazon-ecs-failure
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Failure\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the failed resource.\"\n    },\n    \"reason\": {\n      \"type\": \"string\",\n      \"description\": \"The reason for the failure.\"\n    },\n    \"detail\": {\n      \"type\": \"string\",\n      \"description\": \"The details of the failure.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/json-schema/amazon-ecs-failure-schema.json
tags:
- Amazon
- Aws
- Containers
- Docker
- Ecs
- Orchestration
title: Failure
---
