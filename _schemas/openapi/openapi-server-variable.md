---
description: An object representing a Server Variable for server URL template substitution.
layout: schema
name: OpenAPI Server Variable Object
properties_list:
- description: An enumeration of string values for limited variable substitution options.
  name: enum
  type: array
- description: The default value to use for substitution.
  name: default
  type: string
- description: An optional description for the server variable.
  name: description
  type: string
provider_name: OpenAPI
provider_slug: openapi
schema_file: json-schema/openapi-server-variable.json
slug: openapi-server-variable
source_filename: openapi-server-variable.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"openapi-server-variable.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OpenAPI Server Variable Object\",\n  \"description\": \"An object representing a Server Variable for server URL template substitution.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"default\"\n  ],\n  \"properties\": {\n    \"enum\": {\n      \"type\": \"array\",\n      \"description\": \"An enumeration of string values for limited variable substitution options.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"minItems\": 1\n    },\n    \"default\": {\n      \"type\": \"string\",\n      \"description\": \"The default value to use for substitution.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"An optional description for the server variable.\"\n    }\n  },\n  \"patternProperties\": {\n    \"^x-\": {}\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openapi/refs/heads/main/json-schema/openapi-server-variable.json
tags:
- Documentation
- REST
- Specification
title: OpenAPI Server Variable Object
---
