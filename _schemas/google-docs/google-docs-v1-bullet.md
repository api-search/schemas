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
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-bullet-schema.json
slug: google-docs-v1-bullet
source_filename: google-docs-v1-bullet-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Bullet\",\n  \"type\": \"object\",\n  \"description\": \"Describes the bullet of a paragraph.\",\n  \"properties\": {\n    \"listId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the list this paragraph belongs to.\"\n    },\n    \"nestingLevel\": {\n      \"type\": \"integer\",\n      \"description\": \"The nesting level of this paragraph in the list.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-bullet-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: Bullet
---
