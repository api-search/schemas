---
description: ''
layout: schema
name: DeploymentCanarySettings
properties_list:
- description: ''
  name: percentTraffic
  type: number
- description: ''
  name: stageVariableOverrides
  type: object
- description: ''
  name: useStageCache
  type: boolean
provider_name: Amazon API Gateway
provider_slug: amazon-api-gateway
schema_file: json-schema/amazon-api-gateway-deploymentcanarysettings-schema.json
slug: amazon-api-gateway-deploymentcanarysettings
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"DeploymentCanarySettings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"percentTraffic\": {\n      \"type\": \"number\"\n    },\n    \"stageVariableOverrides\": {\n      \"type\": \"object\"\n    },\n    \"useStageCache\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/json-schema/amazon-api-gateway-deploymentcanarysettings-schema.json
tags:
- AWS
- Gateway
- HTTP API
- REST API
- Serverless
- WebSocket
title: DeploymentCanarySettings
---
