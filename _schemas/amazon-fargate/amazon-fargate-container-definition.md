---
description: Container definition for a task
layout: schema
name: ContainerDefinition
properties_list:
- description: Container name
  name: name
  type: string
- description: Docker image
  name: image
  type: string
- description: Whether container is essential
  name: essential
  type: boolean
- description: CPU units for the container
  name: cpu
  type: integer
- description: Memory limit in MiB
  name: memory
  type: integer
- description: Environment variables
  name: environment
  type: array
- description: Port mappings
  name: portMappings
  type: array
- description: ''
  name: logConfiguration
  type: object
provider_name: Amazon Fargate
provider_slug: amazon-fargate
schema_file: json-schema/amazon-fargate-container-definition-schema.json
slug: amazon-fargate-container-definition
source_filename: amazon-fargate-container-definition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-fargate/refs/heads/main/json-schema/amazon-fargate-container-definition-schema.json\",\n  \"title\": \"ContainerDefinition\",\n  \"description\": \"Container definition for a task\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Container name\",\n      \"example\": \"my-container\"\n    },\n    \"image\": {\n      \"type\": \"string\",\n      \"description\": \"Docker image\",\n      \"example\": \"nginx:latest\"\n    },\n    \"essential\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether container is essential\",\n      \"example\": true\n    },\n    \"cpu\": {\n      \"type\": \"integer\",\n      \"description\": \"CPU units for the container\",\n      \"example\": 256\n    },\n    \"memory\": {\n      \"type\": \"integer\",\n      \"description\"\
  : \"Memory limit in MiB\",\n      \"example\": 512\n    },\n    \"environment\": {\n      \"type\": \"array\",\n      \"description\": \"Environment variables\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/KeyValuePair\"\n      }\n    },\n    \"portMappings\": {\n      \"type\": \"array\",\n      \"description\": \"Port mappings\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/PortMapping\"\n      }\n    },\n    \"logConfiguration\": {\n      \"$ref\": \"#/components/schemas/LogConfiguration\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-fargate/refs/heads/main/json-schema/amazon-fargate-container-definition-schema.json
tags:
- Compute
- Containers
- ECS
- EKS
- Microservices
- Serverless
title: ContainerDefinition
---
