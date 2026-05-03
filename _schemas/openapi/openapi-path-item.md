---
description: Describes the operations available on a single path. A Path Item may be empty due to ACL constraints.
layout: schema
name: OpenAPI Path Item Object
properties_list:
- description: Allows for a referenced definition of this path item.
  name: $ref
  type: string
- description: An optional string summary intended to apply to all operations in this path.
  name: summary
  type: string
- description: An optional string description intended to apply to all operations in this path.
  name: description
  type: string
- description: ''
  name: get
  type: object
- description: ''
  name: put
  type: object
- description: ''
  name: post
  type: object
- description: ''
  name: delete
  type: object
- description: ''
  name: options
  type: object
- description: ''
  name: head
  type: object
- description: ''
  name: patch
  type: object
- description: ''
  name: trace
  type: object
- description: Alternative servers to service all operations in this path.
  name: servers
  type: array
- description: A list of parameters applicable for all operations described under this path.
  name: parameters
  type: array
provider_name: OpenAPI
provider_slug: openapi
schema_file: json-schema/openapi-path-item.json
slug: openapi-path-item
source_filename: openapi-path-item.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"openapi-path-item.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OpenAPI Path Item Object\",\n  \"description\": \"Describes the operations available on a single path. A Path Item may be empty due to ACL constraints.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"$ref\": {\n      \"type\": \"string\",\n      \"description\": \"Allows for a referenced definition of this path item.\"\n    },\n    \"summary\": {\n      \"type\": \"string\",\n      \"description\": \"An optional string summary intended to apply to all operations in this path.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"An optional string description intended to apply to all operations in this path.\"\n    },\n    \"get\": {\n      \"$ref\": \"openapi-operation.json\"\n    },\n    \"put\": {\n      \"$ref\": \"openapi-operation.json\"\n    },\n    \"post\": {\n      \"$ref\": \"openapi-operation.json\"\
  \n    },\n    \"delete\": {\n      \"$ref\": \"openapi-operation.json\"\n    },\n    \"options\": {\n      \"$ref\": \"openapi-operation.json\"\n    },\n    \"head\": {\n      \"$ref\": \"openapi-operation.json\"\n    },\n    \"patch\": {\n      \"$ref\": \"openapi-operation.json\"\n    },\n    \"trace\": {\n      \"$ref\": \"openapi-operation.json\"\n    },\n    \"servers\": {\n      \"type\": \"array\",\n      \"description\": \"Alternative servers to service all operations in this path.\",\n      \"items\": {\n        \"$ref\": \"openapi-server.json\"\n      }\n    },\n    \"parameters\": {\n      \"type\": \"array\",\n      \"description\": \"A list of parameters applicable for all operations described under this path.\",\n      \"items\": {\n        \"$ref\": \"openapi-parameter.json\"\n      }\n    }\n  },\n  \"patternProperties\": {\n    \"^x-\": {}\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openapi/refs/heads/main/json-schema/openapi-path-item.json
tags:
- Documentation
- REST
- Specification
title: OpenAPI Path Item Object
---
