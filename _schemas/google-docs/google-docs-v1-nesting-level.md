---
description: Contains properties describing the look and feel of a list bullet at a given level of nesting.
layout: schema
name: NestingLevel
properties_list:
- description: The alignment of the bullet within the space allotted for rendering.
  name: bulletAlignment
  type: string
- description: The format string used by bullets at this level of nesting.
  name: glyphFormat
  type: string
- description: The number of the first list item at this nesting level.
  name: startNumber
  type: integer
- description: The type of glyph used by bullets at this nesting level.
  name: glyphType
  type: string
- description: A custom glyph symbol used by bullets at this nesting level.
  name: glyphSymbol
  type: string
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-nesting-level-schema.json
slug: google-docs-v1-nesting-level
source_filename: google-docs-v1-nesting-level-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NestingLevel\",\n  \"type\": \"object\",\n  \"description\": \"Contains properties describing the look and feel of a list bullet at a given level of nesting.\",\n  \"properties\": {\n    \"bulletAlignment\": {\n      \"type\": \"string\",\n      \"description\": \"The alignment of the bullet within the space allotted for rendering.\"\n    },\n    \"glyphFormat\": {\n      \"type\": \"string\",\n      \"description\": \"The format string used by bullets at this level of nesting.\"\n    },\n    \"startNumber\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of the first list item at this nesting level.\"\n    },\n    \"glyphType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of glyph used by bullets at this nesting level.\"\n    },\n    \"glyphSymbol\": {\n      \"type\": \"string\",\n      \"description\": \"A custom glyph symbol used by bullets at\
  \ this nesting level.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-nesting-level-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: NestingLevel
---
