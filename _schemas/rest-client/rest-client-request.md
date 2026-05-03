---
description: Schema for an HTTP request as authored in a .http or .rest file using the VS Code REST Client extension.
layout: schema
name: REST Client HTTP Request
properties_list:
- description: The HTTP method for the request.
  name: method
  type: string
- description: The full URL for the request, may include variable placeholders like {{host}}.
  name: url
  type: string
- description: HTTP protocol version.
  name: httpVersion
  type: string
- description: HTTP request headers as key-value pairs.
  name: headers
  type: object
- description: The request body, as a string, JSON object, or GraphQL query.
  name: body
  type: object
- description: 'Optional name for the request, used as a variable in request chaining (e.g., # @name myRequest).'
  name: name
  type: string
- description: File-level variables defined with @variableName = value syntax.
  name: variables
  type: object
- description: The active environment profile name providing variable values.
  name: environment
  type: string
- description: ''
  name: graphql
  type: object
provider_name: REST Client
provider_slug: rest-client
schema_file: json-schema/rest-client-request-schema.json
slug: rest-client-request
source_filename: rest-client-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://marketplace.visualstudio.com/items/humao.rest-client/schemas/request\",\n  \"title\": \"REST Client HTTP Request\",\n  \"description\": \"Schema for an HTTP request as authored in a .http or .rest file using the VS Code REST Client extension.\",\n  \"type\": \"object\",\n  \"required\": [\"method\", \"url\"],\n  \"properties\": {\n    \"method\": {\n      \"type\": \"string\",\n      \"enum\": [\"GET\", \"POST\", \"PUT\", \"DELETE\", \"PATCH\", \"HEAD\", \"OPTIONS\", \"CONNECT\", \"TRACE\"],\n      \"description\": \"The HTTP method for the request.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"The full URL for the request, may include variable placeholders like {{host}}.\"\n    },\n    \"httpVersion\": {\n      \"type\": \"string\",\n      \"enum\": [\"HTTP/1.1\", \"HTTP/2\"],\n      \"default\": \"HTTP/1.1\",\n      \"description\": \"HTTP protocol\
  \ version.\"\n    },\n    \"headers\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"HTTP request headers as key-value pairs.\"\n    },\n    \"body\": {\n      \"description\": \"The request body, as a string, JSON object, or GraphQL query.\",\n      \"oneOf\": [\n        { \"type\": \"string\" },\n        { \"type\": \"object\" },\n        { \"type\": \"array\" }\n      ]\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Optional name for the request, used as a variable in request chaining (e.g., # @name myRequest).\"\n    },\n    \"variables\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"File-level variables defined with @variableName = value syntax.\"\n    },\n    \"environment\": {\n      \"type\": \"string\",\n      \"description\": \"The active environment profile name providing\
  \ variable values.\"\n    },\n    \"graphql\": {\n      \"$ref\": \"#/$defs/GraphQLRequest\"\n    }\n  },\n  \"$defs\": {\n    \"GraphQLRequest\": {\n      \"title\": \"GraphQL Request\",\n      \"description\": \"GraphQL-specific request body structure.\",\n      \"type\": \"object\",\n      \"required\": [\"query\"],\n      \"properties\": {\n        \"query\": {\n          \"type\": \"string\",\n          \"description\": \"The GraphQL query or mutation string.\"\n        },\n        \"variables\": {\n          \"type\": \"object\",\n          \"description\": \"Variable values for the GraphQL query.\"\n        },\n        \"operationName\": {\n          \"type\": \"string\",\n          \"description\": \"Optional operation name for multi-operation documents.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rest-client/refs/heads/main/json-schema/rest-client-request-schema.json
tags:
- Clients
- HTTP Client
- IDE Extension
- VS Code
- API Testing
title: REST Client HTTP Request
---
