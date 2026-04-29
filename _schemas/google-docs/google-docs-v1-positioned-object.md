---
description: An object that is tethered to a paragraph and positioned relative to the beginning of the paragraph.
layout: schema
name: PositionedObject
properties_list:
- description: The ID of this positioned object.
  name: objectId
  type: string
- description: ''
  name: suggestedPositionedObjectPropertiesChanges
  type: object
- description: ''
  name: suggestedInsertionId
  type: string
- description: ''
  name: suggestedDeletionIds
  type: array
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-positioned-object-schema.json
slug: google-docs-v1-positioned-object
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PositionedObject\",\n  \"type\": \"object\",\n  \"description\": \"An object that is tethered to a paragraph and positioned relative to the beginning of the paragraph.\",\n  \"properties\": {\n    \"objectId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of this positioned object.\"\n    },\n    \"suggestedPositionedObjectPropertiesChanges\": {\n      \"type\": \"object\"\n    },\n    \"suggestedInsertionId\": {\n      \"type\": \"string\"\n    },\n    \"suggestedDeletionIds\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-positioned-object-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: PositionedObject
---
