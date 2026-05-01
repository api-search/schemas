---
description: Deployment schema from Amazon API Gateway v2 API
layout: schema
name: Deployment
properties_list:
- description: Deployment identifier.
  name: DeploymentId
  type: string
- description: Description of the deployment.
  name: Description
  type: string
- description: Status of the deployment (PENDING, FAILED, DEPLOYED).
  name: DeploymentStatus
  type: string
- description: Timestamp when the deployment was created.
  name: CreatedDate
  type: string
provider_name: Amazon API Gateway
provider_slug: aws-api-gateway
schema_file: json-schema/v2-deployment-schema.json
slug: v2-deployment
source_filename: v2-deployment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"DeploymentId\": {\n      \"type\": \"string\",\n      \"description\": \"Deployment identifier.\",\n      \"example\": \"abc123\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the deployment.\",\n      \"example\": \"A description of this resource.\"\n    },\n    \"DeploymentStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Status of the deployment (PENDING, FAILED, DEPLOYED).\",\n      \"example\": \"ACTIVE\"\n    },\n    \"CreatedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the deployment was created.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v2-deployment-schema.json\",\n  \"title\": \"Deployment\"\
  ,\n  \"description\": \"Deployment schema from Amazon API Gateway v2 API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v2-deployment-schema.json
tags:
- API Gateway
- Cloud
- REST
- WebSocket
- Serverless
title: Deployment
---
