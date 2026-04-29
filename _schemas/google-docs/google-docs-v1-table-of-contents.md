---
description: A StructuralElement representing a table of contents.
layout: schema
name: TableOfContents
properties_list:
- description: The content of the table of contents.
  name: content
  type: array
- description: ''
  name: suggestedInsertionIds
  type: array
- description: ''
  name: suggestedDeletionIds
  type: array
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-table-of-contents-schema.json
slug: google-docs-v1-table-of-contents
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TableOfContents\",\n  \"type\": \"object\",\n  \"description\": \"A StructuralElement representing a table of contents.\",\n  \"properties\": {\n    \"content\": {\n      \"type\": \"array\",\n      \"description\": \"The content of the table of contents.\"\n    },\n    \"suggestedInsertionIds\": {\n      \"type\": \"array\"\n    },\n    \"suggestedDeletionIds\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-table-of-contents-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: TableOfContents
---
