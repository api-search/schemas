---
description: AutoScalingConfiguration schema from AWS App Runner
layout: schema
name: AutoScalingConfiguration
properties_list:
- description: ''
  name: AutoScalingConfigurationArn
  type: string
- description: ''
  name: AutoScalingConfigurationName
  type: string
- description: ''
  name: AutoScalingConfigurationRevision
  type: integer
- description: ''
  name: Latest
  type: boolean
- description: ''
  name: Status
  type: string
- description: ''
  name: MaxConcurrency
  type: integer
- description: ''
  name: MinSize
  type: integer
- description: ''
  name: MaxSize
  type: integer
- description: ''
  name: CreatedAt
  type: string
- description: ''
  name: DeletedAt
  type: string
- description: ''
  name: HasAssociatedService
  type: boolean
- description: ''
  name: IsDefault
  type: boolean
provider_name: AWS App Runner
provider_slug: aws-app-runner
schema_file: json-schema/app-runner-auto-scaling-configuration-schema.json
slug: app-runner-auto-scaling-configuration
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"AutoScalingConfigurationArn\": {\n      \"type\": \"string\"\n    },\n    \"AutoScalingConfigurationName\": {\n      \"type\": \"string\"\n    },\n    \"AutoScalingConfigurationRevision\": {\n      \"type\": \"integer\"\n    },\n    \"Latest\": {\n      \"type\": \"boolean\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ACTIVE\",\n        \"INACTIVE\"\n      ]\n    },\n    \"MaxConcurrency\": {\n      \"type\": \"integer\"\n    },\n    \"MinSize\": {\n      \"type\": \"integer\"\n    },\n    \"MaxSize\": {\n      \"type\": \"integer\"\n    },\n    \"CreatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"DeletedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"HasAssociatedService\": {\n      \"type\": \"boolean\"\n    },\n    \"IsDefault\": {\n      \"type\": \"boolean\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/json-schema/app-runner-auto-scaling-configuration-schema.json\",\n  \"title\": \"AutoScalingConfiguration\",\n  \"description\": \"AutoScalingConfiguration schema from AWS App Runner\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/json-schema/app-runner-auto-scaling-configuration-schema.json
tags:
- AWS
- CI/CD
- Containers
- Deployment
- Microservices
- Serverless
title: AutoScalingConfiguration
---
