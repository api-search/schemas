---
description: ''
layout: schema
name: LibraryAttributes
properties_list:
- description: The name of the library.
  name: name
  type: string
- description: The current publishing state.
  name: state
  type: string
- description: Whether the library needs a new build.
  name: build_required
  type: boolean
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: Adobe Launch
provider_slug: adobe-launch
schema_file: json-schema/reactor-library-attributes-schema.json
slug: reactor-library-attributes
source_filename: reactor-library-attributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LibraryAttributes\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the library.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The current publishing state.\"\n    },\n    \"build_required\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the library needs a new build.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/json-schema/reactor-library-attributes-schema.json
tags:
- Data Collection
- Edge Network
- Event Forwarding
- Marketing Technology
- Tag Management
title: LibraryAttributes
---
