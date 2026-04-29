---
description: Inserts an empty column into a table.
layout: schema
name: InsertTableColumnRequest
properties_list:
- description: Whether to insert new column to the right of the reference cell.
  name: insertRight
  type: boolean
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-insert-table-column-request-schema.json
slug: google-docs-v1-insert-table-column-request
source_filename: google-docs-v1-insert-table-column-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InsertTableColumnRequest\",\n  \"type\": \"object\",\n  \"description\": \"Inserts an empty column into a table.\",\n  \"properties\": {\n    \"insertRight\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to insert new column to the right of the reference cell.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-insert-table-column-request-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: InsertTableColumnRequest
---
