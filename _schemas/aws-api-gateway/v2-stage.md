---
description: Stage schema from Amazon API Gateway v2 API
layout: schema
name: Stage
properties_list:
- description: Name of the stage.
  name: StageName
  type: string
- description: Deployment identifier.
  name: DeploymentId
  type: string
- description: Description of the stage.
  name: Description
  type: string
- description: Whether updates auto-deploy to this stage.
  name: AutoDeploy
  type: boolean
provider_name: Amazon API Gateway
provider_slug: aws-api-gateway
schema_file: json-schema/v2-stage-schema.json
slug: v2-stage
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"StageName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the stage.\",\n      \"example\": \"my-resource\"\n    },\n    \"DeploymentId\": {\n      \"type\": \"string\",\n      \"description\": \"Deployment identifier.\",\n      \"example\": \"abc123\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the stage.\",\n      \"example\": \"A description of this resource.\"\n    },\n    \"AutoDeploy\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether updates auto-deploy to this stage.\",\n      \"example\": true\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v2-stage-schema.json\",\n  \"title\": \"Stage\",\n  \"description\": \"Stage schema from Amazon API Gateway v2 API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v2-stage-schema.json
tags:
- API Gateway
- AWS
- Cloud
- REST
- WebSocket
- Serverless
title: Stage
---
