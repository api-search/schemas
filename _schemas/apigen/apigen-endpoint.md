---
description: An API endpoint defining a single operation with its path, method, and request/response schemas.
layout: schema
name: APIGen Endpoint
properties_list:
- description: Unique identifier for the endpoint.
  name: id
  type: string
- description: ID of the parent API.
  name: apiId
  type: string
- description: URL path for the endpoint, starting with a forward slash.
  name: path
  type: string
- description: HTTP method for the endpoint.
  name: method
  type: string
- description: Short summary of what the endpoint does.
  name: summary
  type: string
- description: Detailed description of the endpoint behavior.
  name: description
  type: string
- description: Path, query, and header parameters.
  name: parameters
  type: array
- description: JSON Schema defining the request body.
  name: requestSchema
  type: object
- description: JSON Schema defining the success response body.
  name: responseSchema
  type: object
- description: Whether this endpoint requires authentication.
  name: authentication
  type: boolean
- description: ID of the connector used as the data source for this endpoint.
  name: connectorId
  type:
  - string
  - 'null'
- description: Timestamp when the endpoint was created.
  name: createdAt
  type: string
- description: Timestamp when the endpoint was last updated.
  name: updatedAt
  type: string
provider_name: APIGen
provider_slug: apigen
schema_file: json-schema/apigen-endpoint-schema.json
slug: apigen-endpoint
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.apigen.com/schemas/endpoint.json\",\n  \"title\": \"APIGen Endpoint\",\n  \"description\": \"An API endpoint defining a single operation with its path, method, and request/response schemas.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for the endpoint.\"\n    },\n    \"apiId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"ID of the parent API.\"\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"pattern\": \"^/\",\n      \"description\": \"URL path for the endpoint, starting with a forward slash.\"\n    },\n    \"method\": {\n      \"type\": \"string\",\n      \"enum\": [\"GET\", \"POST\", \"PUT\", \"PATCH\", \"DELETE\"],\n      \"description\": \"HTTP method for the endpoint.\"\n    },\n    \"summary\": {\n  \
  \    \"type\": \"string\",\n      \"maxLength\": 255,\n      \"description\": \"Short summary of what the endpoint does.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Detailed description of the endpoint behavior.\"\n    },\n    \"parameters\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"in\": {\n            \"type\": \"string\",\n            \"enum\": [\"path\", \"query\", \"header\"]\n          },\n          \"required\": {\n            \"type\": \"boolean\"\n          },\n          \"schema\": {\n            \"type\": \"object\"\n          },\n          \"description\": {\n            \"type\": \"string\"\n          }\n        },\n        \"required\": [\"name\", \"in\"]\n      },\n      \"description\": \"Path, query, and header parameters.\"\n    },\n    \"requestSchema\": {\n      \"type\": \"\
  object\",\n      \"description\": \"JSON Schema defining the request body.\"\n    },\n    \"responseSchema\": {\n      \"type\": \"object\",\n      \"description\": \"JSON Schema defining the success response body.\"\n    },\n    \"authentication\": {\n      \"type\": \"boolean\",\n      \"default\": true,\n      \"description\": \"Whether this endpoint requires authentication.\"\n    },\n    \"connectorId\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uuid\",\n      \"description\": \"ID of the connector used as the data source for this endpoint.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the endpoint was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the endpoint was last updated.\"\n    }\n  },\n  \"required\": [\"id\", \"apiId\", \"path\", \"method\", \"createdAt\", \"updatedAt\"\
  ],\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apigen/refs/heads/main/json-schema/apigen-endpoint-schema.json
tags:
- Code
- Documentation
- Generation
- Open Source
- PHP
title: APIGen Endpoint
---
