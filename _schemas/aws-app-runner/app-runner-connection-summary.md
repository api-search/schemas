---
description: ConnectionSummary schema from AWS App Runner
layout: schema
name: ConnectionSummary
properties_list:
- description: ''
  name: ConnectionName
  type: string
- description: ''
  name: ConnectionArn
  type: string
- description: ''
  name: ProviderType
  type: string
- description: ''
  name: Status
  type: string
- description: ''
  name: CreatedAt
  type: string
provider_name: AWS App Runner
provider_slug: aws-app-runner
schema_file: json-schema/app-runner-connection-summary-schema.json
slug: app-runner-connection-summary
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConnectionName\": {\n      \"type\": \"string\"\n    },\n    \"ConnectionArn\": {\n      \"type\": \"string\"\n    },\n    \"ProviderType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"GITHUB\",\n        \"BITBUCKET\"\n      ]\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PENDING_HANDSHAKE\",\n        \"AVAILABLE\",\n        \"ERROR\",\n        \"DELETED\"\n      ]\n    },\n    \"CreatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/json-schema/app-runner-connection-summary-schema.json\",\n  \"title\": \"ConnectionSummary\",\n  \"description\": \"ConnectionSummary schema from AWS App Runner\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/json-schema/app-runner-connection-summary-schema.json
tags:
- AWS
- CI/CD
- Containers
- Deployment
- Microservices
- Serverless
title: ConnectionSummary
---
