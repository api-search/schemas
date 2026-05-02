---
description: An indexed documentation library representing a software package or framework whose documentation has been scraped and stored for AI-assisted search.
layout: schema
name: grounded.tools Library
properties_list:
- description: Library name used to identify the documentation source.
  name: name
  type: string
- description: A list of indexed versions available for this library.
  name: versions
  type: array
provider_name: Grounded.tools
provider_slug: grounded-tools
schema_file: json-schema/library.json
slug: library
source_filename: library.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/grounded-tools/blob/main/json-schema/library.json\",\n  \"title\": \"grounded.tools Library\",\n  \"description\": \"An indexed documentation library representing a software package or framework whose documentation has been scraped and stored for AI-assisted search.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Library name used to identify the documentation source.\"\n    },\n    \"versions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"version.json\"\n      },\n      \"description\": \"A list of indexed versions available for this library.\"\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/grounded-tools/refs/heads/main/json-schema/library.json
tags:
- Developer Tools
- Developers
- Documentation
- Experience
title: grounded.tools Library
---
