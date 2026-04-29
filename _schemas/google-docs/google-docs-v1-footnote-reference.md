---
description: A ParagraphElement representing a footnote reference.
layout: schema
name: FootnoteReference
properties_list:
- description: The ID of the footnote that contains the content of this footnote reference.
  name: footnoteId
  type: string
- description: Output only. The rendered number of this footnote.
  name: footnoteNumber
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
schema_file: json-schema/google-docs-v1-footnote-reference-schema.json
slug: google-docs-v1-footnote-reference
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FootnoteReference\",\n  \"type\": \"object\",\n  \"description\": \"A ParagraphElement representing a footnote reference.\",\n  \"properties\": {\n    \"footnoteId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the footnote that contains the content of this footnote reference.\"\n    },\n    \"footnoteNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Output only. The rendered number of this footnote.\"\n    },\n    \"suggestedInsertionIds\": {\n      \"type\": \"array\"\n    },\n    \"suggestedDeletionIds\": {\n      \"type\": \"array\"\n    },\n    \"suggestedTextStyleChanges\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-footnote-reference-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: FootnoteReference
---
