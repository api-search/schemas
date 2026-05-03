---
description: Metadata about the API described by the OpenAPI document.
layout: schema
name: OpenAPI Info Object
properties_list:
- description: The title of the API.
  name: title
  type: string
- description: A short summary of the API.
  name: summary
  type: string
- description: A description of the API. CommonMark syntax may be used.
  name: description
  type: string
- description: A URL to the Terms of Service for the API.
  name: termsOfService
  type: string
- description: ''
  name: contact
  type: object
- description: ''
  name: license
  type: object
- description: The version of the API document.
  name: version
  type: string
provider_name: OpenAPI
provider_slug: openapi
schema_file: json-schema/openapi-info.json
slug: openapi-info
source_filename: openapi-info.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"openapi-info.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OpenAPI Info Object\",\n  \"description\": \"Metadata about the API described by the OpenAPI document.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"title\",\n    \"version\"\n  ],\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the API.\"\n    },\n    \"summary\": {\n      \"type\": \"string\",\n      \"description\": \"A short summary of the API.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the API. CommonMark syntax may be used.\"\n    },\n    \"termsOfService\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"A URL to the Terms of Service for the API.\"\n    },\n    \"contact\": {\n      \"$ref\": \"openapi-contact.json\"\n    },\n    \"license\": {\n      \"$ref\": \"openapi-license.json\"\n\
  \    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"The version of the API document.\"\n    }\n  },\n  \"patternProperties\": {\n    \"^x-\": {}\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openapi/refs/heads/main/json-schema/openapi-info.json
tags:
- Documentation
- REST
- Specification
title: OpenAPI Info Object
---
