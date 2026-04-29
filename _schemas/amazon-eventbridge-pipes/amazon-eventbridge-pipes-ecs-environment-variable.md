---
description: The environment variables to send to the container. You can add new environment variables, which are added to the container at launch, or you can override the existing environment variables from the Docker image or the task definition. You must also specify a container name.
layout: schema
name: EcsEnvironmentVariable
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: value
  type: object
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-ecs-environment-variable-schema.json
slug: amazon-eventbridge-pipes-ecs-environment-variable
source_filename: amazon-eventbridge-pipes-ecs-environment-variable-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-ecs-environment-variable-schema.json\",\n  \"title\": \"EcsEnvironmentVariable\",\n  \"description\": \"The environment variables to send to the container. You can add new environment variables, which are added to the container at launch, or you can override the existing environment variables from the Docker image or the task definition. You must also specify a container name.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the key-value pair. For environment variables, this is the name of the environment variable.\"\n        }\n      ]\n    },\n    \"value\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The value of the key-value pair. For environment variables, this is the value of the environment variable.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-ecs-environment-variable-schema.json
tags:
- Amazon Web Services
- AWS
- Event-Driven
- Integration
- Messaging
- Serverless
title: EcsEnvironmentVariable
---
