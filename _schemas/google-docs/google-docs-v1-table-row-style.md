---
description: Style properties for a table row.
layout: schema
name: TableRowStyle
properties_list:
- description: Whether the row is a table header.
  name: tableHeader
  type: boolean
- description: Whether the row cannot overflow across page or column boundaries.
  name: preventOverflow
  type: boolean
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-table-row-style-schema.json
slug: google-docs-v1-table-row-style
source_filename: google-docs-v1-table-row-style-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TableRowStyle\",\n  \"type\": \"object\",\n  \"description\": \"Style properties for a table row.\",\n  \"properties\": {\n    \"tableHeader\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the row is a table header.\"\n    },\n    \"preventOverflow\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the row cannot overflow across page or column boundaries.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-table-row-style-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: TableRowStyle
---
