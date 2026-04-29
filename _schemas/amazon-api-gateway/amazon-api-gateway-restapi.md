---
description: ''
layout: schema
name: RestApi
properties_list:
- description: The API's identifier.
  name: id
  type: string
- description: The API's name.
  name: name
  type: string
- description: The API's description.
  name: description
  type: string
- description: The timestamp when the API was created.
  name: createdDate
  type: string
- description: A version identifier for the API.
  name: version
  type: string
- description: The warning messages reported when failonwarnings is on.
  name: warnings
  type: array
- description: The list of binary media types supported by the REST API.
  name: binaryMediaTypes
  type: array
- description: A nullable integer for the minimum payload size in bytes to compress.
  name: minimumCompressionSize
  type: integer
- description: The source of the API key for metering requests.
  name: apiKeySource
  type: string
- description: ''
  name: endpointConfiguration
  type: object
- description: A stringified JSON policy document that applies to this REST API.
  name: policy
  type: string
- description: Tags attached to the REST API.
  name: tags
  type: object
- description: Specifies whether clients can invoke your API by using the default execute-api endpoint.
  name: disableExecuteApiEndpoint
  type: boolean
provider_name: Amazon API Gateway
provider_slug: amazon-api-gateway
schema_file: json-schema/amazon-api-gateway-restapi-schema.json
slug: amazon-api-gateway-restapi
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"RestApi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The API's identifier.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The API's name.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The API's description.\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the API was created.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"A version identifier for the API.\"\n    },\n    \"warnings\": {\n      \"type\": \"array\",\n      \"description\": \"The warning messages reported when failonwarnings is on.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"binaryMediaTypes\": {\n      \"type\": \"array\"\
  ,\n      \"description\": \"The list of binary media types supported by the REST API.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"minimumCompressionSize\": {\n      \"type\": \"integer\",\n      \"description\": \"A nullable integer for the minimum payload size in bytes to compress.\"\n    },\n    \"apiKeySource\": {\n      \"type\": \"string\",\n      \"description\": \"The source of the API key for metering requests.\",\n      \"enum\": [\n        \"HEADER\",\n        \"AUTHORIZER\"\n      ]\n    },\n    \"endpointConfiguration\": {\n      \"$ref\": \"#/definitions/EndpointConfiguration\"\n    },\n    \"policy\": {\n      \"type\": \"string\",\n      \"description\": \"A stringified JSON policy document that applies to this REST API.\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Tags attached to the REST API.\"\n    },\n    \"disableExecuteApiEndpoint\": {\n      \"type\": \"boolean\",\n      \"description\": \"Specifies\
  \ whether clients can invoke your API by using the default execute-api endpoint.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/json-schema/amazon-api-gateway-restapi-schema.json
tags:
- AWS
- Gateway
- HTTP API
- REST API
- Serverless
- WebSocket
title: RestApi
---
