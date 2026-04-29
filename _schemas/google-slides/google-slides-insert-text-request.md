---
description: Inserts text into a shape or a table cell.
layout: schema
name: InsertTextRequest
properties_list:
- description: The object ID of the shape or table cell.
  name: objectId
  type: string
- description: The text to be inserted. Inserting a newline character will implicitly create a new ParagraphMarker.
  name: text
  type: string
- description: The index where the text will be inserted, in Unicode code units of the UTF-16 encoding.
  name: insertionIndex
  type: integer
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-insert-text-request-schema.json
slug: google-slides-insert-text-request
source_filename: google-slides-insert-text-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InsertTextRequest\",\n  \"type\": \"object\",\n  \"description\": \"Inserts text into a shape or a table cell.\",\n  \"properties\": {\n    \"objectId\": {\n      \"type\": \"string\",\n      \"description\": \"The object ID of the shape or table cell.\"\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"The text to be inserted. Inserting a newline character will implicitly create a new ParagraphMarker.\\n\"\n    },\n    \"insertionIndex\": {\n      \"type\": \"integer\",\n      \"description\": \"The index where the text will be inserted, in Unicode code units of the UTF-16 encoding.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-insert-text-request-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: InsertTextRequest
---
