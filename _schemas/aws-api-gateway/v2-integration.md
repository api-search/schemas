---
description: Integration schema from Amazon API Gateway v2 API
layout: schema
name: Integration
properties_list:
- description: Integration identifier.
  name: IntegrationId
  type: string
- description: Type of integration (AWS_PROXY, HTTP_PROXY, etc.).
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
schema_file: json-schema/v2-integration-schema.json
slug: v2-integration
source_filename: v2-integration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"IntegrationId\": {\n      \"type\": \"string\",\n      \"description\": \"Integration identifier.\",\n      \"example\": \"abc123\"\n    },\n    \"IntegrationType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of integration (AWS_PROXY, HTTP_PROXY, etc.).\",\n      \"example\": \"example-value\"\n    },\n    \"IntegrationUri\": {\n      \"type\": \"string\",\n      \"description\": \"Integration target URI.\",\n      \"example\": \"https://example.com/resource/123\"\n    },\n    \"PayloadFormatVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Payload format version.\",\n      \"example\": \"1.0\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v2-integration-schema.json\",\n  \"title\": \"Integration\",\n  \"description\": \"Integration schema from\
  \ Amazon API Gateway v2 API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v2-integration-schema.json
tags:
- API Gateway
- Cloud
- REST
- WebSocket
- Serverless
title: Integration
---
