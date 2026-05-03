---
description: Schema for a Zudoku API reference configuration that points to an OpenAPI schema document for generating interactive API documentation with playground support.
layout: schema
name: Zudoku API Reference
properties_list:
- description: How the OpenAPI document is loaded. Use 'file' for local filesystem paths (recommended) or 'url' for remote HTTP endpoints.
  name: type
  type: string
- description: Path, URL, or array of paths to OpenAPI document(s). Supports JSON and YAML formats.
  name: input
  type: object
- description: Identifier used for linking this API reference to sidebar navigation sections.
  name: navigationId
  type: string
- description: Display label for the API reference in navigation and catalog views.
  name: label
  type: string
- description: Override the server URL defined in the OpenAPI document for playground requests.
  name: serverUrl
  type: string
provider_name: Zudoku
provider_slug: zudoku
schema_file: json-schema/api-reference.json
slug: api-reference
source_filename: api-reference.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/zudoku/blob/main/json-schema/api-reference.json\",\n  \"title\": \"Zudoku API Reference\",\n  \"description\": \"Schema for a Zudoku API reference configuration that points to an OpenAPI schema document for generating interactive API documentation with playground support.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"file\", \"url\"],\n      \"description\": \"How the OpenAPI document is loaded. Use 'file' for local filesystem paths (recommended) or 'url' for remote HTTP endpoints.\"\n    },\n    \"input\": {\n      \"oneOf\": [\n        {\n          \"type\": \"string\",\n          \"description\": \"Single path or URL to the OpenAPI document.\"\n        },\n        {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\"\
  : \"Array of file paths for versioned API documentation. Version metadata is automatically extracted from each OpenAPI schema at build time.\"\n        }\n      ],\n      \"description\": \"Path, URL, or array of paths to OpenAPI document(s). Supports JSON and YAML formats.\"\n    },\n    \"navigationId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier used for linking this API reference to sidebar navigation sections.\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"Display label for the API reference in navigation and catalog views.\"\n    },\n    \"serverUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Override the server URL defined in the OpenAPI document for playground requests.\"\n    }\n  },\n  \"required\": [\"type\", \"input\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zudoku/refs/heads/main/json-schema/api-reference.json
tags:
- Developer Tools
- Documentation
title: Zudoku API Reference
---
