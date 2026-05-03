---
description: An object representing a Server, providing connectivity information to a target server.
layout: schema
name: OpenAPI Server Object
properties_list:
- description: A URL to the target host. Supports server variables with {variable} templating.
  name: url
  type: string
- description: An optional string describing the host designated by the URL.
  name: description
  type: string
- description: A map between a variable name and its value for URL template substitution.
  name: variables
  type: object
provider_name: OpenAPI
provider_slug: openapi
schema_file: json-schema/openapi-server.json
slug: openapi-server
source_filename: openapi-server.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"openapi-server.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OpenAPI Server Object\",\n  \"description\": \"An object representing a Server, providing connectivity information to a target server.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"url\"\n  ],\n  \"properties\": {\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"A URL to the target host. Supports server variables with {variable} templating.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"An optional string describing the host designated by the URL.\"\n    },\n    \"variables\": {\n      \"type\": \"object\",\n      \"description\": \"A map between a variable name and its value for URL template substitution.\",\n      \"additionalProperties\": {\n        \"$ref\": \"openapi-server-variable.json\"\n      }\n    }\n  },\n  \"patternProperties\": {\n    \"^x-\": {}\n  },\n  \"additionalProperties\"\
  : false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openapi/refs/heads/main/json-schema/openapi-server.json
tags:
- Documentation
- REST
- Specification
title: OpenAPI Server Object
---
