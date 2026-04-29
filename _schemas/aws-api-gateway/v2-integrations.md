---
description: Integrations schema from Amazon API Gateway v2 API
layout: schema
name: Integrations
properties_list:
- description: ''
  name: Items
  type: array
provider_name: Amazon API Gateway
provider_slug: aws-api-gateway
schema_file: json-schema/v2-integrations-schema.json
slug: v2-integrations
source_filename: v2-integrations-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Items\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"IntegrationId\": {\n            \"type\": \"string\",\n            \"description\": \"Integration identifier.\",\n            \"example\": \"abc123\"\n          },\n          \"IntegrationType\": {\n            \"type\": \"string\",\n            \"description\": \"Type of integration (AWS_PROXY, HTTP_PROXY, etc.).\",\n            \"example\": \"example-value\"\n          },\n          \"IntegrationUri\": {\n            \"type\": \"string\",\n            \"description\": \"Integration target URI.\",\n            \"example\": \"https://example.com/resource/123\"\n          },\n          \"PayloadFormatVersion\": {\n            \"type\": \"string\",\n            \"description\": \"Payload format version.\",\n            \"example\": \"1.0\"\n          }\n        }\n      },\n      \"example\": [\n\
  \        \"example-value\"\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v2-integrations-schema.json\",\n  \"title\": \"Integrations\",\n  \"description\": \"Integrations schema from Amazon API Gateway v2 API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v2-integrations-schema.json
tags:
- API Gateway
- AWS
- Cloud
- REST
- WebSocket
- Serverless
title: Integrations
---
