---
description: Describes a single API operation on a path.
layout: schema
name: OpenAPI Operation Object
properties_list:
- description: A list of tags for API documentation control.
  name: tags
  type: array
- description: A short summary of what the operation does.
  name: summary
  type: string
- description: A verbose explanation of the operation behavior.
  name: description
  type: string
- description: ''
  name: externalDocs
  type: object
- description: Unique string used to identify the operation.
  name: operationId
  type: string
- description: A list of parameters applicable for this operation.
  name: parameters
  type: array
- description: ''
  name: requestBody
  type: object
- description: ''
  name: responses
  type: object
- description: A map of possible out-of-band callbacks related to the operation.
  name: callbacks
  type: object
- description: Declares this operation to be deprecated.
  name: deprecated
  type: boolean
- description: Security mechanisms applicable for this operation.
  name: security
  type: array
- description: Alternative servers to service this operation.
  name: servers
  type: array
provider_name: OpenAPI
provider_slug: openapi
schema_file: json-schema/openapi-operation.json
slug: openapi-operation
source_filename: openapi-operation.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"openapi-operation.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OpenAPI Operation Object\",\n  \"description\": \"Describes a single API operation on a path.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"A list of tags for API documentation control.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"summary\": {\n      \"type\": \"string\",\n      \"description\": \"A short summary of what the operation does.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A verbose explanation of the operation behavior.\"\n    },\n    \"externalDocs\": {\n      \"$ref\": \"openapi-external-documentation.json\"\n    },\n    \"operationId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique string used to identify the operation.\"\n    },\n    \"parameters\": {\n      \"type\": \"\
  array\",\n      \"description\": \"A list of parameters applicable for this operation.\",\n      \"items\": {\n        \"$ref\": \"openapi-parameter.json\"\n      }\n    },\n    \"requestBody\": {\n      \"$ref\": \"openapi-request-body.json\"\n    },\n    \"responses\": {\n      \"$ref\": \"openapi-responses.json\"\n    },\n    \"callbacks\": {\n      \"type\": \"object\",\n      \"description\": \"A map of possible out-of-band callbacks related to the operation.\",\n      \"additionalProperties\": {\n        \"$ref\": \"openapi-path-item.json\"\n      }\n    },\n    \"deprecated\": {\n      \"type\": \"boolean\",\n      \"description\": \"Declares this operation to be deprecated.\",\n      \"default\": false\n    },\n    \"security\": {\n      \"type\": \"array\",\n      \"description\": \"Security mechanisms applicable for this operation.\",\n      \"items\": {\n        \"$ref\": \"openapi-security-requirement.json\"\n      }\n    },\n    \"servers\": {\n      \"type\": \"array\",\n\
  \      \"description\": \"Alternative servers to service this operation.\",\n      \"items\": {\n        \"$ref\": \"openapi-server.json\"\n      }\n    }\n  },\n  \"patternProperties\": {\n    \"^x-\": {}\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openapi/refs/heads/main/json-schema/openapi-operation.json
tags:
- Documentation
- REST
- Specification
title: OpenAPI Operation Object
---
