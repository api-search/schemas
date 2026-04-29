---
description: CreateAuthorizerRequest schema from Amazon API Gateway v2 API
layout: schema
name: CreateAuthorizerRequest
properties_list:
- description: Name of the authorizer.
  name: Name
  type: string
- description: Type of authorizer.
  name: AuthorizerType
  type: string
- description: Identity sources to use.
  name: IdentitySource
  type: array
- description: URI of the Lambda authorizer (REQUEST type).
  name: AuthorizerUri
  type: string
provider_name: Amazon API Gateway
provider_slug: aws-api-gateway
schema_file: json-schema/v2-create-authorizer-request-schema.json
slug: v2-create-authorizer-request
source_filename: v2-create-authorizer-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the authorizer.\",\n      \"example\": \"my-resource\"\n    },\n    \"AuthorizerType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"REQUEST\",\n        \"JWT\"\n      ],\n      \"description\": \"Type of authorizer.\",\n      \"example\": \"REQUEST\"\n    },\n    \"IdentitySource\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Identity sources to use.\",\n      \"example\": [\n        \"example-value\"\n      ]\n    },\n    \"AuthorizerUri\": {\n      \"type\": \"string\",\n      \"description\": \"URI of the Lambda authorizer (REQUEST type).\",\n      \"example\": \"https://example.com/resource/123\"\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"AuthorizerType\",\n    \"IdentitySource\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v2-create-authorizer-request-schema.json\",\n  \"title\": \"CreateAuthorizerRequest\",\n  \"description\": \"CreateAuthorizerRequest schema from Amazon API Gateway v2 API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v2-create-authorizer-request-schema.json
tags:
- API Gateway
- AWS
- Cloud
- REST
- WebSocket
- Serverless
title: CreateAuthorizerRequest
---
