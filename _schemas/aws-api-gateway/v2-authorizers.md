---
description: Authorizers schema from Amazon API Gateway v2 API
layout: schema
name: Authorizers
properties_list:
- description: ''
  name: Items
  type: array
provider_name: Amazon API Gateway
provider_slug: aws-api-gateway
schema_file: json-schema/v2-authorizers-schema.json
slug: v2-authorizers
source_filename: v2-authorizers-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Items\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"AuthorizerId\": {\n            \"type\": \"string\",\n            \"description\": \"Authorizer identifier.\",\n            \"example\": \"abc123\"\n          },\n          \"Name\": {\n            \"type\": \"string\",\n            \"description\": \"Authorizer name.\",\n            \"example\": \"my-resource\"\n          },\n          \"AuthorizerType\": {\n            \"type\": \"string\",\n            \"description\": \"Type of authorizer (REQUEST or JWT).\",\n            \"example\": \"example-value\"\n          },\n          \"IdentitySource\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            },\n            \"description\": \"Identity sources for the authorizer.\",\n            \"example\": [\n              \"example-value\"\
  \n            ]\n          }\n        }\n      },\n      \"example\": [\n        \"example-value\"\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v2-authorizers-schema.json\",\n  \"title\": \"Authorizers\",\n  \"description\": \"Authorizers schema from Amazon API Gateway v2 API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v2-authorizers-schema.json
tags:
- API Gateway
- Cloud
- REST
- WebSocket
- Serverless
title: Authorizers
---
