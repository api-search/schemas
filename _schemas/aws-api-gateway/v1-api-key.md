---
description: ApiKey schema from Amazon API Gateway v1 API
layout: schema
name: ApiKey
properties_list:
- description: ApiKey identifier.
  name: id
  type: string
- description: Value of the ApiKey.
  name: value
  type: string
- description: Name of the ApiKey.
  name: name
  type: string
- description: Whether the ApiKey is enabled.
  name: enabled
  type: boolean
provider_name: Amazon API Gateway
provider_slug: aws-api-gateway
schema_file: json-schema/v1-api-key-schema.json
slug: v1-api-key
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"ApiKey identifier.\",\n      \"example\": \"abc123\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"Value of the ApiKey.\",\n      \"example\": \"example-value\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the ApiKey.\",\n      \"example\": \"my-resource\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the ApiKey is enabled.\",\n      \"example\": true\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v1-api-key-schema.json\",\n  \"title\": \"ApiKey\",\n  \"description\": \"ApiKey schema from Amazon API Gateway v1 API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v1-api-key-schema.json
tags:
- API Gateway
- AWS
- Cloud
- REST
- WebSocket
- Serverless
title: ApiKey
---
