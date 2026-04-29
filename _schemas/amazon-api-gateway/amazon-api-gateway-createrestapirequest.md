---
description: ''
layout: schema
name: CreateRestApiRequest
properties_list:
- description: The name of the REST API.
  name: name
  type: string
- description: The description of the REST API.
  name: description
  type: string
- description: A version identifier for the API.
  name: version
  type: string
- description: The ID of the REST API to clone from.
  name: cloneFrom
  type: string
- description: The list of binary media types to support.
  name: binaryMediaTypes
  type: array
- description: Minimum payload compression size in bytes.
  name: minimumCompressionSize
  type: integer
- description: ''
  name: apiKeySource
  type: string
- description: ''
  name: endpointConfiguration
  type: object
- description: ''
  name: policy
  type: string
- description: ''
  name: tags
  type: object
- description: ''
  name: disableExecuteApiEndpoint
  type: boolean
provider_name: Amazon API Gateway
provider_slug: amazon-api-gateway
schema_file: json-schema/amazon-api-gateway-createrestapirequest-schema.json
slug: amazon-api-gateway-createrestapirequest
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"CreateRestApiRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the REST API.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The description of the REST API.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"A version identifier for the API.\"\n    },\n    \"cloneFrom\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the REST API to clone from.\"\n    },\n    \"binaryMediaTypes\": {\n      \"type\": \"array\",\n      \"description\": \"The list of binary media types to support.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"minimumCompressionSize\": {\n      \"type\": \"integer\",\n      \"description\": \"Minimum payload compression size in bytes.\"\n    },\n    \"apiKeySource\": {\n\
  \      \"type\": \"string\",\n      \"enum\": [\n        \"HEADER\",\n        \"AUTHORIZER\"\n      ]\n    },\n    \"endpointConfiguration\": {\n      \"$ref\": \"#/definitions/EndpointConfiguration\"\n    },\n    \"policy\": {\n      \"type\": \"string\"\n    },\n    \"tags\": {\n      \"type\": \"object\"\n    },\n    \"disableExecuteApiEndpoint\": {\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/json-schema/amazon-api-gateway-createrestapirequest-schema.json
tags:
- AWS
- Gateway
- HTTP API
- REST API
- Serverless
- WebSocket
title: CreateRestApiRequest
---
