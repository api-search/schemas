---
description: ApiKeys schema from Amazon API Gateway v1 API
layout: schema
name: ApiKeys
properties_list:
- description: ''
  name: items
  type: array
provider_name: Amazon API Gateway
provider_slug: aws-api-gateway
schema_file: json-schema/v1-api-keys-schema.json
slug: v1-api-keys
source_filename: v1-api-keys-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"items\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"ApiKey identifier.\",\n            \"example\": \"abc123\"\n          },\n          \"value\": {\n            \"type\": \"string\",\n            \"description\": \"Value of the ApiKey.\",\n            \"example\": \"example-value\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Name of the ApiKey.\",\n            \"example\": \"my-resource\"\n          },\n          \"enabled\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether the ApiKey is enabled.\",\n            \"example\": true\n          }\n        }\n      },\n      \"example\": [\n        \"example-value\"\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v1-api-keys-schema.json\",\n  \"title\": \"ApiKeys\",\n  \"description\": \"ApiKeys schema from Amazon API Gateway v1 API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v1-api-keys-schema.json
tags:
- API Gateway
- Cloud
- REST
- WebSocket
- Serverless
title: ApiKeys
---
