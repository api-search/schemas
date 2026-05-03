---
description: A single encoding definition applied to a single schema property.
layout: schema
name: OpenAPI Encoding Object
properties_list:
- description: The Content-Type for encoding a specific property.
  name: contentType
  type: string
- description: A map allowing additional information to be provided as headers.
  name: headers
  type: object
- description: Describes how a specific property value will be serialized.
  name: style
  type: string
- description: Whether parameter values of type array or object generate separate parameters.
  name: explode
  type: boolean
- description: Whether the parameter value allows reserved characters.
  name: allowReserved
  type: boolean
provider_name: OpenAPI
provider_slug: openapi
schema_file: json-schema/openapi-encoding.json
slug: openapi-encoding
source_filename: openapi-encoding.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"openapi-encoding.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OpenAPI Encoding Object\",\n  \"description\": \"A single encoding definition applied to a single schema property.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"contentType\": {\n      \"type\": \"string\",\n      \"description\": \"The Content-Type for encoding a specific property.\"\n    },\n    \"headers\": {\n      \"type\": \"object\",\n      \"description\": \"A map allowing additional information to be provided as headers.\",\n      \"additionalProperties\": {\n        \"$ref\": \"openapi-header.json\"\n      }\n    },\n    \"style\": {\n      \"type\": \"string\",\n      \"description\": \"Describes how a specific property value will be serialized.\"\n    },\n    \"explode\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether parameter values of type array or object generate separate parameters.\"\n    },\n    \"allowReserved\"\
  : {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the parameter value allows reserved characters.\",\n      \"default\": false\n    }\n  },\n  \"patternProperties\": {\n    \"^x-\": {}\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openapi/refs/heads/main/json-schema/openapi-encoding.json
tags:
- Documentation
- REST
- Specification
title: OpenAPI Encoding Object
---
