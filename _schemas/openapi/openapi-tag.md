---
description: Adds metadata to a single tag that is used by the Operation Object.
layout: schema
name: OpenAPI Tag Object
properties_list:
- description: The name of the tag.
  name: name
  type: string
- description: A description for the tag.
  name: description
  type: string
- description: ''
  name: externalDocs
  type: object
provider_name: OpenAPI
provider_slug: openapi
schema_file: json-schema/openapi-tag.json
slug: openapi-tag
source_filename: openapi-tag.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"openapi-tag.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OpenAPI Tag Object\",\n  \"description\": \"Adds metadata to a single tag that is used by the Operation Object.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"name\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the tag.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description for the tag.\"\n    },\n    \"externalDocs\": {\n      \"$ref\": \"openapi-external-documentation.json\"\n    }\n  },\n  \"patternProperties\": {\n    \"^x-\": {}\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openapi/refs/heads/main/json-schema/openapi-tag.json
tags:
- Documentation
- REST
- Specification
title: OpenAPI Tag Object
---
