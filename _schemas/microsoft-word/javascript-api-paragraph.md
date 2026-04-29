---
description: Represents a single paragraph in a Word document.
layout: schema
name: Paragraph
properties_list:
- description: Unique identifier of the paragraph.
  name: id
  type: string
- description: Plain text content of the paragraph.
  name: text
  type: string
- description: Style name applied to the paragraph.
  name: style
  type: string
- description: Text alignment (Left, Centered, Right, Justified).
  name: alignment
  type: string
- description: First line indent value in points.
  name: firstLineIndent
  type: number
- description: Line spacing in points.
  name: lineSpacing
  type: number
- description: Outline level of the paragraph.
  name: outlineLevel
  type: integer
- description: Whether the paragraph is part of a list.
  name: isListItem
  type: boolean
provider_name: Microsoft Word
provider_slug: microsoft-word
schema_file: json-schema/javascript-api-paragraph-schema.json
slug: javascript-api-paragraph
source_filename: javascript-api-paragraph-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/json-schema/javascript-api-paragraph-schema.json\",\n  \"title\": \"Paragraph\",\n  \"description\": \"Represents a single paragraph in a Word document.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the paragraph.\"\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"Plain text content of the paragraph.\"\n    },\n    \"style\": {\n      \"type\": \"string\",\n      \"description\": \"Style name applied to the paragraph.\"\n    },\n    \"alignment\": {\n      \"type\": \"string\",\n      \"description\": \"Text alignment (Left, Centered, Right, Justified).\",\n      \"enum\": [\"Left\", \"Centered\", \"Right\", \"Justified\"]\n    },\n    \"firstLineIndent\": {\n      \"type\": \"number\",\n   \
  \   \"description\": \"First line indent value in points.\"\n    },\n    \"lineSpacing\": {\n      \"type\": \"number\",\n      \"description\": \"Line spacing in points.\"\n    },\n    \"outlineLevel\": {\n      \"type\": \"integer\",\n      \"description\": \"Outline level of the paragraph.\",\n      \"minimum\": 1,\n      \"maximum\": 9\n    },\n    \"isListItem\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the paragraph is part of a list.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/json-schema/javascript-api-paragraph-schema.json
tags:
- Documents
- Microsoft 365
- Office
- Productivity
- Word Processing
title: Paragraph
---
