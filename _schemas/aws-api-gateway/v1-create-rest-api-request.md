---
description: CreateRestApiRequest schema from Amazon API Gateway v1 API
layout: schema
name: CreateRestApiRequest
properties_list:
- description: Name of the new RestApi.
  name: name
  type: string
- description: Optional description.
  name: description
  type: string
- description: Version identifier.
  name: version
  type: string
- description: ''
  name: endpointConfiguration
  type: object
provider_name: Amazon API Gateway
provider_slug: aws-api-gateway
schema_file: json-schema/v1-create-rest-api-request-schema.json
slug: v1-create-rest-api-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the new RestApi.\",\n      \"example\": \"my-resource\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Optional description.\",\n      \"example\": \"A description of this resource.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Version identifier.\",\n      \"example\": \"1.0\"\n    },\n    \"endpointConfiguration\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"types\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"EDGE\",\n              \"REGIONAL\",\n              \"PRIVATE\"\n            ]\n          },\n          \"description\": \"List of endpoint types (EDGE, REGIONAL, PRIVATE).\",\n          \"example\": [\n            \"EDGE\"\n          ]\n        }\n \
  \     }\n    }\n  },\n  \"required\": [\n    \"name\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v1-create-rest-api-request-schema.json\",\n  \"title\": \"CreateRestApiRequest\",\n  \"description\": \"CreateRestApiRequest schema from Amazon API Gateway v1 API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v1-create-rest-api-request-schema.json
tags:
- API Gateway
- AWS
- Cloud
- REST
- WebSocket
- Serverless
title: CreateRestApiRequest
---
