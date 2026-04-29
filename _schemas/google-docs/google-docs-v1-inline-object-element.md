---
description: A ParagraphElement that contains an InlineObject.
layout: schema
name: InlineObjectElement
properties_list:
- description: The ID of the InlineObject this element contains.
  name: inlineObjectId
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
schema_file: json-schema/google-docs-v1-inline-object-element-schema.json
slug: google-docs-v1-inline-object-element
source_filename: google-docs-v1-inline-object-element-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InlineObjectElement\",\n  \"type\": \"object\",\n  \"description\": \"A ParagraphElement that contains an InlineObject.\",\n  \"properties\": {\n    \"inlineObjectId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the InlineObject this element contains.\"\n    },\n    \"suggestedInsertionIds\": {\n      \"type\": \"array\"\n    },\n    \"suggestedDeletionIds\": {\n      \"type\": \"array\"\n    },\n    \"suggestedTextStyleChanges\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-inline-object-element-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: InlineObjectElement
---
