---
description: A document header.
layout: schema
name: Header
properties_list:
- description: Output only. The ID of the header.
  name: headerId
  type: string
- description: The contents of the header.
  name: content
  type: array
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-header-schema.json
slug: google-docs-v1-header
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Header\",\n  \"type\": \"object\",\n  \"description\": \"A document header.\",\n  \"properties\": {\n    \"headerId\": {\n      \"type\": \"string\",\n      \"description\": \"Output only. The ID of the header.\"\n    },\n    \"content\": {\n      \"type\": \"array\",\n      \"description\": \"The contents of the header.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-header-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: Header
---
