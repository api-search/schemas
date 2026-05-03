---
description: Describes a single operation parameter. A unique parameter is defined by a combination of a name and location.
layout: schema
name: OpenAPI Parameter Object
properties_list:
- description: The name of the parameter.
  name: name
  type: string
- description: The location of the parameter.
  name: in
  type: string
- description: A brief description of the parameter.
  name: description
  type: string
- description: Whether this parameter is mandatory.
  name: required
  type: boolean
- description: Whether the parameter is deprecated.
  name: deprecated
  type: boolean
- description: Whether empty-valued parameters are allowed.
  name: allowEmptyValue
  type: boolean
- description: How the parameter value will be serialized.
  name: style
  type: string
- description: Whether parameter values of type array or object generate separate parameters.
  name: explode
  type: boolean
- description: Whether the parameter value allows reserved characters.
  name: allowReserved
  type: boolean
- description: The schema defining the type used for the parameter.
  name: schema
  type: object
- description: Example of the parameter value.
  name: example
  type: object
- description: Examples of the parameter value.
  name: examples
  type: object
- description: A map containing the representations for the parameter.
  name: content
  type: object
provider_name: OpenAPI
provider_slug: openapi
schema_file: json-schema/openapi-parameter.json
slug: openapi-parameter
source_filename: openapi-parameter.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"openapi-parameter.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OpenAPI Parameter Object\",\n  \"description\": \"Describes a single operation parameter. A unique parameter is defined by a combination of a name and location.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"name\",\n    \"in\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the parameter.\"\n    },\n    \"in\": {\n      \"type\": \"string\",\n      \"description\": \"The location of the parameter.\",\n      \"enum\": [\n        \"query\",\n        \"header\",\n        \"path\",\n        \"cookie\"\n      ]\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A brief description of the parameter.\"\n    },\n    \"required\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this parameter is mandatory.\",\n      \"default\": false\n \
  \   },\n    \"deprecated\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the parameter is deprecated.\",\n      \"default\": false\n    },\n    \"allowEmptyValue\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether empty-valued parameters are allowed.\",\n      \"default\": false\n    },\n    \"style\": {\n      \"type\": \"string\",\n      \"description\": \"How the parameter value will be serialized.\"\n    },\n    \"explode\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether parameter values of type array or object generate separate parameters.\"\n    },\n    \"allowReserved\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the parameter value allows reserved characters.\",\n      \"default\": false\n    },\n    \"schema\": {\n      \"description\": \"The schema defining the type used for the parameter.\"\n    },\n    \"example\": {\n      \"description\": \"Example of the parameter value.\"\n    },\n    \"examples\"\
  : {\n      \"type\": \"object\",\n      \"description\": \"Examples of the parameter value.\",\n      \"additionalProperties\": {\n        \"$ref\": \"openapi-example.json\"\n      }\n    },\n    \"content\": {\n      \"type\": \"object\",\n      \"description\": \"A map containing the representations for the parameter.\",\n      \"maxProperties\": 1,\n      \"additionalProperties\": {\n        \"$ref\": \"openapi-media-type.json\"\n      }\n    }\n  },\n  \"patternProperties\": {\n    \"^x-\": {}\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openapi/refs/heads/main/json-schema/openapi-parameter.json
tags:
- Documentation
- REST
- Specification
title: OpenAPI Parameter Object
---
