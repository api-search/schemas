---
description: Deployment schema from Amazon API Gateway v1 API
layout: schema
name: Deployment
properties_list:
- description: Deployment identifier.
  name: id
  type: string
- description: Description of the deployment.
  name: description
  type: string
- description: Timestamp when the deployment was created.
  name: createdDate
  type: string
provider_name: Amazon API Gateway
provider_slug: aws-api-gateway
schema_file: json-schema/v1-deployment-schema.json
slug: v1-deployment
source_filename: v1-deployment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Deployment identifier.\",\n      \"example\": \"abc123\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the deployment.\",\n      \"example\": \"A description of this resource.\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the deployment was created.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v1-deployment-schema.json\",\n  \"title\": \"Deployment\",\n  \"description\": \"Deployment schema from Amazon API Gateway v1 API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v1-deployment-schema.json
tags:
- API Gateway
- AWS
- Cloud
- REST
- WebSocket
- Serverless
title: Deployment
---
