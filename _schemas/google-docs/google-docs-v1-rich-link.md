---
description: A link to a Google resource such as a file in Drive, a YouTube video, or a Calendar event.
layout: schema
name: RichLink
properties_list:
- description: Output only. The ID of this link.
  name: richLinkId
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
schema_file: json-schema/google-docs-v1-rich-link-schema.json
slug: google-docs-v1-rich-link
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RichLink\",\n  \"type\": \"object\",\n  \"description\": \"A link to a Google resource such as a file in Drive, a YouTube video, or a Calendar event.\",\n  \"properties\": {\n    \"richLinkId\": {\n      \"type\": \"string\",\n      \"description\": \"Output only. The ID of this link.\"\n    },\n    \"suggestedInsertionIds\": {\n      \"type\": \"array\"\n    },\n    \"suggestedDeletionIds\": {\n      \"type\": \"array\"\n    },\n    \"suggestedTextStyleChanges\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-rich-link-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: RichLink
---
