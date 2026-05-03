---
description: Describes a single response from an API Operation, including design-time, static links to operations based on the response.
layout: schema
name: OpenAPI Response Object
properties_list:
- description: A description of the response.
  name: description
  type: string
- description: Maps a header name to its definition.
  name: headers
  type: object
- description: A map containing the representations for the response.
  name: content
  type: object
- description: A map of operations links that can be followed from the response.
  name: links
  type: object
provider_name: OpenAPI
provider_slug: openapi
schema_file: json-schema/openapi-response.json
slug: openapi-response
source_filename: openapi-response.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"openapi-response.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OpenAPI Response Object\",\n  \"description\": \"Describes a single response from an API Operation, including design-time, static links to operations based on the response.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"description\"\n  ],\n  \"properties\": {\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the response.\"\n    },\n    \"headers\": {\n      \"type\": \"object\",\n      \"description\": \"Maps a header name to its definition.\",\n      \"additionalProperties\": {\n        \"$ref\": \"openapi-header.json\"\n      }\n    },\n    \"content\": {\n      \"type\": \"object\",\n      \"description\": \"A map containing the representations for the response.\",\n      \"additionalProperties\": {\n        \"$ref\": \"openapi-media-type.json\"\n      }\n    },\n    \"links\": {\n      \"type\"\
  : \"object\",\n      \"description\": \"A map of operations links that can be followed from the response.\",\n      \"additionalProperties\": {\n        \"$ref\": \"openapi-link.json\"\n      }\n    }\n  },\n  \"patternProperties\": {\n    \"^x-\": {}\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openapi/refs/heads/main/json-schema/openapi-response.json
tags:
- Documentation
- REST
- Specification
title: OpenAPI Response Object
---
