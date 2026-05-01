---
description: CreateStageRequest schema from Amazon API Gateway v2 API
layout: schema
name: CreateStageRequest
properties_list:
- description: Name of the stage.
  name: StageName
  type: string
- description: Deployment identifier.
  name: DeploymentId
  type: string
- description: Whether to enable auto-deploy.
  name: AutoDeploy
  type: boolean
provider_name: Amazon API Gateway
provider_slug: aws-api-gateway
schema_file: json-schema/v2-create-stage-request-schema.json
slug: v2-create-stage-request
source_filename: v2-create-stage-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"StageName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the stage.\",\n      \"example\": \"my-resource\"\n    },\n    \"DeploymentId\": {\n      \"type\": \"string\",\n      \"description\": \"Deployment identifier.\",\n      \"example\": \"abc123\"\n    },\n    \"AutoDeploy\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to enable auto-deploy.\",\n      \"example\": true\n    }\n  },\n  \"required\": [\n    \"StageName\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v2-create-stage-request-schema.json\",\n  \"title\": \"CreateStageRequest\",\n  \"description\": \"CreateStageRequest schema from Amazon API Gateway v2 API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v2-create-stage-request-schema.json
tags:
- API Gateway
- Cloud
- REST
- WebSocket
- Serverless
title: CreateStageRequest
---
