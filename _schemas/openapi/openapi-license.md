---
description: License information for the exposed API.
layout: schema
name: OpenAPI License Object
properties_list:
- description: The license name used for the API.
  name: name
  type: string
- description: An SPDX license expression for the API.
  name: identifier
  type: string
- description: A URL to the license used for the API.
  name: url
  type: string
provider_name: OpenAPI
provider_slug: openapi
schema_file: json-schema/openapi-license.json
slug: openapi-license
source_filename: openapi-license.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"openapi-license.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OpenAPI License Object\",\n  \"description\": \"License information for the exposed API.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"name\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The license name used for the API.\"\n    },\n    \"identifier\": {\n      \"type\": \"string\",\n      \"description\": \"An SPDX license expression for the API.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"A URL to the license used for the API.\"\n    }\n  },\n  \"patternProperties\": {\n    \"^x-\": {}\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openapi/refs/heads/main/json-schema/openapi-license.json
tags:
- Documentation
- REST
- Specification
title: OpenAPI License Object
---
