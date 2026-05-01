---
description: ObservabilityConfiguration schema from AWS App Runner
layout: schema
name: ObservabilityConfiguration
properties_list:
- description: ''
  name: ObservabilityConfigurationArn
  type: string
- description: ''
  name: ObservabilityConfigurationName
  type: string
- description: ''
  name: ObservabilityConfigurationRevision
  type: integer
- description: ''
  name: Latest
  type: boolean
- description: ''
  name: Status
  type: string
- description: ''
  name: TraceConfiguration
  type: object
- description: ''
  name: CreatedAt
  type: string
- description: ''
  name: DeletedAt
  type: string
provider_name: AWS App Runner
provider_slug: aws-app-runner
schema_file: json-schema/app-runner-observability-configuration-schema.json
slug: app-runner-observability-configuration
source_filename: app-runner-observability-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ObservabilityConfigurationArn\": {\n      \"type\": \"string\"\n    },\n    \"ObservabilityConfigurationName\": {\n      \"type\": \"string\"\n    },\n    \"ObservabilityConfigurationRevision\": {\n      \"type\": \"integer\"\n    },\n    \"Latest\": {\n      \"type\": \"boolean\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ACTIVE\",\n        \"INACTIVE\"\n      ]\n    },\n    \"TraceConfiguration\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Vendor\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"AWSXRAY\"\n          ]\n        }\n      }\n    },\n    \"CreatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"DeletedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/json-schema/app-runner-observability-configuration-schema.json\"\
  ,\n  \"title\": \"ObservabilityConfiguration\",\n  \"description\": \"ObservabilityConfiguration schema from AWS App Runner\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/json-schema/app-runner-observability-configuration-schema.json
tags:
- CI/CD
- Containers
- Deployment
- Microservices
- Serverless
title: ObservabilityConfiguration
---
