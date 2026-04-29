---
description: ''
layout: schema
name: CanarySettings
properties_list:
- description: The percent of traffic the canary deployment receives.
  name: percentTraffic
  type: number
- description: ''
  name: deploymentId
  type: string
- description: ''
  name: stageVariableOverrides
  type: object
- description: ''
  name: useStageCache
  type: boolean
provider_name: Amazon API Gateway
provider_slug: amazon-api-gateway
schema_file: json-schema/amazon-api-gateway-canarysettings-schema.json
slug: amazon-api-gateway-canarysettings
source_filename: amazon-api-gateway-canarysettings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"CanarySettings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"percentTraffic\": {\n      \"type\": \"number\",\n      \"description\": \"The percent of traffic the canary deployment receives.\"\n    },\n    \"deploymentId\": {\n      \"type\": \"string\"\n    },\n    \"stageVariableOverrides\": {\n      \"type\": \"object\"\n    },\n    \"useStageCache\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/json-schema/amazon-api-gateway-canarysettings-schema.json
tags:
- AWS
- Gateway
- HTTP API
- REST API
- Serverless
- WebSocket
title: CanarySettings
---
