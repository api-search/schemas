---
description: Describes a single header parameter, following the structure of the Parameter Object but with fixed name and location.
layout: schema
name: OpenAPI Header Object
properties_list:
- description: A brief description of the header.
  name: description
  type: string
- description: ''
  name: required
  type: boolean
- description: ''
  name: deprecated
  type: boolean
- description: ''
  name: allowEmptyValue
  type: boolean
- description: ''
  name: style
  type: string
- description: ''
  name: explode
  type: boolean
- description: The schema defining the type used for the header.
  name: schema
  type: object
- description: Example of the header value.
  name: example
  type: object
- description: ''
  name: examples
  type: object
- description: ''
  name: content
  type: object
provider_name: OpenAPI
provider_slug: openapi
schema_file: json-schema/openapi-header.json
slug: openapi-header
source_filename: openapi-header.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"openapi-header.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OpenAPI Header Object\",\n  \"description\": \"Describes a single header parameter, following the structure of the Parameter Object but with fixed name and location.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A brief description of the header.\"\n    },\n    \"required\": {\n      \"type\": \"boolean\",\n      \"default\": false\n    },\n    \"deprecated\": {\n      \"type\": \"boolean\",\n      \"default\": false\n    },\n    \"allowEmptyValue\": {\n      \"type\": \"boolean\",\n      \"default\": false\n    },\n    \"style\": {\n      \"type\": \"string\",\n      \"default\": \"simple\"\n    },\n    \"explode\": {\n      \"type\": \"boolean\"\n    },\n    \"schema\": {\n      \"description\": \"The schema defining the type used for the header.\"\n    },\n    \"example\"\
  : {\n      \"description\": \"Example of the header value.\"\n    },\n    \"examples\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"$ref\": \"openapi-example.json\"\n      }\n    },\n    \"content\": {\n      \"type\": \"object\",\n      \"maxProperties\": 1,\n      \"additionalProperties\": {\n        \"$ref\": \"openapi-media-type.json\"\n      }\n    }\n  },\n  \"patternProperties\": {\n    \"^x-\": {}\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openapi/refs/heads/main/json-schema/openapi-header.json
tags:
- Documentation
- REST
- Specification
title: OpenAPI Header Object
---
