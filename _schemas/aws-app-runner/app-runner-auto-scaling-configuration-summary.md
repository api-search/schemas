---
description: AutoScalingConfigurationSummary schema from AWS App Runner
layout: schema
name: AutoScalingConfigurationSummary
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
  name: Status
  type: string
- description: ''
  name: CreatedAt
  type: string
- description: ''
  name: HasAssociatedService
  type: boolean
- description: ''
  name: IsDefault
  type: boolean
provider_name: AWS App Runner
provider_slug: aws-app-runner
schema_file: json-schema/app-runner-auto-scaling-configuration-summary-schema.json
slug: app-runner-auto-scaling-configuration-summary
source_filename: app-runner-auto-scaling-configuration-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"AutoScalingConfigurationArn\": {\n      \"type\": \"string\"\n    },\n    \"AutoScalingConfigurationName\": {\n      \"type\": \"string\"\n    },\n    \"AutoScalingConfigurationRevision\": {\n      \"type\": \"integer\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ACTIVE\",\n        \"INACTIVE\"\n      ]\n    },\n    \"CreatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"HasAssociatedService\": {\n      \"type\": \"boolean\"\n    },\n    \"IsDefault\": {\n      \"type\": \"boolean\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/json-schema/app-runner-auto-scaling-configuration-summary-schema.json\",\n  \"title\": \"AutoScalingConfigurationSummary\",\n  \"description\": \"AutoScalingConfigurationSummary schema from AWS\
  \ App Runner\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/json-schema/app-runner-auto-scaling-configuration-summary-schema.json
tags:
- AWS
- CI/CD
- Containers
- Deployment
- Microservices
- Serverless
title: AutoScalingConfigurationSummary
---
