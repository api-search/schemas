---
description: ''
layout: schema
name: CreateDeploymentRequest
properties_list:
- description: The name of the stage that the deployment is made to. If not specified, a new stage is created with a generated name.
  name: stageName
  type: string
- description: ''
  name: stageDescription
  type: string
- description: A description for the deployment.
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
  name: canarySettings
  type: object
- description: ''
  name: tracingEnabled
  type: boolean
provider_name: Amazon API Gateway
provider_slug: amazon-api-gateway
schema_file: json-schema/amazon-api-gateway-createdeploymentrequest-schema.json
slug: amazon-api-gateway-createdeploymentrequest
source_filename: amazon-api-gateway-createdeploymentrequest-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"CreateDeploymentRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"stageName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the stage that the deployment is made to. If not specified, a new stage is created with a generated name.\"\n    },\n    \"stageDescription\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description for the deployment.\"\n    },\n    \"cacheClusterEnabled\": {\n      \"type\": \"boolean\"\n    },\n    \"cacheClusterSize\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"0.5\",\n        \"1.6\",\n        \"6.1\",\n        \"13.5\",\n        \"28.4\",\n        \"58.2\",\n        \"118\",\n        \"237\"\n      ]\n    },\n    \"variables\": {\n      \"type\": \"object\"\n    },\n    \"canarySettings\": {\n      \"$ref\": \"#/definitions/DeploymentCanarySettings\"\
  \n    },\n    \"tracingEnabled\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/json-schema/amazon-api-gateway-createdeploymentrequest-schema.json
tags:
- Gateway
- HTTP API
- REST API
- Serverless
- WebSocket
title: CreateDeploymentRequest
---
