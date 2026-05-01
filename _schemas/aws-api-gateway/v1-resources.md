---
description: Resources schema from Amazon API Gateway v1 API
layout: schema
name: Resources
properties_list:
- description: ''
  name: items
  type: array
provider_name: Amazon API Gateway
provider_slug: aws-api-gateway
schema_file: json-schema/v1-resources-schema.json
slug: v1-resources
source_filename: v1-resources-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"items\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"Resource identifier.\",\n            \"example\": \"abc123\"\n          },\n          \"parentId\": {\n            \"type\": \"string\",\n            \"description\": \"Parent resource identifier.\",\n            \"example\": \"abc123\"\n          },\n          \"pathPart\": {\n            \"type\": \"string\",\n            \"description\": \"Last path segment for this resource.\",\n            \"example\": \"example-value\"\n          },\n          \"path\": {\n            \"type\": \"string\",\n            \"description\": \"Full path of the resource.\",\n            \"example\": \"example-value\"\n          }\n        }\n      },\n      \"example\": [\n        \"example-value\"\n      ]\n    }\n  },\n  \"$schema\":\
  \ \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v1-resources-schema.json\",\n  \"title\": \"Resources\",\n  \"description\": \"Resources schema from Amazon API Gateway v1 API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v1-resources-schema.json
tags:
- API Gateway
- Cloud
- REST
- WebSocket
- Serverless
title: Resources
---
