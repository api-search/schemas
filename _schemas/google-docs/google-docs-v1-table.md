---
description: A StructuralElement representing a table.
layout: schema
name: Table
properties_list:
- description: Number of rows in the table.
  name: rows
  type: integer
- description: Number of columns in the table.
  name: columns
  type: integer
- description: The contents and style of each row.
  name: tableRows
  type: array
- description: ''
  name: suggestedInsertionIds
  type: array
- description: ''
  name: suggestedDeletionIds
  type: array
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-table-schema.json
slug: google-docs-v1-table
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Table\",\n  \"type\": \"object\",\n  \"description\": \"A StructuralElement representing a table.\",\n  \"properties\": {\n    \"rows\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of rows in the table.\"\n    },\n    \"columns\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of columns in the table.\"\n    },\n    \"tableRows\": {\n      \"type\": \"array\",\n      \"description\": \"The contents and style of each row.\"\n    },\n    \"suggestedInsertionIds\": {\n      \"type\": \"array\"\n    },\n    \"suggestedDeletionIds\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-table-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: Table
---
