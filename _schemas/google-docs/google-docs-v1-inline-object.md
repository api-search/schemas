---
description: An object that appears inline with text. An InlineObject contains an EmbeddedObject such as an image.
layout: schema
name: InlineObject
properties_list:
- description: The ID of this inline object.
  name: objectId
  type: string
- description: ''
  name: suggestedInlineObjectPropertiesChanges
  type: object
- description: ''
  name: suggestedInsertionId
  type: string
- description: ''
  name: suggestedDeletionIds
  type: array
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-inline-object-schema.json
slug: google-docs-v1-inline-object
source_filename: google-docs-v1-inline-object-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InlineObject\",\n  \"type\": \"object\",\n  \"description\": \"An object that appears inline with text. An InlineObject contains an EmbeddedObject such as an image.\",\n  \"properties\": {\n    \"objectId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of this inline object.\"\n    },\n    \"suggestedInlineObjectPropertiesChanges\": {\n      \"type\": \"object\"\n    },\n    \"suggestedInsertionId\": {\n      \"type\": \"string\"\n    },\n    \"suggestedDeletionIds\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-inline-object-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: InlineObject
---
