---
description: Each Media Type Object provides schema and examples for the media type identified by its key.
layout: schema
name: OpenAPI Media Type Object
properties_list:
- description: The schema defining the content of the request, response, or parameter.
  name: schema
  type: object
- description: Example of the media type in the specified format.
  name: example
  type: object
- description: Examples of the media type.
  name: examples
  type: object
- description: A map between a property name and its encoding information.
  name: encoding
  type: object
provider_name: OpenAPI
provider_slug: openapi
schema_file: json-schema/openapi-media-type.json
slug: openapi-media-type
source_filename: openapi-media-type.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"openapi-media-type.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OpenAPI Media Type Object\",\n  \"description\": \"Each Media Type Object provides schema and examples for the media type identified by its key.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"schema\": {\n      \"description\": \"The schema defining the content of the request, response, or parameter.\"\n    },\n    \"example\": {\n      \"description\": \"Example of the media type in the specified format.\"\n    },\n    \"examples\": {\n      \"type\": \"object\",\n      \"description\": \"Examples of the media type.\",\n      \"additionalProperties\": {\n        \"$ref\": \"openapi-example.json\"\n      }\n    },\n    \"encoding\": {\n      \"type\": \"object\",\n      \"description\": \"A map between a property name and its encoding information.\",\n      \"additionalProperties\": {\n        \"$ref\": \"openapi-encoding.json\"\n      }\n  \
  \  }\n  },\n  \"patternProperties\": {\n    \"^x-\": {}\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openapi/refs/heads/main/json-schema/openapi-media-type.json
tags:
- Documentation
- REST
- Specification
title: OpenAPI Media Type Object
---
