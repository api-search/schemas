---
description: CreateIntegrationRequest schema from Amazon API Gateway v2 API
layout: schema
name: CreateIntegrationRequest
properties_list:
- description: Type of integration.
  name: IntegrationType
  type: string
- description: Integration target URI.
  name: IntegrationUri
  type: string
- description: Payload format version.
  name: PayloadFormatVersion
  type: string
provider_name: Amazon API Gateway
provider_slug: aws-api-gateway
schema_file: json-schema/v2-create-integration-request-schema.json
slug: v2-create-integration-request
source_filename: v2-create-integration-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"IntegrationType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"AWS\",\n        \"AWS_PROXY\",\n        \"HTTP\",\n        \"HTTP_PROXY\",\n        \"MOCK\"\n      ],\n      \"description\": \"Type of integration.\",\n      \"example\": \"AWS\"\n    },\n    \"IntegrationUri\": {\n      \"type\": \"string\",\n      \"description\": \"Integration target URI.\",\n      \"example\": \"https://example.com/resource/123\"\n    },\n    \"PayloadFormatVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Payload format version.\",\n      \"example\": \"1.0\"\n    }\n  },\n  \"required\": [\n    \"IntegrationType\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v2-create-integration-request-schema.json\",\n  \"title\": \"CreateIntegrationRequest\",\n  \"description\": \"\
  CreateIntegrationRequest schema from Amazon API Gateway v2 API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v2-create-integration-request-schema.json
tags:
- API Gateway
- AWS
- Cloud
- REST
- WebSocket
- Serverless
title: CreateIntegrationRequest
---
