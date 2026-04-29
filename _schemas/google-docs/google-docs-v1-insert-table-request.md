---
description: Inserts a table at the specified location.
layout: schema
name: InsertTableRequest
properties_list:
- description: The number of rows in the table.
  name: rows
  type: integer
- description: The number of columns in the table.
  name: columns
  type: integer
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-insert-table-request-schema.json
slug: google-docs-v1-insert-table-request
source_filename: google-docs-v1-insert-table-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InsertTableRequest\",\n  \"type\": \"object\",\n  \"description\": \"Inserts a table at the specified location.\",\n  \"properties\": {\n    \"rows\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of rows in the table.\"\n    },\n    \"columns\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of columns in the table.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-insert-table-request-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: InsertTableRequest
---
