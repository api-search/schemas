---
description: Represents a possible design-time link for a response, allowing transitions between operations.
layout: schema
name: OpenAPI Link Object
properties_list:
- description: A relative or absolute URI reference to an OAS operation.
  name: operationRef
  type: string
- description: The name of an existing resolvable OAS operation.
  name: operationId
  type: string
- description: A map representing parameters to pass to the linked operation.
  name: parameters
  type: object
- description: A literal value or runtime expression to use as a request body for the linked operation.
  name: requestBody
  type: object
- description: A description of the link.
  name: description
  type: string
- description: ''
  name: server
  type: object
provider_name: OpenAPI
provider_slug: openapi
schema_file: json-schema/openapi-link.json
slug: openapi-link
source_filename: openapi-link.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"openapi-link.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OpenAPI Link Object\",\n  \"description\": \"Represents a possible design-time link for a response, allowing transitions between operations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"operationRef\": {\n      \"type\": \"string\",\n      \"description\": \"A relative or absolute URI reference to an OAS operation.\"\n    },\n    \"operationId\": {\n      \"type\": \"string\",\n      \"description\": \"The name of an existing resolvable OAS operation.\"\n    },\n    \"parameters\": {\n      \"type\": \"object\",\n      \"description\": \"A map representing parameters to pass to the linked operation.\",\n      \"additionalProperties\": {}\n    },\n    \"requestBody\": {\n      \"description\": \"A literal value or runtime expression to use as a request body for the linked operation.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n\
  \      \"description\": \"A description of the link.\"\n    },\n    \"server\": {\n      \"$ref\": \"openapi-server.json\"\n    }\n  },\n  \"patternProperties\": {\n    \"^x-\": {}\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openapi/refs/heads/main/json-schema/openapi-link.json
tags:
- Documentation
- REST
- Specification
title: OpenAPI Link Object
---
