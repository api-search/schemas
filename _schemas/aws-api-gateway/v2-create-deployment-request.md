---
description: CreateDeploymentRequest schema from Amazon API Gateway v2 API
layout: schema
name: CreateDeploymentRequest
properties_list:
- description: Stage to deploy to.
  name: StageName
  type: string
- description: Description of the deployment.
  name: Description
  type: string
provider_name: Amazon API Gateway
provider_slug: aws-api-gateway
schema_file: json-schema/v2-create-deployment-request-schema.json
slug: v2-create-deployment-request
source_filename: v2-create-deployment-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"StageName\": {\n      \"type\": \"string\",\n      \"description\": \"Stage to deploy to.\",\n      \"example\": \"my-resource\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the deployment.\",\n      \"example\": \"A description of this resource.\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v2-create-deployment-request-schema.json\",\n  \"title\": \"CreateDeploymentRequest\",\n  \"description\": \"CreateDeploymentRequest schema from Amazon API Gateway v2 API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v2-create-deployment-request-schema.json
tags:
- API Gateway
- Cloud
- REST
- WebSocket
- Serverless
title: CreateDeploymentRequest
---
