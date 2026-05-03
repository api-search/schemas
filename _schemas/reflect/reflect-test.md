---
description: Schema for a Reflect automated end-to-end test definition.
layout: schema
name: Reflect Test
properties_list:
- description: Unique integer identifier for the test.
  name: id
  type: integer
- description: Human-readable name for the test.
  name: name
  type: string
- description: Unix timestamp when the test was created.
  name: created
  type: integer
- description: List of tags for organizing and filtering tests.
  name: tags
  type: array
provider_name: Reflect
provider_slug: reflect
schema_file: json-schema/reflect-test-schema.json
slug: reflect-test
source_filename: reflect-test-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/reflect/json-schema/reflect-test-schema.json\",\n  \"title\": \"Reflect Test\",\n  \"description\": \"Schema for a Reflect automated end-to-end test definition.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique integer identifier for the test.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name for the test.\"\n    },\n    \"created\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp when the test was created.\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"List of tags for organizing and filtering tests.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\"id\", \"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/reflect/refs/heads/main/json-schema/reflect-test-schema.json
tags:
- AI Testing
- Artificial Intelligence
- Automated Testing
- CI/CD
- End-to-End Testing
- QA
- Testing
title: Reflect Test
---
