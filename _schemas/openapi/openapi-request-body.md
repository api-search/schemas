---
description: Describes a single request body.
layout: schema
name: OpenAPI Request Body Object
properties_list:
- description: A brief description of the request body.
  name: description
  type: string
- description: The content of the request body, mapped by media type.
  name: content
  type: object
- description: Whether the request body is required in the request.
  name: required
  type: boolean
provider_name: OpenAPI
provider_slug: openapi
schema_file: json-schema/openapi-request-body.json
slug: openapi-request-body
source_filename: openapi-request-body.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"openapi-request-body.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OpenAPI Request Body Object\",\n  \"description\": \"Describes a single request body.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"content\"\n  ],\n  \"properties\": {\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A brief description of the request body.\"\n    },\n    \"content\": {\n      \"type\": \"object\",\n      \"description\": \"The content of the request body, mapped by media type.\",\n      \"additionalProperties\": {\n        \"$ref\": \"openapi-media-type.json\"\n      }\n    },\n    \"required\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the request body is required in the request.\",\n      \"default\": false\n    }\n  },\n  \"patternProperties\": {\n    \"^x-\": {}\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openapi/refs/heads/main/json-schema/openapi-request-body.json
tags:
- Documentation
- REST
- Specification
title: OpenAPI Request Body Object
---
