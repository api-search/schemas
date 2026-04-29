---
description: Describes the bullet of a paragraph.
layout: schema
name: Bullet
properties_list:
- description: The ID of the list this paragraph belongs to.
  name: listId
  type: string
- description: The nesting level of this paragraph in the list.
  name: nestingLevel
  type: integer
- description: The rendered bullet glyph for this paragraph.
  name: glyph
  type: string
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-bullet-schema.json
slug: google-slides-bullet
source_filename: google-slides-bullet-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Bullet\",\n  \"type\": \"object\",\n  \"description\": \"Describes the bullet of a paragraph.\",\n  \"properties\": {\n    \"listId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the list this paragraph belongs to.\"\n    },\n    \"nestingLevel\": {\n      \"type\": \"integer\",\n      \"description\": \"The nesting level of this paragraph in the list.\"\n    },\n    \"glyph\": {\n      \"type\": \"string\",\n      \"description\": \"The rendered bullet glyph for this paragraph.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-bullet-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: Bullet
---
