---
description: Updates the properties of columns in a table.
layout: schema
name: UpdateTableColumnPropertiesRequest
properties_list:
- description: The list of zero-based column indices whose property should be updated.
  name: columnIndices
  type: array
- description: The fields that should be updated.
  name: fields
  type: string
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-update-table-column-properties-request-schema.json
slug: google-docs-v1-update-table-column-properties-request
source_filename: google-docs-v1-update-table-column-properties-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateTableColumnPropertiesRequest\",\n  \"type\": \"object\",\n  \"description\": \"Updates the properties of columns in a table.\",\n  \"properties\": {\n    \"columnIndices\": {\n      \"type\": \"array\",\n      \"description\": \"The list of zero-based column indices whose property should be updated.\"\n    },\n    \"fields\": {\n      \"type\": \"string\",\n      \"description\": \"The fields that should be updated.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-update-table-column-properties-request-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: UpdateTableColumnPropertiesRequest
---
