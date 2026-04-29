---
description: A magnitude in a single direction in the specified units.
layout: schema
name: Dimension
properties_list:
- description: The magnitude.
  name: magnitude
  type: number
- description: The units for magnitude.
  name: unit
  type: string
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-dimension-schema.json
slug: google-docs-v1-dimension
source_filename: google-docs-v1-dimension-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Dimension\",\n  \"type\": \"object\",\n  \"description\": \"A magnitude in a single direction in the specified units.\",\n  \"properties\": {\n    \"magnitude\": {\n      \"type\": \"number\",\n      \"description\": \"The magnitude.\"\n    },\n    \"unit\": {\n      \"type\": \"string\",\n      \"description\": \"The units for magnitude.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-dimension-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: Dimension
---
