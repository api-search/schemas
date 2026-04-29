---
description: Updates the style of a table row.
layout: schema
name: UpdateTableRowStyleRequest
properties_list:
- description: The list of zero-based row indices whose style should be updated.
  name: rowIndices
  type: array
- description: The fields that should be updated.
  name: fields
  type: string
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-update-table-row-style-request-schema.json
slug: google-docs-v1-update-table-row-style-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateTableRowStyleRequest\",\n  \"type\": \"object\",\n  \"description\": \"Updates the style of a table row.\",\n  \"properties\": {\n    \"rowIndices\": {\n      \"type\": \"array\",\n      \"description\": \"The list of zero-based row indices whose style should be updated.\"\n    },\n    \"fields\": {\n      \"type\": \"string\",\n      \"description\": \"The fields that should be updated.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-update-table-row-style-request-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: UpdateTableRowStyleRequest
---
