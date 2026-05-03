---
description: Standard error response returned by the Zluri API.
layout: schema
name: Zluri API Error
properties_list:
- description: Error message describing what went wrong.
  name: error
  type: string
- description: Machine-readable error code.
  name: code
  type: string
provider_name: Zluri
provider_slug: zluri
schema_file: json-schema/error.json
slug: error
source_filename: error.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/zluri/refs/heads/main/json-schema/error.json\",\n  \"title\": \"Zluri API Error\",\n  \"description\": \"Standard error response returned by the Zluri API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"error\": {\n      \"type\": \"string\",\n      \"description\": \"Error message describing what went wrong.\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Machine-readable error code.\"\n    }\n  },\n  \"required\": [\"error\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zluri/refs/heads/main/json-schema/error.json
tags:
- Access Management
- SaaS Management
title: Zluri API Error
---
