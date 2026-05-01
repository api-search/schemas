---
description: ServiceSummary schema from AWS App Runner
layout: schema
name: ServiceSummary
properties_list:
- description: ''
  name: ServiceName
  type: string
- description: ''
  name: ServiceId
  type: string
- description: ''
  name: ServiceArn
  type: string
- description: ''
  name: ServiceUrl
  type: string
- description: ''
  name: CreatedAt
  type: string
- description: ''
  name: UpdatedAt
  type: string
- description: ''
  name: Status
  type: string
provider_name: AWS App Runner
provider_slug: aws-app-runner
schema_file: json-schema/app-runner-service-summary-schema.json
slug: app-runner-service-summary
source_filename: app-runner-service-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ServiceName\": {\n      \"type\": \"string\"\n    },\n    \"ServiceId\": {\n      \"type\": \"string\"\n    },\n    \"ServiceArn\": {\n      \"type\": \"string\"\n    },\n    \"ServiceUrl\": {\n      \"type\": \"string\"\n    },\n    \"CreatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"UpdatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CREATE_FAILED\",\n        \"RUNNING\",\n        \"DELETED\",\n        \"DELETE_FAILED\",\n        \"PAUSED\",\n        \"OPERATION_IN_PROGRESS\"\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/json-schema/app-runner-service-summary-schema.json\",\n  \"title\": \"ServiceSummary\",\n  \"description\": \"ServiceSummary\
  \ schema from AWS App Runner\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/json-schema/app-runner-service-summary-schema.json
tags:
- CI/CD
- Containers
- Deployment
- Microservices
- Serverless
title: ServiceSummary
---
