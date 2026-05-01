---
description: Deployments schema from Amazon API Gateway v2 API
layout: schema
name: Deployments
properties_list:
- description: ''
  name: Items
  type: array
provider_name: Amazon API Gateway
provider_slug: aws-api-gateway
schema_file: json-schema/v2-deployments-schema.json
slug: v2-deployments
source_filename: v2-deployments-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Items\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"DeploymentId\": {\n            \"type\": \"string\",\n            \"description\": \"Deployment identifier.\",\n            \"example\": \"abc123\"\n          },\n          \"Description\": {\n            \"type\": \"string\",\n            \"description\": \"Description of the deployment.\",\n            \"example\": \"A description of this resource.\"\n          },\n          \"DeploymentStatus\": {\n            \"type\": \"string\",\n            \"description\": \"Status of the deployment (PENDING, FAILED, DEPLOYED).\",\n            \"example\": \"ACTIVE\"\n          },\n          \"CreatedDate\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"Timestamp when the deployment was created.\",\n            \"example\": \"2025-03-15T14:30:00Z\"\
  \n          }\n        }\n      },\n      \"example\": [\n        \"example-value\"\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v2-deployments-schema.json\",\n  \"title\": \"Deployments\",\n  \"description\": \"Deployments schema from Amazon API Gateway v2 API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v2-deployments-schema.json
tags:
- API Gateway
- Cloud
- REST
- WebSocket
- Serverless
title: Deployments
---
