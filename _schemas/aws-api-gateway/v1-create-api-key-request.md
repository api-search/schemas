---
description: CreateApiKeyRequest schema from Amazon API Gateway v1 API
layout: schema
name: CreateApiKeyRequest
properties_list:
- description: Name of the ApiKey.
  name: name
  type: string
- description: Description of the ApiKey.
  name: description
  type: string
- description: Whether the ApiKey should be enabled.
  name: enabled
  type: boolean
provider_name: Amazon API Gateway
provider_slug: aws-api-gateway
schema_file: json-schema/v1-create-api-key-request-schema.json
slug: v1-create-api-key-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the ApiKey.\",\n      \"example\": \"my-resource\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the ApiKey.\",\n      \"example\": \"A description of this resource.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the ApiKey should be enabled.\",\n      \"example\": true\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v1-create-api-key-request-schema.json\",\n  \"title\": \"CreateApiKeyRequest\",\n  \"description\": \"CreateApiKeyRequest schema from Amazon API Gateway v1 API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v1-create-api-key-request-schema.json
tags:
- API Gateway
- AWS
- Cloud
- REST
- WebSocket
- Serverless
title: CreateApiKeyRequest
---
