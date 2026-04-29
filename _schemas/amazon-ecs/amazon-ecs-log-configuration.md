---
description: ''
layout: schema
name: LogConfiguration
properties_list:
- description: The log driver to use for the container.
  name: logDriver
  type: string
- description: The configuration options to send to the log driver.
  name: options
  type: object
- description: The secrets to pass to the log driver configuration.
  name: secretOptions
  type: array
provider_name: Amazon ECS
provider_slug: amazon-ecs
schema_file: json-schema/amazon-ecs-log-configuration-schema.json
slug: amazon-ecs-log-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LogConfiguration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"logDriver\": {\n      \"type\": \"string\",\n      \"description\": \"The log driver to use for the container.\"\n    },\n    \"options\": {\n      \"type\": \"object\",\n      \"description\": \"The configuration options to send to the log driver.\"\n    },\n    \"secretOptions\": {\n      \"type\": \"array\",\n      \"description\": \"The secrets to pass to the log driver configuration.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/json-schema/amazon-ecs-log-configuration-schema.json
tags:
- Amazon
- Aws
- Containers
- Docker
- Ecs
- Orchestration
title: LogConfiguration
---
