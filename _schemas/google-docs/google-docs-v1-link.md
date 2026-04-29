---
description: A reference to another portion of a document or an external URL.
layout: schema
name: Link
properties_list:
- description: An external URI.
  name: url
  type: string
- description: The ID of a bookmark in this document.
  name: bookmarkId
  type: string
- description: The ID of a heading in this document.
  name: headingId
  type: string
- description: The ID of a tab in this document.
  name: tabId
  type: string
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-link-schema.json
slug: google-docs-v1-link
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Link\",\n  \"type\": \"object\",\n  \"description\": \"A reference to another portion of a document or an external URL.\",\n  \"properties\": {\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"An external URI.\"\n    },\n    \"bookmarkId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of a bookmark in this document.\"\n    },\n    \"headingId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of a heading in this document.\"\n    },\n    \"tabId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of a tab in this document.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-link-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: Link
---
