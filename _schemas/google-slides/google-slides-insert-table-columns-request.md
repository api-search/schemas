---
description: Inserts columns into a table.
layout: schema
name: InsertTableColumnsRequest
properties_list:
- description: The table to insert columns into.
  name: tableObjectId
  type: string
- description: Whether to insert new columns to the right of the reference cell location.
  name: insertRight
  type: boolean
- description: The number of columns to be inserted.
  name: number
  type: integer
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-insert-table-columns-request-schema.json
slug: google-slides-insert-table-columns-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InsertTableColumnsRequest\",\n  \"type\": \"object\",\n  \"description\": \"Inserts columns into a table.\",\n  \"properties\": {\n    \"tableObjectId\": {\n      \"type\": \"string\",\n      \"description\": \"The table to insert columns into.\"\n    },\n    \"insertRight\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to insert new columns to the right of the reference cell location.\"\n    },\n    \"number\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of columns to be inserted.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-insert-table-columns-request-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: InsertTableColumnsRequest
---
