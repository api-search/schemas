---
description: The placeholder information that uniquely identifies a placeholder shape.
layout: schema
name: Placeholder
properties_list:
- description: The type of the placeholder.
  name: type
  type: string
- description: The index of the placeholder. If the same placeholder types are present in the same page, they would have different index values.
  name: index
  type: integer
- description: The object ID of this shape's parent placeholder.
  name: parentObjectId
  type: string
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-placeholder-schema.json
slug: google-slides-placeholder
source_filename: google-slides-placeholder-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Placeholder\",\n  \"type\": \"object\",\n  \"description\": \"The placeholder information that uniquely identifies a placeholder shape.\\n\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the placeholder.\"\n    },\n    \"index\": {\n      \"type\": \"integer\",\n      \"description\": \"The index of the placeholder. If the same placeholder types are present in the same page, they would have different index values.\\n\"\n    },\n    \"parentObjectId\": {\n      \"type\": \"string\",\n      \"description\": \"The object ID of this shape's parent placeholder.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-placeholder-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: Placeholder
---
