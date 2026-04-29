---
description: Authorizer schema from Amazon API Gateway v2 API
layout: schema
name: Authorizer
properties_list:
- description: Authorizer identifier.
  name: AuthorizerId
  type: string
- description: Authorizer name.
  name: Name
  type: string
- description: Type of authorizer (REQUEST or JWT).
  name: AuthorizerType
  type: string
- description: Identity sources for the authorizer.
  name: IdentitySource
  type: array
provider_name: Amazon API Gateway
provider_slug: aws-api-gateway
schema_file: json-schema/v2-authorizer-schema.json
slug: v2-authorizer
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"AuthorizerId\": {\n      \"type\": \"string\",\n      \"description\": \"Authorizer identifier.\",\n      \"example\": \"abc123\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"Authorizer name.\",\n      \"example\": \"my-resource\"\n    },\n    \"AuthorizerType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of authorizer (REQUEST or JWT).\",\n      \"example\": \"example-value\"\n    },\n    \"IdentitySource\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Identity sources for the authorizer.\",\n      \"example\": [\n        \"example-value\"\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v2-authorizer-schema.json\",\n  \"title\": \"Authorizer\",\n  \"description\"\
  : \"Authorizer schema from Amazon API Gateway v2 API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v2-authorizer-schema.json
tags:
- API Gateway
- AWS
- Cloud
- REST
- WebSocket
- Serverless
title: Authorizer
---
