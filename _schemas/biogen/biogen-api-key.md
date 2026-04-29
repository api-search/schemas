---
description: A developer API key for accessing Biogen services.
layout: schema
name: ApiKey
properties_list:
- description: Key ID.
  name: id
  type: string
- description: Key display name.
  name: name
  type: string
- description: The API key value (shown once at creation).
  name: key
  type: string
- description: Key status.
  name: status
  type: string
- description: Key creation timestamp.
  name: created_at
  type: string
- description: ''
  name: usage
  type: object
provider_name: Biogen
provider_slug: biogen
schema_file: json-schema/biogen-api-key-schema.json
slug: biogen-api-key
source_filename: biogen-api-key-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ApiKey\",\n  \"type\": \"object\",\n  \"description\": \"A developer API key for accessing Biogen services.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Key ID.\",\n      \"example\": \"key-abc123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Key display name.\",\n      \"example\": \"Production Key\"\n    },\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The API key value (shown once at creation).\",\n      \"example\": \"bde7f3...\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Key status.\",\n      \"enum\": [\n        \"active\",\n        \"inactive\",\n        \"revoked\"\n      ],\n      \"example\": \"active\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Key creation timestamp.\"\
  ,\n      \"example\": \"2024-01-01T00:00:00Z\"\n    },\n    \"usage\": {\n      \"$ref\": \"#/components/schemas/ApiKeyUsage\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/biogen/refs/heads/main/json-schema/biogen-api-key-schema.json
tags:
- Biotechnology
- Healthcare
- Life Sciences
- Pharmaceuticals
- Neurology
title: ApiKey
---
