---
description: A document footnote.
layout: schema
name: Footnote
properties_list:
- description: Output only. The ID of the footnote.
  name: footnoteId
  type: string
- description: The contents of the footnote.
  name: content
  type: array
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-footnote-schema.json
slug: google-docs-v1-footnote
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Footnote\",\n  \"type\": \"object\",\n  \"description\": \"A document footnote.\",\n  \"properties\": {\n    \"footnoteId\": {\n      \"type\": \"string\",\n      \"description\": \"Output only. The ID of the footnote.\"\n    },\n    \"content\": {\n      \"type\": \"array\",\n      \"description\": \"The contents of the footnote.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-footnote-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: Footnote
---
