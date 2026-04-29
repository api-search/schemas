---
description: CreateDeploymentRequest schema from Amazon API Gateway v1 API
layout: schema
name: CreateDeploymentRequest
properties_list:
- description: Name of the stage to deploy to.
  name: stageName
  type: string
- description: Description of the deployment.
  name: description
  type: string
provider_name: Amazon API Gateway
provider_slug: aws-api-gateway
schema_file: json-schema/v1-create-deployment-request-schema.json
slug: v1-create-deployment-request
source_filename: v1-create-deployment-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"stageName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the stage to deploy to.\",\n      \"example\": \"my-resource\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the deployment.\",\n      \"example\": \"A description of this resource.\"\n    }\n  },\n  \"required\": [\n    \"stageName\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v1-create-deployment-request-schema.json\",\n  \"title\": \"CreateDeploymentRequest\",\n  \"description\": \"CreateDeploymentRequest schema from Amazon API Gateway v1 API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v1-create-deployment-request-schema.json
tags:
- API Gateway
- AWS
- Cloud
- REST
- WebSocket
- Serverless
title: CreateDeploymentRequest
---
