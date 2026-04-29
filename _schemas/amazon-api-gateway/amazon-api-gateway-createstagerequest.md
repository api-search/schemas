---
description: ''
layout: schema
name: CreateStageRequest
properties_list:
- description: The name for the stage.
  name: stageName
  type: string
- description: The identifier of the deployment.
  name: deploymentId
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: cacheClusterEnabled
  type: boolean
- description: ''
  name: cacheClusterSize
  type: string
- description: ''
  name: variables
  type: object
- description: ''
  name: documentationVersion
  type: string
- description: ''
  name: canarySettings
  type: object
- description: ''
  name: tracingEnabled
  type: boolean
- description: ''
  name: tags
  type: object
provider_name: Amazon API Gateway
provider_slug: amazon-api-gateway
schema_file: json-schema/amazon-api-gateway-createstagerequest-schema.json
slug: amazon-api-gateway-createstagerequest
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"CreateStageRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"stageName\": {\n      \"type\": \"string\",\n      \"description\": \"The name for the stage.\"\n    },\n    \"deploymentId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the deployment.\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"cacheClusterEnabled\": {\n      \"type\": \"boolean\"\n    },\n    \"cacheClusterSize\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"0.5\",\n        \"1.6\",\n        \"6.1\",\n        \"13.5\",\n        \"28.4\",\n        \"58.2\",\n        \"118\",\n        \"237\"\n      ]\n    },\n    \"variables\": {\n      \"type\": \"object\"\n    },\n    \"documentationVersion\": {\n      \"type\": \"string\"\n    },\n    \"canarySettings\": {\n      \"$ref\": \"#/definitions/CanarySettings\"\n    },\n    \"tracingEnabled\":\
  \ {\n      \"type\": \"boolean\"\n    },\n    \"tags\": {\n      \"type\": \"object\"\n    }\n  },\n  \"required\": [\n    \"stageName\",\n    \"deploymentId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/json-schema/amazon-api-gateway-createstagerequest-schema.json
tags:
- AWS
- Gateway
- HTTP API
- REST API
- Serverless
- WebSocket
title: CreateStageRequest
---
