---
description: A List represents the list attributes for a group of paragraphs that all belong to the same list.
layout: schema
name: List
properties_list:
- description: ''
  name: suggestedListPropertiesChanges
  type: object
- description: ''
  name: suggestedInsertionId
  type: string
- description: ''
  name: suggestedDeletionIds
  type: array
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-list-schema.json
slug: google-docs-v1-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"List\",\n  \"type\": \"object\",\n  \"description\": \"A List represents the list attributes for a group of paragraphs that all belong to the same list.\",\n  \"properties\": {\n    \"suggestedListPropertiesChanges\": {\n      \"type\": \"object\"\n    },\n    \"suggestedInsertionId\": {\n      \"type\": \"string\"\n    },\n    \"suggestedDeletionIds\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-list-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: List
---
