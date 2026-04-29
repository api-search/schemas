---
description: RestApi schema from Amazon API Gateway v1 API
layout: schema
name: RestApi
properties_list:
- description: Identifier of the RestApi.
  name: id
  type: string
- description: Name of the RestApi.
  name: name
  type: string
- description: Description of the RestApi.
  name: description
  type: string
- description: Timestamp when the RestApi was created.
  name: createdDate
  type: string
- description: Version identifier of the API.
  name: version
  type: string
- description: ''
  name: endpointConfiguration
  type: object
provider_name: Amazon API Gateway
provider_slug: aws-api-gateway
schema_file: json-schema/v1-rest-api-schema.json
slug: v1-rest-api
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the RestApi.\",\n      \"example\": \"abc123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the RestApi.\",\n      \"example\": \"my-resource\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the RestApi.\",\n      \"example\": \"A description of this resource.\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the RestApi was created.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Version identifier of the API.\",\n      \"example\": \"1.0\"\n    },\n    \"endpointConfiguration\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"types\": {\n          \"type\": \"\
  array\",\n          \"items\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"EDGE\",\n              \"REGIONAL\",\n              \"PRIVATE\"\n            ]\n          },\n          \"description\": \"List of endpoint types (EDGE, REGIONAL, PRIVATE).\",\n          \"example\": [\n            \"EDGE\"\n          ]\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v1-rest-api-schema.json\",\n  \"title\": \"RestApi\",\n  \"description\": \"RestApi schema from Amazon API Gateway v1 API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v1-rest-api-schema.json
tags:
- API Gateway
- AWS
- Cloud
- REST
- WebSocket
- Serverless
title: RestApi
---
