---
description: A person or email address mentioned in a document.
layout: schema
name: Person
properties_list:
- description: Output only. The unique ID of this link.
  name: personId
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
schema_file: json-schema/google-docs-v1-person-schema.json
slug: google-docs-v1-person
source_filename: google-docs-v1-person-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Person\",\n  \"type\": \"object\",\n  \"description\": \"A person or email address mentioned in a document.\",\n  \"properties\": {\n    \"personId\": {\n      \"type\": \"string\",\n      \"description\": \"Output only. The unique ID of this link.\"\n    },\n    \"suggestedInsertionIds\": {\n      \"type\": \"array\"\n    },\n    \"suggestedDeletionIds\": {\n      \"type\": \"array\"\n    },\n    \"suggestedTextStyleChanges\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-person-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: Person
---
