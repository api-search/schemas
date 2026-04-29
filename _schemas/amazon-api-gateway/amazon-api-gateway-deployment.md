---
description: ''
layout: schema
name: Deployment
properties_list:
- description: The identifier of the deployment.
  name: id
  type: string
- description: The description for the deployment.
  name: description
  type: string
- description: ''
  name: createdDate
  type: string
- description: ''
  name: apiSummary
  type: object
provider_name: Amazon API Gateway
provider_slug: amazon-api-gateway
schema_file: json-schema/amazon-api-gateway-deployment-schema.json
slug: amazon-api-gateway-deployment
source_filename: amazon-api-gateway-deployment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Deployment\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the deployment.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The description for the deployment.\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"apiSummary\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/json-schema/amazon-api-gateway-deployment-schema.json
tags:
- AWS
- Gateway
- HTTP API
- REST API
- Serverless
- WebSocket
title: Deployment
---
