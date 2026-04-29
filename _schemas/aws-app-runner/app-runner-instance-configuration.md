---
description: InstanceConfiguration schema from AWS App Runner
layout: schema
name: InstanceConfiguration
properties_list:
- description: CPU units (e.g., 1024 for 1 vCPU, 256, 512, 1024, 2048, 4096).
  name: Cpu
  type: string
- description: Memory in MB (e.g., 2048 for 2 GB).
  name: Memory
  type: string
- description: ''
  name: InstanceRoleArn
  type: string
provider_name: AWS App Runner
provider_slug: aws-app-runner
schema_file: json-schema/app-runner-instance-configuration-schema.json
slug: app-runner-instance-configuration
source_filename: app-runner-instance-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Cpu\": {\n      \"type\": \"string\",\n      \"description\": \"CPU units (e.g., 1024 for 1 vCPU, 256, 512, 1024, 2048, 4096).\"\n    },\n    \"Memory\": {\n      \"type\": \"string\",\n      \"description\": \"Memory in MB (e.g., 2048 for 2 GB).\"\n    },\n    \"InstanceRoleArn\": {\n      \"type\": \"string\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/json-schema/app-runner-instance-configuration-schema.json\",\n  \"title\": \"InstanceConfiguration\",\n  \"description\": \"InstanceConfiguration schema from AWS App Runner\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/json-schema/app-runner-instance-configuration-schema.json
tags:
- AWS
- CI/CD
- Containers
- Deployment
- Microservices
- Serverless
title: InstanceConfiguration
---
