---
description: Allows referencing an external resource for extended documentation.
layout: schema
name: OpenAPI External Documentation Object
properties_list:
- description: A description of the target documentation.
  name: description
  type: string
- description: The URL for the target documentation.
  name: url
  type: string
provider_name: OpenAPI
provider_slug: openapi
schema_file: json-schema/openapi-external-documentation.json
slug: openapi-external-documentation
source_filename: openapi-external-documentation.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"openapi-external-documentation.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OpenAPI External Documentation Object\",\n  \"description\": \"Allows referencing an external resource for extended documentation.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"url\"\n  ],\n  \"properties\": {\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the target documentation.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL for the target documentation.\"\n    }\n  },\n  \"patternProperties\": {\n    \"^x-\": {}\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openapi/refs/heads/main/json-schema/openapi-external-documentation.json
tags:
- Documentation
- REST
- Specification
title: OpenAPI External Documentation Object
---
