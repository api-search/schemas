---
description: A ParagraphElement representing a column break. A column break makes the subsequent text start at the top of the next column.
layout: schema
name: ColumnBreak
properties_list:
- description: ''
  name: suggestedInsertionIds
  type: array
- description: ''
  name: suggestedDeletionIds
  type: array
- description: ''
  name: suggestedTextStyleChanges
  type: object
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-column-break-schema.json
slug: google-docs-v1-column-break
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ColumnBreak\",\n  \"type\": \"object\",\n  \"description\": \"A ParagraphElement representing a column break. A column break makes the subsequent text start at the top of the next column.\",\n  \"properties\": {\n    \"suggestedInsertionIds\": {\n      \"type\": \"array\"\n    },\n    \"suggestedDeletionIds\": {\n      \"type\": \"array\"\n    },\n    \"suggestedTextStyleChanges\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-column-break-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: ColumnBreak
---
