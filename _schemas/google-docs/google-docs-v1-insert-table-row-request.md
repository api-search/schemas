---
description: Inserts an empty row into a table.
layout: schema
name: InsertTableRowRequest
properties_list:
- description: Whether to insert new row below the reference cell location.
  name: insertBelow
  type: boolean
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-insert-table-row-request-schema.json
slug: google-docs-v1-insert-table-row-request
source_filename: google-docs-v1-insert-table-row-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InsertTableRowRequest\",\n  \"type\": \"object\",\n  \"description\": \"Inserts an empty row into a table.\",\n  \"properties\": {\n    \"insertBelow\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to insert new row below the reference cell location.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-insert-table-row-request-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: InsertTableRowRequest
---
