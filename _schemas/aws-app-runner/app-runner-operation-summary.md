---
description: OperationSummary schema from AWS App Runner
layout: schema
name: OperationSummary
properties_list:
- description: ''
  name: Id
  type: string
- description: ''
  name: Type
  type: string
- description: ''
  name: Status
  type: string
- description: ''
  name: TargetArn
  type: string
- description: ''
  name: StartedAt
  type: string
- description: ''
  name: EndedAt
  type: string
- description: ''
  name: UpdatedAt
  type: string
provider_name: AWS App Runner
provider_slug: aws-app-runner
schema_file: json-schema/app-runner-operation-summary-schema.json
slug: app-runner-operation-summary
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\"\n    },\n    \"Type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CREATE_SERVICE\",\n        \"START_DEPLOYMENT\",\n        \"PAUSE_SERVICE\",\n        \"RESUME_SERVICE\",\n        \"DELETE_SERVICE\",\n        \"UPDATE_SERVICE\"\n      ]\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PENDING\",\n        \"IN_PROGRESS\",\n        \"FAILED\",\n        \"SUCCEEDED\",\n        \"ROLLBACK_IN_PROGRESS\",\n        \"ROLLBACK_FAILED\",\n        \"ROLLBACK_SUCCEEDED\"\n      ]\n    },\n    \"TargetArn\": {\n      \"type\": \"string\"\n    },\n    \"StartedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"EndedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"UpdatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/json-schema/app-runner-operation-summary-schema.json\",\n  \"title\": \"OperationSummary\",\n  \"description\": \"OperationSummary schema from AWS App Runner\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/json-schema/app-runner-operation-summary-schema.json
tags:
- AWS
- CI/CD
- Containers
- Deployment
- Microservices
- Serverless
title: OperationSummary
---
