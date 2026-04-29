---
description: A ParagraphElement representing a spot in the text that is dynamically replaced with content that can change over time, like a page number.
layout: schema
name: AutoText
properties_list:
- description: The type of this auto text.
  name: type
  type: string
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
schema_file: json-schema/google-docs-v1-auto-text-schema.json
slug: google-docs-v1-auto-text
source_filename: google-docs-v1-auto-text-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AutoText\",\n  \"type\": \"object\",\n  \"description\": \"A ParagraphElement representing a spot in the text that is dynamically replaced with content that can change over time, like a page number.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of this auto text.\"\n    },\n    \"suggestedInsertionIds\": {\n      \"type\": \"array\"\n    },\n    \"suggestedDeletionIds\": {\n      \"type\": \"array\"\n    },\n    \"suggestedTextStyleChanges\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-auto-text-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: AutoText
---
